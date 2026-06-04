# Technical University of Berlin (tu-berlin)

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
