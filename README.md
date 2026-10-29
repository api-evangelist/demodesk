# Demodesk

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Demodesk is an AI Sales Agent platform for B2B revenue teams, founded in 2018 in Munich, Germany. Four AI agents (Assistant, Coach, Analyst, CRM Concierge) plus a custom AI Agent Builder record and transcribe sales conversations, generate summaries and scorecards, update CRMs (Salesforce, HubSpot, Pipedrive), coach reps, and flag at-risk deals. The company exposes a public REST API (v2, OpenAPI 3.1) for recordings, transcripts, AI summaries, scorecards, and users, authenticated with Bearer API keys, plus a webhook event surface for meeting and recording lifecycle events and an official hosted MCP server (OAuth2) at demodesk.com/mcp. GDPR-native with EU-only data residency (Azure Frankfurt) and ISO 27001:2022 certification.

**Areas:** Company · Sales · Artificial Intelligence · Conversation Intelligence · Video Conferencing · CRM · Transcription · Webhook · MCP

## Demodesk on APIs.io

Everything profiled for Demodesk is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/demodesk/](https://apis.io/providers/demodesk/)** — or go straight to one of the APIs or properties below.

### APIs (4)

- [Demodesk Externally recorded demos API](https://apis.io/apis/demodesk/demodesk-externally-recorded-demos-api/) — The Externally recorded demos API from Demodesk — 3 operation(s) for externally recorded demos.
- [Demodesk Recordings API](https://apis.io/apis/demodesk/demodesk-recordings-api/) — Endpoints to discover recordings and fetch related artifacts.
- [Demodesk Users API](https://apis.io/apis/demodesk/demodesk-users-api/) — Endpoints regarding user management.
- [Demodesk Public API](https://apis.io/apis/demodesk/demodesk-demodesk-public-api-api/) — The Demodesk Public API API from Demodesk — 0 operation(s) for demodesk public api.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### AsyncAPI (1)

Event-driven and webhook contracts.

- [Demodesk Webhooks](https://apis.io/asyncapis/demodesk/demodesk-webhooks-asyncapi/)

#### Event channels (10)

Individual events and webhooks the provider emits.

- [demo.call_note_updated](https://apis.io/channels/demodesk/demo-call-note-updated/)
- [demo.canceled](https://apis.io/channels/demodesk/demo-canceled/)
- [demo.ended](https://apis.io/channels/demodesk/demo-ended/)
- [demo.event_response_updated](https://apis.io/channels/demodesk/demo-event-response-updated/)
- [demo.handovered](https://apis.io/channels/demodesk/demo-handovered/)
- [demo.rescheduled](https://apis.io/channels/demodesk/demo-rescheduled/)
- [demo.scheduled](https://apis.io/channels/demodesk/demo-scheduled/)
- [demo.started](https://apis.io/channels/demodesk/demo-started/)
- [recording.transcription_postprocessed](https://apis.io/channels/demodesk/recording-transcription-postprocessed/)
- [recording.uploaded](https://apis.io/channels/demodesk/recording-uploaded/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [demodesk](https://apis.io/servers/demodesk/demodesk/)

#### Collections (3)

Postman and Open Collection request collections.

- [API V1 Externally recorded demos API](https://apis.io/collections/demodesk/open-demodesk-externally-recorded-demos-api/)
- [API V1 Externally recorded demos Recordings API](https://apis.io/collections/demodesk/open-demodesk-recordings-api/)
- [API V1 Externally recorded demos Users API](https://apis.io/collections/demodesk/open-demodesk-users-api/)

#### Overlays (2)

OpenAPI overlays, including conversational phrasing for each operation.

- [Demodesk V1 Overlay](https://apis.io/overlays/demodesk/demodesk-v1-overlay/)
- [Demodesk V2 Overlay](https://apis.io/overlays/demodesk/demodesk-v2-overlay/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Demodesk Authentication](https://apis.io/security/demodesk/demodesk-authentication/)
- [Demodesk Domain Security](https://apis.io/security/demodesk/demodesk-domain-security/)
- [Demodesk Trust Center](https://apis.io/security/demodesk/demodesk-trust-center/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Demodesk Scopes](https://apis.io/scopes/demodesk/demodesk-scopes/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Demodesk Plans Pricing](https://apis.io/plans/demodesk/demodesk-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Demodesk Rate Limits](https://apis.io/rate-limits/demodesk/demodesk-rate-limits/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://demodesk.com/)
- [Documentation](https://help.demodesk.com/en/collections/3177803-api-integrations)
- [API reference](https://help.demodesk.com/en/articles/8518816-api-reference)
- [Pricing](https://demodesk.com/pricing)
- [Sign up](https://demodesk.com/manage/auth/register?seatType=ci)
- [Support](https://help.demodesk.com)
- [Blog](https://demodesk.com/blog)
- [Compliance](https://security.demodesk.com)
- [Terms of service](https://demodesk.com/legal/terms-of-use)
- [Privacy policy](https://demodesk.com/legal/privacy-policy)
- [GitHub](https://github.com/demodesk)
- [Status](https://status.demodesk.com)

## API Evangelist rating

**Kin Score 57.9** — strong · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 66.7 |
| Contract quality | 59.1 |
| Contract governance | 4.5 |
| Operational transparency | 60.5 |
| Developer ergonomics | 47.0 |
| Access clarity | 84.2 |

**Agent readiness 56.2** — agent-ready (gated down from agent-native)

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | documented (partial credit) |
| MCP Server | verified |
| Auth Clarity | served (partial credit) |
| Idempotency | — |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | partial |
| Rate Limit Signal | verified |
| Event Surface Described | yes |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | served (partial credit) |
| Protected Resource Metadata | verified |
| Dynamic Client Registration | yes |
| Agentic Commerce | — |
| Pagination Ratio | partial |
| Operation Distinctiveness | distinct |

**Regulatory alignment 31.8** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/demodesk/](https://apis.io/providers/demodesk/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Demodesk: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/demodesk/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
