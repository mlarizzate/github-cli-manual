# `gh discussion list`

> List discussions in a GitHub repository. By default, only open discussions

## Description

are shown.

For more information about output formatting flags, see `gh help formatting`.

## Synopsis

```bash
gh discussion list [flags]
```

## Aliases

- `gh discussion ls`

## Flags

```text
--after string             Cursor for the next page of results
      --answered                 Filter by answered state
  -A, --author string            Filter by author
  -c, --category string          Filter by category name or slug
  -q, --jq expression            Filter JSON output using a jq expression
      --json fields              Output JSON with the specified fields
  -l, --label strings            Filter by label
  -L, --limit int                Maximum number of discussions to fetch (default 30)
      --order string             Order of results: {asc|desc} (default "desc")
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
  -S, --search query             Search discussions with query
      --sort string              Sort by field: {created|updated} (default "updated")
  -s, --state string             Filter by state: {open|closed|all} (default "open")
  -t, --template string          Format JSON output using a Go template; see "gh help formatting"
  -w, --web                      List discussions in the web browser
```

## Inherited Flags

```text
--help   Show help for command

JSON FIELDS
  answerChosenAt, answerChosenBy, answered, author, body, category, closed,
  closedAt, createdAt, id, labels, locked, number, stateReason, title, updatedAt,
  url
```

## Examples

```bash
# List open discussions
  $ gh discussion list
  
  # List discussions with a specific category
  $ gh discussion list --category General
  
  # List closed discussions by author
  $ gh discussion list --state closed --author monalisa
  
  # List all discussions (closed or open) by label
  $ gh discussion list --state all --label bug,enhancement
  
  # List answered Q&A discussions as JSON
  $ gh discussion list --answered --json number,title,url
  
  # List unanswered Q&A discussions as JSON
  $ gh discussion list --answered=false --json number,title,url
```

## AI Agent Automation Tips

- **Machine-Readable Output**: Use `--json <fields>` and `--jq '<filter>'` for deterministic, parseable JSON output rather than text scraping.
- **Explicit Parameters**: In automation pipelines, explicitly pass flags like `--title`, `--body`, or `--body-file -` to bypass editor popups.
- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh discussion`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
