# `gh label list`

> Display labels in a GitHub repository.

## Description

When using the `--search` flag results are sorted by best match of the query.
This behavior cannot be configured with the `--order` or `--sort` flags.

For more information about output formatting flags, see `gh help formatting`.

## Synopsis

```bash
gh label list [flags]
```

## Aliases

- `gh label ls`

## Flags

```text
-q, --jq expression     Filter JSON output using a jq expression
      --json fields       Output JSON with the specified fields
  -L, --limit int         Maximum number of labels to fetch (default 30)
      --order string      Order of labels returned: {asc|desc} (default "asc")
  -S, --search string     Search label names and descriptions
      --sort string       Sort fetched labels: {created|name} (default "created")
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
  -w, --web               List labels in the web browser
```

## Inherited Flags

```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format

JSON FIELDS
  color, createdAt, description, id, isDefault, name, updatedAt, url
```

## Examples

```bash
# Sort labels by name
  $ gh label list --sort name
  
  # Find labels with "bug" in the name or description
  $ gh label list --search bug
```

## AI Agent Automation Tips

- **Machine-Readable Output**: Use `--json <fields>` and `--jq '<filter>'` for deterministic, parseable JSON output rather than text scraping.
- **Explicit Parameters**: In automation pipelines, explicitly pass flags like `--title`, `--body`, or `--body-file -` to bypass editor popups.
- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh label`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
