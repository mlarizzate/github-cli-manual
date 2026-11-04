# `gh org`

> Work with GitHub organizations.

## Synopsis

```bash
gh org <command> [flags]

GENERAL COMMANDS
  list:          List organizations for the authenticated user.
```

## Subcommands

| Command | Description |
| :--- | :--- |
| [`gh org list`](./list.md) | List organizations for the authenticated user. |

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
$ gh org list
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
