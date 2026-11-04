# `gh issue artifact list`

> List the artifacts on an issue, in number order. Every artifact is listed

## Description

unless you set `--limit`.

For more information about output formatting flags, see `gh help formatting`.

## Synopsis

```bash
gh issue artifact list {<issue-number> | <issue-url>} [flags]
```

## Aliases

- `gh issue artifact ls`

## Flags

```text
-q, --jq expression     Filter JSON output using a jq expression
      --json fields       Output JSON with the specified fields
  -L, --limit int         Maximum number of artifacts to fetch
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
      --type string       Filter by type: {generic|plan|link|embedded_html}
```

## Inherited Flags

```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format

JSON FIELDS
  body, bodyHtml, createdAt, creator, description, id, name, number, type,
  updatedAt, updatedByActor, url
```

## Examples

```bash
# List the artifacts on issue 142
  $ gh issue artifact list 142
  
  # List only links
  $ gh issue artifact list 142 --type link
  
  # Print artifact numbers and names as JSON
  $ gh issue artifact list 142 --json number,name
```

## AI Agent Automation Tips

- **Machine-Readable Output**: Use `--json <fields>` and `--jq '<filter>'` for deterministic, parseable JSON output rather than text scraping.
- **Explicit Parameters**: In automation pipelines, explicitly pass flags like `--title`, `--body`, or `--body-file -` to bypass editor popups.
- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh issue`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
