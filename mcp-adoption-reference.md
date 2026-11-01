# MCP Adoption Reference

Internal reference: Model Context Protocol adoption notes.

## 1. Web Research: Google Search for "Model Context Protocol"

A Google search for "Model Context Protocol" was run via the Oxylabs Google Search Scraper during this run. The call returned HTTP 429 (quota exceeded):

"Your current plan's quota has been reached. Upgrade your plan to continue scraping."

The error was non-retryable, and no search results (page titles, URLs, or AI-overview text) were returned. As a fallback, a universal web scrape of https://www.google.com/search?q=Model+Context+Protocol and of Amazon search URLs was also attempted; both also returned HTTP 429 quota-exceeded errors. As a result, no verbatim search results or AI-overview fragments can be reported from live sources in this run. Any AI-overview text that may have appeared could not be captured or quoted.

## 2. Ecosystem

### modelcontextprotocol/modelcontextprotocol
- Full name: modelcontextprotocol/modelcontextprotocol
- Stars: 9584 (stargazers_count as reported by the GitHub API at fetch time)
- Open issues: 119 (open_issues_count as reported by the GitHub API at fetch time)
- Default branch: main
- Latest commit on default branch (main):
  - SHA: 194cc86e3ae6400958555bd4116849d822d69263
  - Author date: 2026-10-28T20:43:56Z
  - Author: Cliff Hall (cliffhall)
  - Commit message: Merge pull request #5342 from modelcontextprotocol/v2/chore/5330-release-v2.2.0
  - URL: https://github.com/modelcontextprotocol/servers/commit/194cc86e3ae6400958555bd4116849d822d69263

### github/docs (GitHub organization's primary repository; github/github does not exist)
The repository `github/github` was requested but returned HTTP 404 Not Found:

"main: GET https://api.github.com/repos/github/github/commits?page=1&per_page=1&sha=main: 404 Not Found []"

The canonical repository under the `github` organization is `github/docs`, whose details are reported below.
- Full name: github/docs
- Stars: 21197 (stargazers_count as reported by the GitHub API at fetch time)
- Open issues: 63 (open_issues_count as reported by the GitHub API at fetch time)
- Default branch: main
- Latest commit on default branch (main):
  - SHA: 33b1f4a6fec2d9b6fd3d374afa56bcd9f0875b57
  - Author date: 2026-10-31T07:47:08Z
  - Author: Awais Ur Rehman (awais-ur-rehman)
  - Commit message: docs(dependabot): correct security update scope (#46758)
  - URL: https://github.com/github/docs/commit/33b1f4a6fec2d9b6fd3d374afa56bcd9f0875b57

### GitHub Actions workflow files in modelcontextprotocol/servers (.github/workflows/)
Files confirmed present in the directory via the GitHub contents API (the API response was truncated after this entry, so additional files may exist beyond those listed):
- claude.yml
- dco.yml
- dependabot-alerts.yml
- dependency-refresh.yml
- everything-mcp-diff.yml
- main-source.yml
- prepare-python-release.yml
- python.yml
- release.yml
- sdk-watch.yml
- typescript.yml
- version-packages.yml

## 3. Procurement (Amazon)

### Query: "Model Context Protocol"
Amazon search for "Model Context Protocol" was attempted via the Oxylabs Amazon Search Scraper. The call returned HTTP 429 (quota exceeded):

"Your current plan's quota has been reached. Upgrade your plan to continue scraping."

The error was non-retryable, and no search results (title, author, price, rating) were returned. A fallback universal scrape of an Amazon search URL also returned HTTP 429. Therefore, no book data can be reported from live sources in this run.

### Query: "Python programming"
Amazon search for "Python programming" was attempted via the Oxylabs Amazon Search Scraper. The call returned HTTP 429 (quota exceeded):

"Your current plan's quota has been reached. Upgrade your plan to continue scraping."

The error was non-retryable, and no search results (title, author, price, rating) were returned. A fallback universal scrape of an Amazon search URL also returned HTTP 429. Therefore, no book data can be reported from live sources in this run.

## Notes on Verifiability

- All GitHub API figures (stars, open issues, default branch, latest commit SHA and author date) are traceable to tool results received during this run.
- The Web Research (Google search) and Procurement (Amazon search) sections could not be populated because the scraping endpoints returned HTTP 429 quota-exceeded errors; no results were returned to quote or report.
- The workflow directory listing for modelcontextprotocol/servers was truncated by the API response, so the 12 filenames above are confirmed present but may not be exhaustive.
