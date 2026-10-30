# Moxion Power Co

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

> **No longer operating.** This company or product has shut down, been discontinued, or been deprecated. This profile is kept as a historical record and is not maintained or rated.

Moxion Power Co is a mobile energy storage company (a Y Combinator alum) that builds trailer-mounted, zero-emission Mobile Power Units (MPUs) used as quiet, clean replacements for diesel generators on construction sites, film productions, events, and grid-support jobs. Moxion operated a REST Developer API that let fleet operators fetch device metadata, real-time GPS location, and time-series telemetry (state of charge, pack voltage, net/output power, energy available/capacity, cellular signal) for their Mobile Power Units, along with active fault codes. The API additionally exposed AEMP 2.0 (ISO 15143-3 v.20190501) compliant fleet-snapshot endpoints so telematics platforms could ingest Moxion equipment alongside other heavy-equipment fleets. Authentication used bearer tokens issued to Service Accounts. Note the company filed for bankruptcy in August 2024; the developer documentation remains online but the API host may no longer be operational.

**Areas:** Company · Energy Storage · Mobile Power · Battery · Telemetry · IoT · Fleet Management · Clean Energy · Construction · Device Metrics · Defunct

## Moxion Power Co on APIs.io (historical record)

Everything profiled for Moxion Power Co is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/moxion-power-co/](https://apis.io/providers/moxion-power-co/)** — or go straight to one of the APIs or properties below.

### APIs (6)

- [Moxion Power Co Device Faults API](https://apis.io/apis/moxion-power-co/moxion-power-co-device-faults-api/) — The Device Faults API from Moxion Power Co — 1 operation(s) for device faults.
- [Moxion Power Co Device Location API](https://apis.io/apis/moxion-power-co/moxion-power-co-device-location-api/) — The Device Location API from Moxion Power Co — 2 operation(s) for device location.
- [Moxion Power Co Device Metrics API](https://apis.io/apis/moxion-power-co/moxion-power-co-device-metrics-api/) — The Device Metrics API from Moxion Power Co — 1 operation(s) for device metrics.
- [Moxion Power Co Devices API](https://apis.io/apis/moxion-power-co/moxion-power-co-devices-api/) — The Devices API from Moxion Power Co — 2 operation(s) for devices.
- [Moxion Power Co Fleet Snapshot (AEMP) API](https://apis.io/apis/moxion-power-co/moxion-power-co-fleet-snapshot-aemp-api/) — The Fleet Snapshot (AEMP) API from Moxion Power Co — 3 operation(s) for fleet snapshot (aemp).
- [Moxion Power Co Organizations API](https://apis.io/apis/moxion-power-co/moxion-power-co-organizations-api/) — The Organizations API from Moxion Power Co — 1 operation(s) for organizations.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [moxion-power](https://apis.io/servers/moxion-power-co/moxion-power/)

#### Collections (6)

Postman and Open Collection request collections.

- [Moxion Power Developer Device Faults API](https://apis.io/collections/moxion-power-co/open-moxion-power-co-device-faults-api/)
- [Moxion Power Developer Device Faults Device Location API](https://apis.io/collections/moxion-power-co/open-moxion-power-co-device-location-api/)
- [Moxion Power Developer Device Faults Device Metrics API](https://apis.io/collections/moxion-power-co/open-moxion-power-co-device-metrics-api/)
- [Moxion Power Developer Device Faults Devices API](https://apis.io/collections/moxion-power-co/open-moxion-power-co-devices-api/)
- [Moxion Power Developer Device Faults Fleet Snapshot (AEMP) API](https://apis.io/collections/moxion-power-co/open-moxion-power-co-fleet-snapshot-aemp-api/)
- [Moxion Power Developer Device Faults Organizations API](https://apis.io/collections/moxion-power-co/open-moxion-power-co-organizations-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Moxion Power Co Openapi Overlay](https://apis.io/overlays/moxion-power-co/moxion-power-co-openapi-overlay/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Moxion Power Co Authentication](https://apis.io/security/moxion-power-co/moxion-power-co-authentication/)
- [Moxion Power Co Domain Security](https://apis.io/security/moxion-power-co/moxion-power-co-domain-security/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.moxionpower.com)
- [Documentation](https://developer.moxionpower.com/docs)
- [Getting started](https://developer.moxionpower.com/docs/getting-started)
- [API reference](https://developer.moxionpower.com/reference)
- [Sign up](https://developer.moxionpower.com/login)
- [Blog](https://viridiparente.com/feed/)

## API Evangelist rating

**Not rated** — this company is recorded as no longer operating, so no score is published. If it is in fact operating, say so on this repository and it will be re-profiled.

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Moxion Power Co: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/moxion-power-co/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
