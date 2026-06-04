# University of Calgary (university-of-calgary)

The University of Calgary is a public research university in Calgary, Alberta, Canada, ranked #198 in the QS World University Rankings 2025. This repository catalogs the institution's real, public developer and API footprint as an APIs.json profile. Rather than a single central developer portal, UCalgary's documented APIs are research- and repository-driven: the Space Remote Sensing and AuroraX space-physics APIs, the PRISM institutional repository (DSpace), and the PRISM research-data collection on Borealis Dataverse.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/university-of-calgary/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=university-of-calgary-api-evangelist&utm_content=repo

## Type

- Index / Consumer / 3rd-Party

## Tags

- Education
- Higher Education
- University
- Research
- Open Data
- Repository
- Space Physics
- Canada

## APIs

- **UCalgary Space Remote Sensing API** — RESTful API for space physics and remote-sensing data (all-sky imagers, riometers); Swagger docs. Docs: https://api.phys.ucalgary.ca/ , https://data.phys.ucalgary.ca/working_with_data/
- **AuroraX API** — Public auroral-science data platform API (read open, key for writes); Python/IDL clients. Docs: https://docs.aurorax.space/ , https://api.aurorax.space/
- **PRISM Institutional Repository (DSpace)** — DSpace 8.3 REST API and OAI-PMH metadata harvesting. Docs: https://prism.ucalgary.ca/server/api , https://prism.ucalgary.ca/server/oai/request?verb=Identify
- **PRISM Research Data Repository (Borealis Dataverse)** — Dataverse REST API for the UCalgary research-data collection. Docs: https://borealisdata.ca/dataverse/calgary , https://guides.dataverse.org/en/latest/api/

## Plans, Rate Limits, and FinOps

- Plans: [plans/university-of-calgary-plans-pricing.yml](plans/university-of-calgary-plans-pricing.yml)
- Rate Limits: [rate-limits/university-of-calgary-rate-limits.yml](rate-limits/university-of-calgary-rate-limits.yml)
- FinOps: [finops/university-of-calgary-finops.yml](finops/university-of-calgary-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-06-03

## Common Properties

- Website: https://www.ucalgary.ca/
- GitHub: https://github.com/ucalgary
- LinkedIn: https://ca.linkedin.com/school/ucalgary/
- Developer Portal (library APIs guide): https://libguides.ucalgary.ca/apis
- Review: [review.yml](review.yml)

## Notes

All endpoints were probed live on 2026-06-03 and returned HTTP 200 unless noted in `review.yml`. No endpoints or properties were fabricated. The PRISM repository (`prism.ucalgary.ca`) now redirects to `ucalgary.scholaris.ca` and runs DSpace 8.3; the bare `/oai/request` path returns 404 while `/server/oai/request` responds. The library's "APIs" guide catalogs third-party scholarly APIs rather than first-party UCalgary endpoints. Most administrative, identity, course, and SIS interfaces are gated behind institutional SSO/affiliation and are not openly self-service.

## Maintainers

- Kin Lane — kin@apievangelist.com
