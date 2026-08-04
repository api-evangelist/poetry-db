# PoetryDB

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

PoetryDB is a public REST API providing programmatic access to a database of English-language poems. Developers can search the collection by author name, poem title, line content, and line count. The API requires no authentication or API key, returns JSON or plain text responses, and supports CORS.

**Base URL:** https://poetrydb.org

**GitHub:** https://github.com/thundercomb/poetrydb

## Endpoints

| Input Field | Example | Description |
|---|---|---|
| `/author` | `/author/Shakespeare` | Search poems by author name |
| `/title` | `/title/Sonnet 18` | Search poems by title |
| `/lines` | `/lines/Shall I compare` | Search by line content |
| `/linecount` | `/linecount/14` | Filter by number of lines |
| `/random` | `/random/3` | Retrieve random poems |

Append `:abs` for exact matching. Combine fields with commas. Select output fields by appending them to the path. Append `.text` for plain text output (default is JSON).

## Authentication

None required.

## Pricing

Free with no usage quotas or rate limits documented.

## Resources

- [APIs.json Profile](apis.yml)
- [Plans and Pricing](plans/poetry-db-plans-pricing.yml)
- [Rate Limits](rate-limits/poetry-db-rate-limits.yml)
- [FinOps](finops/poetry-db-finops.yml)
