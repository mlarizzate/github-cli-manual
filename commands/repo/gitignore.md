# `gh repo gitignore`

> List and view available repository gitignore templates

## Synopsis

```bash
gh repo gitignore <command> [flags]

AVAILABLE COMMANDS
  list:          List available repository gitignore templates
  view:          View an available repository gitignore template
```

## Subcommands

| Command | Description |
| :--- | :--- |
| [`gh repo gitignore list`](./gitignore-list.md) | List available repository gitignore templates |
| [`gh repo gitignore view`](./gitignore-view.md) | View an available repository gitignore template |

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
