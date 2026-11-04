# `gh release view`

> View information about a GitHub Release.

## Description

Without an explicit tag name argument, the latest release in the project
is shown.

For more information about output formatting flags, see `gh help formatting`.

## Synopsis

```bash
gh release view [<tag>] [flags]
```

## Flags

```text
-q, --jq expression     Filter JSON output using a jq expression
      --json fields       Output JSON with the specified fields
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
  -w, --web               Open the release in the browser
```

## Inherited Flags

```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format

JSON FIELDS
  apiUrl, assets, author, body, createdAt, databaseId, id, isDraft, isImmutable,
  isPrerelease, name, publishedAt, tagName, tarballUrl, targetCommitish,
  uploadUrl, url, zipballUrl
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
