# BostonGene

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

BostonGene is a Waltham, Massachusetts precision-oncology company that pairs an in-house CLIA-certified, CAP-accredited clinical laboratory with an AI-powered bioinformatics platform. It integrates whole-exome and whole-transcriptome sequencing, liquid biopsy (cfDNA/cfRNA), single-cell RNA sequencing, flow cytometry, spatial proteomics and digital pathology into multimodal molecular and immune profiling — sold to providers as the Tumor Portrait test, immune system profiling, an IHC test and an Unknown Primary test, and to biopharma as target analysis, biomarker discovery and clinical trial support.

- https://bostongene.com/
- https://bostongene.my.site.com/ (authenticated customer portal)
- https://github.com/BostonGene

## API surface

**None public.** As of the 2026-08-02 enrichment pass BostonGene publishes no developer API, no SDK, no API documentation, no OpenAPI/AsyncAPI/GraphQL contract, no MCP server, no A2A agent card and no `llms.txt`. Clinician ordering and report delivery run through an authenticated Salesforce Experience Cloud customer portal; accounts are provisioned by request, not self-service.

The only machine-readable document found on a BostonGene-controlled host is the portal's OpenID Connect discovery document — captured verbatim in `well-known/`.

## Artifacts

| Path | Type | Method |
|---|---|---|
| `well-known/bostongene-well-known.yml` | WellKnown | probed |
| `well-known/bostongene-openid-configuration.json` | — (verbatim) | probed |
| `authentication/bostongene-authentication.yml` | Authentication | probed |
| `scopes/bostongene-scopes.yml` | OAuthScopes | probed |
| `conformance/bostongene-conformance.yml` | Conformance | searched |
| `packages/bostongene-packages.yml` | Packages | searched |
| `security/bostongene-domain-security.yml` | DomainSecurity | probed |
| `llms/bostongene-llms.txt` | LLMsTxt | generated |

BostonGene publishes real laboratory accreditations (CLIA, CAP, New York State DOH, and MA/CA/MD/DC/PA/RI clinical laboratory licenses) at https://bostongene.com/news-and-publications/documents — captured in `conformance/`.
