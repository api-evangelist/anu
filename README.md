# Australian National University (anu)

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
