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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

The Australian National University (ANU) is a public research university in Canberra, ranked #28 in the QS World University Rankings 2025. This repository catalogs ANU's public developer/API footprint as an [APIs.json](https://apisjson.org) profile for the API Evangelist network.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/anu/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=anu-api-evangelist&utm_content=repo

## Type

- Index
- Consumer
- 3rd-Party

## Tags

Education, Higher Education, University, Research, Australia, Open Data, Quantum

## APIs

- **QRNG@ANU Quantum Random Numbers API** — live quantum random numbers (uint8/uint16/hex16), no auth on the legacy endpoint; free API key on the newer service. Docs: https://qrng.anu.edu.au/contact/api-documentation/ — Base: `https://qrng.anu.edu.au/API/jsonI.php` — Signup: https://quantumnumbers.anu.edu.au/
- **ANU Open Research OAI-PMH** — OAI-PMH 2.0 metadata harvesting for the Open Research institutional repository (DSpace). Docs: https://openresearch.anu.edu.au/open-research-collections — Base: `https://openresearch-repository.anu.edu.au/server/oai/request`

## Plans, Rate Limits, and FinOps

- Plans / Pricing: [plans/anu-plans-pricing.yml](plans/anu-plans-pricing.yml)
- Rate Limits: [rate-limits/anu-rate-limits.yml](rate-limits/anu-rate-limits.yml)
- FinOps: [finops/anu-finops.yml](finops/anu-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-06-03

## Common Properties

- Website: https://www.anu.edu.au/
- GitHub: https://github.com/AustralianNationalUniversity
- LinkedIn: https://www.linkedin.com/school/the-australian-national-university/
- Review: [review.yml](review.yml)

## Notes

ANU does not operate a central institutional developer portal. The two APIs cataloged here were probed live on 2026-06-03 and returned valid responses. Timetabling (mytimetable.anu.edu.au) and programs/courses data are accessed via community-built scrapers rather than documented public APIs, so they were intentionally excluded to avoid fabricating endpoints. No endpoints were invented; see [review.yml](review.yml) for per-URL verification status.

## Maintainers

- Kin Lane — kin@apievangelist.com
