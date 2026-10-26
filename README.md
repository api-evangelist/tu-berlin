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

Technische Universität Berlin (TU Berlin) is a public technical research university in Berlin, Germany, and a member of the TU9 alliance and the Berlin University Alliance. This repository is an [APIs.json](https://apisjson.org) provider profile of its **public** programmable footprint, profiled under the API Evangelist university pipeline — where the first question is never "is there a spec" but **who operates the thing the spec describes**.

TU Berlin authors no API contract. There is no developer portal, no OpenAPI, no AsyncAPI, no apis.json, no llms.txt (404) and no security.txt (403). What it does operate is a set of standards-based deployments on its own hosts, and those are what this profile records — each one labelled with an operator.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/tu-berlin/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=tu-berlin-api-evangelist&utm_content=repo

## Type

- **Class:** university (`x-type: university`)
- **Category:** Technical University
- **Type:** Index · **Position:** Consumer · **Access:** 3rd-Party

## Tags

University, Higher Education, Education, Technical University, Germany, Berlin, Research Data, Open Access, Repository, Library, Identity Federation, Course Catalog, Research Computing

## Surfaces — and who operates them

All probed live and unauthenticated on **2026-08-30**.

| Surface | Operator | Status |
|---|---|---|
| **DepositOnce OAI-PMH** `api-depositonce.tu-berlin.de/server/oai/request` | institution | 200 — OAI-PMH 2.0, 15 metadata formats, DataCite DOIs under 10.14279 |
| **DepositOnce DSpace REST/HAL** `api-depositonce.tu-berlin.de/server/api` | institution | 200 — DSpace **9.4** (June said 8.1); discovery open, `/core/items` 401 |
| **Shibboleth IdP SAML metadata** `shibboleth.tu-berlin.de/idp/shibboleth` | institution | 200 — entityID `https://ephraim.tu-berlin.de/shibboleth`, DFN-AAI |
| **GitLab REST v4** `git.tu-berlin.de/api/v4` | institution | 200 for public projects (**2,851**, unauthenticated); `/version`, `/metadata`, `/mcp` 401 |
| **Matrix Client-Server API** `matrix.tu-berlin.de/_matrix/client` | institution | 200 — Synapse 1.157.2, versions r0.0.1–v1.12 |
| **ISIS (Moodle) LTI 1.3 platform** `isis.tu-berlin.de/mod/lti` | institution | 200 — public RS256 JWKS; Moodle web services enabled but token-gated |
| **tubCloud (Nextcloud)** `tubcloud.tu-berlin.de` | institution | 200 on `/status.php` only — WebDAV/OCS account-gated |
| **Library discovery (Ex Libris Primo)** `tu-berlin.hosted.exlibrisgroup.com` | **tenant** | 200 — TU Berlin's holdings, Ex Libris' contract |

**No vendor specification is saved under this slug.** The software behind DepositOnce, GitLab, Matrix and ISIS is DSpace's, GitLab's, Element/Matrix.org's and Moodle's; those products' generic specifications belong to their own profiles. Recording the deployment credits TU Berlin for what it actually runs without crediting it with someone else's engineering.

## Education-regime standards

Confirmed live (see [conformance](conformance/tu-berlin-conformance.yml)): **oai-pmh**, **saml**, **shibboleth**, **lti**, **datacite**.
Probed and **not** found: orcid, crossref, scim, oneroster, caliper, qti, ed-fi — recorded as absent rather than claimed.

## Corrections to the June 2026 profile

1. The GitLab API was recorded as fully gated. It is not — public project and group listings return 200 without a credential. Only `/version`, `/metadata` and `/mcp` are 401.
2. DepositOnce was recorded as DSpace 8.1. It reports **DSpace 9.4**.
3. Library discovery was not recorded at all; it is an Ex Libris Primo **tenant** and is now labelled as one.
4. Three institution-operated surfaces were missing entirely: the Shibboleth IdP metadata, the Matrix homeserver, and the ISIS LTI 1.3 platform.

## Artifacts

- [Conformance](conformance/tu-berlin-conformance.yml) · [Authentication](authentication/tu-berlin-authentication.yml) · [OAuth scopes](scopes/tu-berlin-scopes.yml) · [GitLab OIDC discovery](well-known/tu-berlin-gitlab-openid-configuration.json)
- [Plans & Pricing](plans/tu-berlin-plans-pricing.yml) · [Rate Limits](rate-limits/tu-berlin-rate-limits.yml) · [FinOps](finops/tu-berlin-finops.yml) · [Domain security](security/tu-berlin-domain-security.yml)
- [Probe log](review.yml)

## Institutional pointers

- Website: https://www.tu.berlin/en
- Identity federation: https://shibboleth.tu-berlin.de/idp/shibboleth · https://www.tu.berlin/campusmanagement/angebot/shibboleth
- Research repository: https://depositonce.tu-berlin.de/
- Course catalog (Moses VVZ): https://moseskonto.tu-berlin.de/moses/verzeichnis/index.html
- Research computing: https://hpc.wiki.tu-berlin.de/
- AI policy (ZEWK digit KI-Leitlinien): https://digit.zewk.wiki.tu-berlin.de/doku.php?id=ki:richtlinien
- AI tooling (ChatGPT Edu pilot): https://www.tu.berlin/en/wm/services/it-services-and-software/pilot-project-chatgpt-edu
- Service status: https://www.tu.berlin/campusmanagement/angebot/aktueller-dienste-status
- GitHub: https://github.com/TU-Berlin · https://github.com/tuub · GitLab: https://git.tu-berlin.de/explore/projects

## Timestamps

- **Created:** 2026-06-03
- **Modified:** 2026-08-30

## Maintainers

- Kin Lane — kin@apievangelist.com
