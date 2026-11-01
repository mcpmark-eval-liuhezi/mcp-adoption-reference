# MCP Adoption Reference

Internal reference: Model Context Protocol adoption notes.

## 1. Web Research: Google Search for "Model Context Protocol"

A Google search for "Model Context Protocol" was run during this build using the Google Search Scraper tool. Every attempt returned HTTP 429 — "Your current plan's quota has been reached. Upgrade your plan to continue scraping." — in both parsed and raw/markdown output modes, including retries. As fallbacks, the Universal Scraper was used on Google, Bing, and DuckDuckGo search URLs; all three also returned HTTP 429 quota-exhausted errors.

Result: no search results were returned — no page titles, URLs, or AI-overview fragments were provided by the search tooling in this run. Therefore, this section cannot cite any search results or overview text verbatim, because the search gave back nothing usable. The web research section is effectively empty pending quota reset or an alternative search source.

## 2. Ecosystem

### modelcontextprotocol/modelcontextprotocol
- Full name (owner/repo): modelcontextprotocol/modelcontextprotocol
- Stars: 9584 (GitHub API stargazers_count at time of fetch)
- Open issues: 119 (GitHub API open_issues_count at time of fetch)
- Default branch: main
- Latest commit on default branch (main):
  - SHA: 194cc86e3ae6400955bd4116849d822d69263
  - Author date: 2026-10-28T20:43:56Z
  - Author: Cliff Hall (cliffhall)
  - Commit message: "Merge pull request #5342 from modelcontextprotocol/v2/chore/5330-release-v2.2.0\n\nRelease v2.2.0: merge v2/main into main (certifi lock)"
- GitHub Actions workflow files in modelcontextprotocol/servers (.github/workflows/): claude.yml, dco.yml, dependabot-alerts.yml, dependency-refresh.yml, everything-mcp-diff.yml, main-source.yml, prepare-python-release.yml, python.yml, release.yml, sdk-watch.yml, typescript.yml, version-packages.yml

  Note: the directory listing API response was truncated after the version-packages.yml entry, so the 12 filenames above are all that were returned before truncation.

### github/github
- Full name (owner/repo): could not be verified.
- Stars, open issues, default branch, and latest commit on default branch: not available. All GitHub API calls for this repository returned 404 Not Found (commits with sha=main, HEAD, and master; branches list; git tree at main; workflows; releases/latest; releases list; tags list) and repository/issue search with repo:github/github returned 422 "The listed users and repositories cannot be searched either because the resources do not exist or you do not have permission to view them." No star count, issue count, default branch, or commit date/SHA could be retrieved for github/github during this run.

## 3. Procurement

### Amazon search: "Model Context Protocol"
- Top result title, author, price, and rating: not available. The Amazon Search Scraper returned HTTP 429 — "Your current plan's quota has been reached. Upgrade your plan to continue scraping." — for this query, and the Amazon Product Scraper (queried with "Model Context Protocol") also returned HTTP 429. No product data was returned, so no title/author/price/rating can be reported for this query.

### Amazon search: "Python programming" (second query, chosen as a developer gear/procurement example)
- Top result title, author, price, and rating: not available for the same reason — HTTP 429 quota-exhausted on all Amazon scraping attempts in this run. No fields can be reported.

## Notes on Verifiability

- All numbers for modelcontextprotocol/modelcontextprotocol are traceable to the GitHub repository search API response received during this run (stargazers_count 9584, open_issues_count 119, default_branch main, latest commit SHA 194cc86e3ae6400955bd4116849d822d69263, author date 2026-10-28T20:43:56Z).
- The .github/workflows/ listing for modelcontextprotocol/servers returned 12 workflow filenames before the API response was truncated; the list above reflects exactly those returned.
- github/github could not be verified: every GitHub API endpoint attempted returned 404 or 422.
- Google web search and both Amazon procurement searches could not be executed: the scraping plan's quota was exhausted (HTTP 429) for the entire run, so those sections contain no tool-sourced data and no verbatim AI-overview fragments exist to quote.
