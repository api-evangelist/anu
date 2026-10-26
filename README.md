# Australian National University (anu)

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

The Australian National University (ANU) is a public research university in Canberra and a member of the Group of Eight. This repository catalogs ANU's public developer/API footprint as an [APIs.json](https://apisjson.org) profile for the API Evangelist network.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/anu/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=anu-api-evangelist&utm_content=repo

## Type

- University (`x-type: university`) — Public Research University
- Index / Consumer / 3rd-Party

## Tags

University, Higher Education, Education, Research, Australia, Group of Eight, Research Repository, Identity Federation, Open Access, Quantum, Random Numbers, OAI-PMH

## Who operates what

A university is a federation of buyers, not an API producer. Every surface below carries an **operator**, settled by live probe on 2026-08-19 *before* anything was saved:

| Surface | Operator | Why |
|---|---|---|
| ANU Quantum Numbers (AQN) API | `institution` | `api.quantumnumbers.anu.edu.au` under ANU's domain, ANU's AWS account, ANU contact |
| QRNG@ANU legacy JSON API | `institution` | `qrng.anu.edu.au` → 150.203.48.55, ANU address space |
| ANU Open Research OAI-PMH | `institution` | `openresearch-repository.anu.edu.au` → `dspace-prod.anu.edu.au`, self-hosted DSpace |
| ANU Open Research DSpace REST | `institution` | Same self-hosted instance; contract shape is upstream DSpace's, so no spec is saved |
| ANU Shibboleth IdP (SAML metadata) | `institution` | Institution-operated by definition; registered in the AAF |
| ANU Research Portal Plus | **`tenant`** | CNAMEs to `anu2-portal.elsevierpure.com`; `x-product: Pure Portal`. ANU's data, **Elsevier's contract** |

No Elsevier Pure specification is saved in this repository, and none of Elsevier's engineering is scored as ANU's.

## APIs

- **ANU Quantum Numbers (AQN) API** — current quantum RNG service. `uint8`/`uint16`/`hex8`/`hex16`, length 1–1024, free self-serve `x-api-key`. Docs: https://quantumnumbers.anu.edu.au/documentation — Base: `https://api.quantumnumbers.anu.edu.au`
- **QRNG@ANU Legacy JSON API** — **deprecated**. No auth, throttled to **one request per minute**, and the throttle returns HTTP **200** with a plain-text sentence rather than a 429. Base: `https://qrng.anu.edu.au/API/jsonI.php`
- **ANU Open Research OAI-PMH** — OAI-PMH 2.0, twelve metadata formats, records carrying ORCID iDs and DOIs under ANU's own DataCite prefix `10.25911`. Base: `https://openresearch-repository.anu.edu.au/server/oai/request`
- **ANU Open Research DSpace REST API** — HAL+JSON, DSpace 7.6.7. Base: `https://openresearch-repository.anu.edu.au/server/api`
- **ANU Shibboleth Identity Provider** — SAML 2.0 metadata, entityID `https://idp2.anu.edu.au/idp/shibboleth`, scope `anu.edu.au`, in the Australian Access Federation and eduGAIN. A login federation, not a developer authorization surface.
- **ANU Research Portal Plus (Elsevier Pure)** — recorded as a **tenant relationship**, not an ANU API.

ANU publishes **no OpenAPI** for anything. Every specification under [`openapi/`](openapi/) is `derived` or `probed` by API Evangelist from ANU's own documentation and live responses, and is marked as such in `info.x-provenance`.

## Education-regime conformance

Probed against the Kin Score `education` regime standards — see [conformance/anu-conformance.yml](conformance/anu-conformance.yml):

- **Conforming:** `oai-pmh` (2.0), `shibboleth`, `saml` (2.0), `lti` (1.3, live JWKS on ANU's self-hosted Moodle), `orcid`, `datacite` (prefix 10.25911, 25,559 DOIs)
- **Not found:** `scim`, `oneroster`, `ed-fi`, `caliper`, `qti`, `crossref` (member 9402 exists with **0** deposited DOIs)

## Artifacts

- OpenAPI: [openapi/](openapi/) (pristine copies in [openapi/_original/](openapi/_original/))
- JSON Schema: [json-schema/](json-schema/) · Examples: [examples/](examples/) · Rules: [rules/](rules/) · Vocabulary: [vocabulary/](vocabulary/) · JSON-LD: [json-ld/](json-ld/)
- Authentication: [authentication/](authentication/) · Scopes: [scopes/](scopes/) · Errors: [errors/](errors/) · Conformance: [conformance/](conformance/) · Lifecycle: [lifecycle/](lifecycle/)
- Plans: [plans/anu-plans-pricing.yml](plans/anu-plans-pricing.yml) · Rate Limits: [rate-limits/anu-rate-limits.yml](rate-limits/anu-rate-limits.yml) · FinOps: [finops/anu-finops.yml](finops/anu-finops.yml) · Domain Security: [security/anu-domain-security.yml](security/anu-domain-security.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-08-19

## Common Properties

- Website: https://www.anu.edu.au/
- API Reference: https://quantumnumbers.anu.edu.au/documentation
- Research repository: https://openresearch.anu.edu.au/
- Open data / Data Commons: https://datacommons.anu.edu.au/DataCommons/
- Course catalog: https://programsandcourses.anu.edu.au/
- Identity federation: https://idp2.anu.edu.au/idp/shibboleth
- AI policy: https://www.anu.edu.au/privacy/training-and-resources/generative-ai-and-data-governance
- AI tooling guidance: https://libguides.anu.edu.au/generative-ai
- GitHub: https://github.com/AustralianNationalUniversity · https://github.com/ANUcybernetics · https://github.com/anu-hpc
- LinkedIn: https://www.linkedin.com/school/the-australian-national-university/
- Review: [review.yml](review.yml)

## Notes and deliberate exclusions

ANU operates **no central developer portal and no API gateway** — `api.anu.edu.au` and `developer.anu.edu.au` do not resolve. There is no `llms.txt`, no `.well-known/security.txt`, no OIDC discovery document, no status page and no changelog; each of those was confirmed by negative probe, not assumed.

Three things were deliberately **not** claimed:

- **NCI (nci.org.au)** — a national facility ANU collaborates in rather than operates. Its own "who we are" page describes a multi-agency collaboration, so its HPC surfaces are not credited to ANU.
- **timetable.cssa.club** — a student-built timetable scrape on a non-institutional domain. No endorsement of it was found on ANU's own timetabling pages, so it is not credited even as a tenant.
- **Wattle (Moodle) and library discovery** — behind authentication. Wattle is cited only as LTI 1.3 conformance evidence, not listed as a consumable API.

No endpoints were invented. See [review.yml](review.yml) and `x-coverage` in [apis.yml](apis.yml) for per-URL verification status.

## Maintainers

- Kin Lane — kin@apievangelist.com
