# `gh codespace list`

> List codespaces of the authenticated user.

## Description

Alternatively, organization administrators may list all codespaces billed to the organization.

For more information about output formatting flags, see `gh help formatting`.

## Synopsis

```bash
gh codespace list [flags]
```

## Aliases

- `gh codespace ls, gh cs ls`

## Flags

```text
-q, --jq expression     Filter JSON output using a jq expression
      --json fields       Output JSON with the specified fields
  -L, --limit int         Maximum number of codespaces to list (default 30)
  -o, --org login         The login handle of the organization to list codespaces for (admin-only)
  -R, --repo string       Repository name with owner: user/repo
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
  -u, --user username     The username to list codespaces for (used with --org)
  -w, --web               List codespaces in the web browser, cannot be used with --user or --org
```

## Inherited Flags

```text
--help   Show help for command

JSON FIELDS
  createdAt, displayName, gitStatus, lastUsedAt, machineName, name, owner,
  repository, state, vscsTarget
```

## AI Agent Automation Tips

- **Machine-Readable Output**: Use `--json <fields>` and `--jq '<filter>'` for deterministic, parseable JSON output rather than text scraping.
- **Explicit Parameters**: In automation pipelines, explicitly pass flags like `--title`, `--body`, or `--body-file -` to bypass editor popups.
- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh codespace`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
