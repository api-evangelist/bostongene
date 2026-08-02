# BostonGene

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
