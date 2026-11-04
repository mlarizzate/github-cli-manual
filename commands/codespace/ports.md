# `gh codespace ports`

> List ports in a codespace

## Description

For more information about output formatting flags, see `gh help formatting`.

## Synopsis

```bash
gh codespace ports [flags]

AVAILABLE COMMANDS
  forward:       Forward ports
  visibility:    Change the visibility of the forwarded port
```

## Subcommands

| Command | Description |
| :--- | :--- |
| [`gh codespace ports forward`](./ports-forward.md) | Forward ports |
| [`gh codespace ports visibility`](./ports-visibility.md) | Change the visibility of the forwarded port |

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
  browseUrl, label, sourcePort, visibility
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
