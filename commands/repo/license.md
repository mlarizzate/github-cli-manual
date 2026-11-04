# `gh repo license`

> Explore repository licenses

## Synopsis

```bash
gh repo license <command> [flags]

AVAILABLE COMMANDS
  list:          List common repository licenses
  view:          View a specific repository license
```

## Subcommands

| Command | Description |
| :--- | :--- |
| [`gh repo license list`](./license-list.md) | List common repository licenses |
| [`gh repo license view`](./license-view.md) | View a specific repository license |

## Inherited Flags

```text
--help   Show help for command
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh repo`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
