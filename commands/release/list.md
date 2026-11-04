# `gh release list`

> List releases in a repository

## Description

For more information about output formatting flags, see `gh help formatting`.

## Synopsis

```bash
gh release list [flags]
```

## Aliases

- `gh release ls`

## Flags

```text
--exclude-drafts         Exclude draft releases
      --exclude-pre-releases   Exclude pre-releases
  -q, --jq expression          Filter JSON output using a jq expression
      --json fields            Output JSON with the specified fields
  -L, --limit int              Maximum number of items to fetch (default 30)
  -O, --order string           Order of releases returned: {asc|desc} (default "desc")
  -t, --template string        Format JSON output using a Go template; see "gh help formatting"
```

## Inherited Flags

```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format

JSON FIELDS
  createdAt, isDraft, isImmutable, isLatest, isPrerelease, name, publishedAt,
  tagName
```

## AI Agent Automation Tips

- **Machine-Readable Output**: Use `--json <fields>` and `--jq '<filter>'` for deterministic, parseable JSON output rather than text scraping.
- **Explicit Parameters**: In automation pipelines, explicitly pass flags like `--title`, `--body`, or `--body-file -` to bypass editor popups.
- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh release`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
