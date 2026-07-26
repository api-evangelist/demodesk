---
name: Fetch Demodesk recording insights
description: Retrieve a call recording plus its transcript, AI summaries, and coaching scorecards from the Demodesk v2 API.
api: openapi/demodesk-v2-openapi.yml
operations: [listRecordings, getRecording, getRecordingTranscript, listRecordingSummaries, listRecordingScorecards]
---

# Fetch Demodesk recording insights

Use the Demodesk Public v2 API to pull a sales call's recording and its AI-generated artifacts.

## Auth
Pass your API key as a Bearer token: `Authorization: Bearer YOUR_API_KEY`.
Generate the key in Demodesk under *Settings > Integrations > Other*. The key inherits
the creating user's permissions — use an admin key for company-wide access.
Base URL: `https://demodesk.com/api/v2`.

## Steps
1. `listRecordings` — page through recordings. Responses wrap results in `data[]`
   with a `meta` object; when `meta.hasNext` is true, pass `meta.nextCursor` back as
   the `cursor` param to get the next page.
2. `getRecording` with the recording `{token}` — get host, participants, meeting
   location, and statistics.
3. `getRecordingTranscript` with `{token}` — get the diarized transcript
   (speakers -> paragraphs -> sentences). For many recordings, prefer
   `batchGetRecordingsTranscripts` (POST `/transcripts/batch`).
4. `listRecordingSummaries` with `{token}` — AI summaries.
5. `listRecordingScorecards` with `{token}` — coaching scorecards (e.g. MEDDIC/BANT).

## Error handling
Errors return `{ "error": { "code", "message", "requestId" } }`. On 401 check the
Bearer token; on 404 the token is invalid or not visible to your key's user; on 429
back off and retry. Quote `error.requestId` to support@demodesk.com.
