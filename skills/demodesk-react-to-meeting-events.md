---
name: React to Demodesk meeting events
description: Subscribe to Demodesk webhooks and enrich each event by calling the v2 API when a recording is ready.
api: openapi/demodesk-v2-openapi.yml
operations: [getRecording, getRecordingTranscript, listRecordingSummaries]
---

# React to Demodesk meeting events

Drive automations off Demodesk's webhook events, then pull the details via the v2 API.

## Enable webhooks
Demodesk webhooks are enabled on request: email support@demodesk.com with your HTTPS
endpoint URL and the events to activate. Event catalog (see
`asyncapi/demodesk-webhooks-asyncapi.yml`):
`demo.scheduled`, `demo.rescheduled`, `demo.handovered`, `demo.canceled`,
`demo.started`, `demo.ended`, `demo.call_note_updated`,
`demo.event_response_updated`, `recording.uploaded`,
`recording.transcription_postprocessed`.

## Steps
1. Receive the webhook POST. Read `meta.action` to route on the event type and
   `meta.createdAt` for ordering. Each payload carries the demo/recording identifiers
   plus any CRM ids.
2. On `recording.uploaded` — call `getRecording` with the recording token for full
   metadata.
3. On `recording.transcription_postprocessed` — call `getRecordingTranscript` and
   `listRecordingSummaries` to fetch the finished transcript and AI summary, then
   forward them to your CRM/workflow.
4. On `demo.*` lifecycle events — update your scheduling/CRM state.

## Notes
- Authenticate API calls with `Authorization: Bearer YOUR_API_KEY`.
- Treat webhooks as at-least-once: dedupe on the event identifiers.
- Errors use `{ "error": { "code", "message", "requestId" } }`; retry 429s with backoff.
