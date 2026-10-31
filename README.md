# Polymath Robotics

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

Polymath Robotics builds general autonomy and safety software for off-highway and industrial vehicles such as tractors, loaders, dozers, and mining trucks. Its Synapse REST API lets developers command a real or simulated Polymath-powered vehicle: sending GPS and relative waypoints, issuing motion and vehicle commands, reading combined autonomy, navigation, and vehicle feedback, managing exclusive teleoperation control leases, and streaming media over LiveKit. Caladan, its browser-based simulation environment, lets teams build and test autonomous behaviors in Python without ROS, Gazebo, or Linux before deploying to physical machines. Founded in 2021 (YC S22), San Francisco.

**Areas:** Robotics · Autonomy · Industrial Vehicles · Off-Highway · Machine Learning · Simulation · Teleoperation · Automation · Artificial Intelligence · Unmanned Vehicles

## Polymath Robotics on APIs.io

Everything profiled for Polymath Robotics is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/polymath/](https://apis.io/providers/polymath/)** — or go straight to one of the APIs or properties below.

### APIs (10)

- [Polymath Robotics CANBus API](https://apis.io/apis/polymath/polymath-canbus-api/) — The CANBus API from Polymath Robotics — 1 operation(s) for canbus.
- [Polymath Robotics Filesystem API](https://apis.io/apis/polymath/polymath-filesystem-api/) — The filesystem API from Polymath Robotics — 3 operation(s) for filesystem.
- [Polymath Robotics Health Check API](https://apis.io/apis/polymath/polymath-health-check-api/) — Contains UUID endpoint that can be used to health check the robot
- [Polymath Robotics Livekit API](https://apis.io/apis/polymath/polymath-livekit-api/) — The Livekit API from Polymath Robotics — 4 operation(s) for livekit.
- [Polymath Robotics Media API](https://apis.io/apis/polymath/polymath-media-api/) — All endpoints related to interacting with Robot's media resources
- [Polymath Robotics Ros API](https://apis.io/apis/polymath/polymath-ros-api/) — The ros API from Polymath Robotics — 1 operation(s) for ros.
- [Polymath Robotics Systemd API](https://apis.io/apis/polymath/polymath-systemd-api/) — The systemd API from Polymath Robotics — 1 operation(s) for systemd.
- [Polymath Robotics Teleop Control API](https://apis.io/apis/polymath/polymath-teleop-control-api/) — Endpoints for managing control leases
- [Polymath Robotics Vehicle Autonomy API](https://apis.io/apis/polymath/polymath-vehicle-autonomy-api/) — All endpoints related to interacting with Robot's autonomy operations here
- [Polymath Robotics Vehicle Operations API](https://apis.io/apis/polymath/polymath-vehicle-operations-api/) — All endpoints related to interacting with Robot's vehicle operations here

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [polymath-synapse](https://apis.io/servers/polymath/polymath-synapse/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Polymath Agentic Access](https://apis.io/agentic-access/polymath/polymath-agentic-access/)

#### Collections (10)

Postman and Open Collection request collections.

- [Polymath API Service CANBus API](https://apis.io/collections/polymath/open-polymath-canbus-api/)
- [Polymath API Service CANBus filesystem API](https://apis.io/collections/polymath/open-polymath-filesystem-api/)
- [Polymath API Service CANBus Health Check API](https://apis.io/collections/polymath/open-polymath-health-check-api/)
- [Polymath API Service CANBus Livekit API](https://apis.io/collections/polymath/open-polymath-livekit-api/)
- [Polymath API Service CANBus Media API](https://apis.io/collections/polymath/open-polymath-media-api/)
- [Polymath API Service CANBus ros API](https://apis.io/collections/polymath/open-polymath-ros-api/)
- [Polymath API Service CANBus systemd API](https://apis.io/collections/polymath/open-polymath-systemd-api/)
- [Polymath API Service CANBus Teleop Control API](https://apis.io/collections/polymath/open-polymath-teleop-control-api/)
- [Polymath API Service CANBus Vehicle Autonomy API](https://apis.io/collections/polymath/open-polymath-vehicle-autonomy-api/)
- [Polymath API Service CANBus Vehicle Operations API](https://apis.io/collections/polymath/open-polymath-vehicle-operations-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Polymath Synapse V2 Overlay](https://apis.io/overlays/polymath/polymath-synapse-v2-overlay/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Polymath Authentication](https://apis.io/security/polymath/polymath-authentication/)
- [Polymath Domain Security](https://apis.io/security/polymath/polymath-domain-security/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.polymathrobotics.com/)
- [Documentation](https://synapse.docs.polymathrobotics.dev/docs/reference)
- [Getting started](https://synapse.docs.polymathrobotics.dev/docs/guides/authentication)
- [API reference](https://synapse.docs.polymathrobotics.dev/docs/reference)
- [Blog](https://www.polymathrobotics.com/blog)
- [Terms of service](https://www.polymathrobotics.com/legal/terms-of-service)
- [Privacy policy](https://www.polymathrobotics.com/legal/privacy-policy)
- [GitHub](https://github.com/polymathrobotics)

## API Evangelist rating

**Kin Score 37.0** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 43.8 |
| Contract governance | 4.5 |
| Operational transparency | 2.6 |
| Developer ergonomics | 66.1 |
| Access clarity | 21.1 |

**Agent readiness 26.4** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | verified |
| OpenAPI Examples | partial |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 22.7** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/polymath/](https://apis.io/providers/polymath/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Polymath Robotics: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/polymath/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
