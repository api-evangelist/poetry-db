# PoetryDB

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
