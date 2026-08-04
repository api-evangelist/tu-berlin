# Technical University of Berlin (tu-berlin)

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

Technische Universität Berlin (TU Berlin) is a public research university in Berlin, Germany, ranked #66 in the QS World University Rankings 2025. This repository catalogs TU Berlin's public developer/API footprint as an [APIs.json](https://apisjson.org) provider profile. TU Berlin has no single unified developer portal; its confirmed machine-readable API surface centers on the DepositOnce research-data repository (DSpace 8.1), with a self-hosted GitLab instance gated behind Shibboleth SSO.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/tu-berlin/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=tu-berlin-api-evangelist&utm_content=repo

## Type

- **Type:** Index
- **Position:** Consumer
- **Access:** 3rd-Party

## Tags

Education, Higher Education, University, Research Data, Open Access, Repository, Library, Germany

## APIs

- **DepositOnce OAI-PMH Interface** — OAI-PMH 2.0 metadata harvesting for the TU Berlin institutional repository (DSpace 8.1). Base: `https://api-depositonce.tu-berlin.de/server/oai/request`. [Docs](https://depositonce.tu-berlin.de/info/help)
- **DepositOnce DSpace REST API** — DSpace 8.1 REST/HAL API exposing communities, collections, items and bitstreams. Base: `https://api-depositonce.tu-berlin.de/server/api`. [Docs](https://depositonce.tu-berlin.de/info/help)
- **TU Berlin GitLab API** — Self-hosted GitLab EE REST API (v4); gated, requires Shibboleth SSO (unauthenticated `/api/v4/` returns 401). Base: `https://git.tu-berlin.de/api/v4`. [Docs](https://www.tu.berlin/en/campusmanagement/news-details/gitlab-anmeldung-mit-shibboleth-single-sign-on)

## Plans / Rate Limits / FinOps

- [Plans & Pricing](plans/tu-berlin-plans-pricing.yml)
- [Rate Limits](rate-limits/tu-berlin-rate-limits.yml)
- [FinOps](finops/tu-berlin-finops.yml)

## Timestamps

- **Created:** 2026-06-03
- **Modified:** 2026-06-03

## Common Properties

- Website: https://www.tu.berlin/en
- GitHub: https://github.com/TU-Berlin
- SourceCode (Library): https://github.com/TUUB
- LinkedIn: https://www.linkedin.com/school/tu-berlin/
- Authentication (Shibboleth/SAML): https://www.tu.berlin/campusmanagement/angebot/shibboleth

## Notes

All endpoints were probed live on 2026-06-03. DepositOnce OAI-PMH and REST API returned HTTP 200 with valid responses (DSpace 8.1). The GitLab API is present but gated — `/api/v4/version` returned HTTP 401. The library "APIs for Scientific Resources" page lists only external third-party APIs (OECD, World Bank, IEEE Xplore, OpenAlex, etc.), not TU Berlin's own services. No endpoints were fabricated; see [review.yml](review.yml) for the full probe log.

## Maintainers

- Kin Lane — kin@apievangelist.com
