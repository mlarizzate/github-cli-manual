# `gh issue artifact view`

> Display an issue artifact's name, type, authors, content, and edit history. A

## Description

link shows its URL.

Name the artifact by its issue and number, or by its URL. `<issue>` is an
issue number or URL.

By default, the current version is shown. Use `--version` to show an earlier
version from the edit history.

With `--web`, open a document's page on GitHub, or a link's URL.

For more information about output formatting flags, see `gh help formatting`.

## Synopsis

```bash
gh issue artifact view {<issue> <artifact-number> | <artifact-url>} [flags]
```

## Flags

```text
-q, --jq expression     Filter JSON output using a jq expression
      --json fields       Output JSON with the specified fields
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
      --version number    Show the version with this number from the edit history
  -w, --web               Open a document's page on GitHub, or a link's URL
```

## Inherited Flags

```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format

JSON FIELDS
  body, bodyHtml, createdAt, creator, description, id, name, number, type,
  updatedAt, updatedByActor, url, versions
```

## Examples

```bash
# View artifact 2 on issue 142
  $ gh issue artifact view 142 2
  
  # View an earlier version
  $ gh issue artifact view 142 2 --version 5
  
  # View an artifact by its URL
  $ gh issue artifact view https://github.com/monalisa/monas-cafe/issues/142/artifacts/3
  
  # Open a link artifact in the browser
  $ gh issue artifact view 142 3 --web
  
  # Print an artifact's body
  $ gh issue artifact view 142 2 --json body --jq .body
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
