# University of Calgary (university-of-calgary)

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
