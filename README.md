# Australian National University

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

The Australian National University (ANU) is a public research university in Canberra and a member of the Group of Eight, ranked #27 in the QS World University Rankings order used by this cohort. Like almost every university, ANU is a federation of buyers rather than an API producer: it operates no central developer portal, no institutional API gateway (api.anu.edu.au and developer.anu.edu.au do not resolve), and publishes no OpenAPI for anything. What it does operate is small, real and genuinely its own — the ANU Quantum Numbers (AQN) service serving live quantum random numbers from the ANU Quantum Optics group, a deprecated predecessor endpoint at qrng.anu.edu.au throttled to one request per minute, a self-hosted DSpace 7.6.7 institutional repository exposing a conformant OAI-PMH 2.0 interface across twelve metadata formats plus a HAL+JSON REST API, and a Shibboleth identity provider registered in the Australian Access Federation and interfederated through eduGAIN. ANU is a DataCite member in its own right, holding DOI prefix 10.25911 with 25,559 registered DOIs. Its research information portal, by contrast, is an Elsevier Pure tenancy (researchportalplus.anu.edu.au CNAMEs to elsevierpure.com) — ANU's data on Elsevier's contract, recorded here as a tenant relationship and deliberately not credited as ANU engineering. Course, timetable and student systems are gated; the widely used ANU timetable tool is student-built by the Computer Science Students' Association on a non-ANU domain and is not endorsed on ANU's own timetabling pages.

**Areas:** University · Higher Education · Education · Research · Australia · Group of Eight · Research Repository · Identity Federation · Open Access · Quantum · Random Numbers · OAI-PMH

## Australian National University on APIs.io

Everything profiled for Australian National University is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/anu/](https://apis.io/providers/anu/)** — or go straight to one of the APIs or properties below.

### APIs (5)

- [ANU Open Research DSpace REST API](https://apis.io/apis/anu/openresearch-rest/) — The HAL+JSON REST API of ANU's self-hosted DSpace 7.6.7 repository, reachable anonymously at /server/api for the root and discovery resources;…
- [ANU Shibboleth Identity Provider (SAML 2.0 metadata)](https://apis.io/apis/anu/identity-federation/) — ANU's institutional identity provider, publishing machine-readable SAML 2.0 metadata at a stable URL. entityID https://idp2.anu.edu.au/idp/shibboleth,…
- [ANU Research Portal Plus (Elsevier Pure) — TENANT](https://apis.io/apis/anu/research-portal-pure/) — ANU's research information portal and public researcher/output profiles, running on Elsevier Pure. This is a genuine institutional fact and one of the few…
- [Australian National University Harvesting API](https://apis.io/apis/anu/anu-harvesting-api/) — OAI-PMH verbs for metadata harvesting.
- [Australian National University Random Numbers API](https://apis.io/apis/anu/anu-random-numbers-api/) — Retrieval of quantum-generated random values.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### JSON Schema (2)

The data models the API reads and writes.

- [ANU Quantum Numbers request parameters](https://apis.io/schemas/anu/anu-quantum-numbers-request/)
- [ANU Quantum Numbers response](https://apis.io/schemas/anu/anu-quantum-numbers-response/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Anu Context](https://apis.io/jsonld/anu/anu-context/)

#### Examples (3)

Example requests and responses.

- [Anu Qrng Legacy Uint8 Example](https://apis.io/examples/anu/anu-qrng-legacy-uint8-example/)
- [Anu Quantum Numbers Forbidden Example](https://apis.io/examples/anu/anu-quantum-numbers-forbidden-example/)
- [Anu Quantum Numbers Hex16 Example](https://apis.io/examples/anu/anu-quantum-numbers-hex16-example/)

#### Governance rules (1)

Spectral rulesets for the provider's contracts.

- [Australian National University API Rules](https://apis.io/rules/anu/anu-rules/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Anu Authentication](https://apis.io/security/anu/anu-authentication/)
- [Anu Domain Security](https://apis.io/security/anu/anu-domain-security/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Anu Scopes](https://apis.io/scopes/anu/anu-scopes/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Anu Plans Pricing](https://apis.io/plans/anu/anu-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Anu Rate Limits](https://apis.io/rate-limits/anu/anu-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Anu Finops](https://apis.io/finops/anu/anu-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.anu.edu.au/)
- [Documentation](https://qrng.anu.edu.au/contact/api-documentation/)
- [API reference](https://quantumnumbers.anu.edu.au/documentation)
- [Support](https://services.anu.edu.au/information-technology)
- [Blog](https://www.anu.edu.au/news)
- [Terms of service](https://www.anu.edu.au/disclaimer)
- [Privacy policy](https://www.anu.edu.au/privacy)
- [GitHub](https://github.com/ANUcybernetics)

## API Evangelist rating

**Kin Score 39.0** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 71.4 |
| Contract quality | 41.4 |
| Contract governance | 11.4 |
| Operational transparency | 18.4 |
| Developer ergonomics | 28.6 |
| Access clarity | 42.1 |

**Agent readiness 24.5** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | — |
| Reversibility Documented | na |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | na |
| Error Semantics | — |
| OpenAPI Examples | verified |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | na |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 42.2** — Education & Research

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/anu/](https://apis.io/providers/anu/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Australian National University: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/anu/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
