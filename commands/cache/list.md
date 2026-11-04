# `gh cache list`

> List GitHub Actions caches

## Description

For more information about output formatting flags, see `gh help formatting`.

## Synopsis

```bash
gh cache list [flags]
```

## Aliases

- `gh cache ls`

## Flags

```text
-q, --jq expression     Filter JSON output using a jq expression
      --json fields       Output JSON with the specified fields
  -k, --key string        Filter by cache key prefix
  -L, --limit int         Maximum number of caches to fetch (default 30)
  -O, --order string      Order of caches returned: {asc|desc} (default "desc")
  -r, --ref string        Filter by ref, formatted as refs/heads/<branch name> or refs/pull/<number>/merge
  -S, --sort string       Sort fetched caches: {created_at|last_accessed_at|size_in_bytes} (default "last_accessed_at")
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
```

## Inherited Flags

```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format

JSON FIELDS
  createdAt, id, key, lastAccessedAt, ref, sizeInBytes, version
```

## Examples

```bash
# List caches for current repository
  $ gh cache list
  
  # List caches for specific repository
  $ gh cache list --repo cli/cli
  
  # List caches sorted by least recently accessed
  $ gh cache list --sort last_accessed_at --order asc
  
  # List caches that have keys matching a prefix (or that match exactly)
  $ gh cache list --key key-prefix
  
  # List caches for a specific branch, replace <branch-name> with the actual branch name
  $ gh cache list --ref refs/heads/<branch-name>
  
  # List caches for a specific pull request, replace <pr-number> with the actual pull request number
  $ gh cache list --ref refs/pull/<pr-number>/merge
```

## AI Agent Automation Tips

- **Machine-Readable Output**: Use `--json <fields>` and `--jq '<filter>'` for deterministic, parseable JSON output rather than text scraping.
- **Explicit Parameters**: In automation pipelines, explicitly pass flags like `--title`, `--body`, or `--body-file -` to bypass editor popups.
- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh cache`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
