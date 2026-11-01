# MCP Adoption Reference

Internal one-stop reference for the Model Context Protocol (MCP) adoption report appendix.

All figures below were gathered from live tool calls during this run. Items that could not be verified are explicitly marked.

---

## 1. Web Research: Google Search for "Model Context Protocol"

**Status: NOT VERIFIABLE.** The Google search scraper call returned an HTTP 429 error:

```
{"message":"Your current plan's quota has been reached. Upgrade your plan to continue scraping.","instance":"/v1/queries","timestamp":"2026-11-01T22:03:58.647842951Z","trace_id":"6ae7b74e-8670f7178ad9309e359e799b"}
```

A fallback attempt using the universal web scraper on `https://www.google.com/search?q=Model+Context+Protocol` also returned HTTP 429:

```
{"message":"Your current plan's quota has been reached. Upgrade your plan to continue scraping.","instance":"/v1/queries","timestamp":"2026-11-01T22:04:17.120838951Z","trace_id":"6ae7b760-5007776e63b7eb7b45c046f7"}
```

No page titles, URLs, or AI-overview fragments could be captured from the search. This section is therefore left empty rather than filled from memory.

---

## 2. Ecosystem Section

### 2.1 modelcontextprotocol/modelcontextprotocol

- **Full name:** `modelcontextprotocol/modelcontextprotocol`
- **Stars:** 9,584 (as reported by the GitHub API search result: `stargazers_count: 9584`)
- **Open issues:** 119 (as reported by the GitHub API search result: `open_issues_count: 119`; both `open_issues` and `open_issues_count` returned 119)
- **Default branch:** `main`
- **Latest commit on default branch (`main`):**
  - **SHA:** `d0e246ea3c69eafaa2806bc4cd28025703ba2c2b`
  - **Commit author date:** 2026-10-31T15:43:32Z
  - **Author:** claude[bot] (GitHub login: claude[bot]; email 209825114+claude[bot]@users.noreply.github.com; committed via web-flow)
  - **Commit message:** "Restructure Security IG as a routing group (#3331)"
- **Other API-reported fields:** description "Specification and documentation for the Model Context Protocol"; homepage https://modelcontextprotocol.io; primary language TypeScript; forks 1,889; size 60,566 KB; created 2024-09-24T20:26:52Z; pushed 2026-10-31T15:43:36Z; updated 2026-11-01T19:54:43Z; topics: docs, mcp, specification, standard; not archived; not disabled.

### 2.2 github/github

- **Full name:** `github/github`
- **Status: NOT AVAILABLE.** The GitHub API returned **404 Not Found** for this repository across multiple calls:
  - `GET https://api.github.com/repos/github/github/branches?page=1&per_page=30` → 404 Not Found
  - `GET https://api.github.com/repos/github/github/commits?page=1&per_page=1&sha=main` → 404 Not Found
  - `GET https://api.github.com/repos/github/github/commits?page=1&per_page=1&sha=master` → 404 Not Found
  - `GET https://api.github.com/repos/github/github/contents/README.md` → 404 Not Found
- **Stars, open issues, default branch, and latest commit date/SHA: could not be verified** because the repository `github/github` does not exist (or is not accessible) at the time of this run.
- **Closest verifiable repository under the `github` organization** (from a GitHub repository search, `user:github`): `github/docs`
  - **Full name:** `github/docs`
  - **Stars:** 21,197 (`stargazers_count: 21197`)
  - **Open issues:** 63 (`open_issues_count: 63`; `open_issues` also returned 63)
  - **Default branch:** `main`
  - **Latest commit on default branch (`main`):**
    - **SHA:** `33b1f4a6fec2d9b6fd3d374afa56bcd9f0875b57`
    - **Commit author date:** 2026-10-31T07:47:08Z
    - **Author:** Awais Ur Rehman (GitHub login: awais-ur-rehman; email 75811924+awais-ur-rehman@users.noreply.github.com; committed via web-flow)
    - **Commit message:** "docs(dependabot): correct security update scope (#46758)"
  - This is reported for reference only; it is NOT `github/github`.

### 2.3 GitHub Actions workflow files in modelcontextprotocol/servers (.github/workflows/)

The directory `modelcontextprotocol/servers/.github/workflows/` **does exist** and contains the following workflow files (fetched at ref `194cc86e3ae6400958555bd4116849d822d69263`):

1. `claude.yml`
2. `dco.yml`
3. `dependabot-alerts.yml`
4. `dependency-refresh.yml`
5. `everything-mcp-diff.yml`
6. `main-source.yml`
7. `prepare-python-release.yml`
8. `python.yml`
9. `release.yml`
10. `sdk-watch.yml`
11. `typescript.yml`
12. `version-packages.yml`

Note: the directory listing returned by the API was truncated after `version-packages.yml`; additional files may exist beyond what was returned. The 12 filenames above are exactly those observed in the tool result.

---

## 3. Procurement Section

### 3.1 Amazon search: "Model Context Protocol"

**Status: NOT VERIFIABLE.** The Amazon search scraper call returned HTTP 429:

```
{"message":"Your current plan's quota has been reached. Upgrade your plan to continue scraping.","instance":"/v1/queries","timestamp":"2026-11-01T22:04:01.721798182Z","trace_id":"6ae7b751-9a8ec6aa092f57679bbb1646"}
```

A second Amazon search for a related developer query also returned HTTP 429:

```
{"message":"Your current plan's quota has been reached. Upgrade your plan to continue scraping.","instance":"/v1/queries","timestamp":"2026-11-01T22:04:01.949140027Z","trace_id":"6ae7b751-20e85f3b4aea7d3cacf20cda"}
```

No product title, author, price, or rating could be captured. This section is therefore left empty rather than filled from memory.

### 3.2 Amazon search: "Designing Data-Intensive Applications" (developer gear query)

**Status: NOT VERIFIABLE.** Same HTTP 429 quota-exceeded response as above; no top-result fields (title, author, price, rating) are recoverable from this run.

---

## 4. Summary of Verified vs. Unverified Data

| Item | Verifiable? | Source |
|---|---|---|
| modelcontextprotocol/modelcontextprotocol stars (9,584) | Yes | GitHub repo search API |
| modelcontextprotocol/modelcontextprotocol open issues (119) | Yes | GitHub repo search API |
| modelcontextprotocol/modelcontextprotocol default branch (main) | Yes | GitHub repo search API |
| modelcontextprotocol/modelcontextprotocol latest commit SHA/date/author | Yes | GitHub commits API (sha=main, perPage=1) |
| github/docs stars (21,197), open issues (63), default branch (main) | Yes | GitHub repo search API (user:github) |
| github/docs latest commit SHA/date/author | Yes | GitHub commits API (sha=main, perPage=1) |
| modelcontextprotocol/servers/.github/workflows/ file list (12 files) | Yes (partial) | GitHub contents API (truncated listing) |
| github/github existence | No — 404 Not Found | GitHub API branches/commits/contents |
| Google search results | No — HTTP 429 | Oxylabs Google search scraper |
| Amazon "Model Context Protocol" results | No — HTTP 429 | Oxylabs Amazon search scraper |
| Amazon "Designing Data-Intensive Applications" results | No — HTTP 429 | Oxylabs Amazon search scraper |

---

*Generated for internal adoption report appendix. Authenticated GitHub user: HeziLiu.*
*File stored at: https://github.com/mcpmark-eval-liuhezi/mcp-adoption-reference/blob/main/mcp-adoption-reference.md*
