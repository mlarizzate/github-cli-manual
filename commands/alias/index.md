# `gh alias`

> Aliases can be used to make shortcuts for gh commands or to compose multiple commands.

## Description

Run `gh help alias set` to learn more.

## Synopsis

```bash
gh alias <command> [flags]

AVAILABLE COMMANDS
  delete:        Delete set aliases
  import:        Import aliases from a YAML file
  list:          List your aliases
  set:           Create a shortcut for a gh command
```

## Subcommands

| Command | Description |
| :--- | :--- |
| [`gh alias delete`](./delete.md) | Delete set aliases |
| [`gh alias import`](./import.md) | Import aliases from a YAML file |
| [`gh alias list`](./list.md) | List your aliases |
| [`gh alias set`](./set.md) | Create a shortcut for a gh command |

## Inherited Flags

```text
--help   Show help for command
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
