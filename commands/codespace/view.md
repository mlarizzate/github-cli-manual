# `gh codespace view`

> View details about a codespace

## Description

For more information about output formatting flags, see `gh help formatting`.

## Synopsis

```bash
gh codespace view [flags]
```

## Flags

```text
-c, --codespace string    Name of the codespace
  -q, --jq expression       Filter JSON output using a jq expression
      --json fields         Output JSON with the specified fields
  -R, --repo string         Filter codespace selection by repository name (user/repo)
      --repo-owner string   Filter codespace selection by repository owner (username or org)
  -t, --template string     Format JSON output using a Go template; see "gh help formatting"
```

## Inherited Flags

```text
--help   Show help for command

JSON FIELDS
  billableOwner, createdAt, devcontainerPath, displayName, environmentId,
  gitStatus, idleTimeoutMinutes, lastUsedAt, location, machineDisplayName,
  machineName, name, owner, prebuild, recentFolders, repository,
  retentionExpiresAt, retentionPeriodDays, state, vscsTarget
```

## Examples

```bash
# Select a codespace from a list of all codespaces you own
  $ gh cs view
  
  # View the details of a specific codespace
  $ gh cs view -c codespace-name-12345
  
  # View the list of all available fields for a codespace
  $ gh cs view --json
  
  # View specific fields for a codespace
  $ gh cs view --json displayName,machineDisplayName,state
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
