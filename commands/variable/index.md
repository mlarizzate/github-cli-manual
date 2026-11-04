# `gh variable`

> Variables can be set at the repository, environment or organization level for use in

## Description

GitHub Actions or Dependabot. Run `gh help variable set` to learn how to get started.

## Synopsis

```bash
gh variable <command> [flags]

AVAILABLE COMMANDS
  delete:        Delete variables
  get:           Get variables
  list:          List variables
  set:           Create or update variables
```

## Subcommands

| Command | Description |
| :--- | :--- |
| [`gh variable delete`](./delete.md) | Delete variables |
| [`gh variable get`](./get.md) | Get variables |
| [`gh variable list`](./list.md) | List variables |
| [`gh variable set`](./set.md) | Create or update variables |

## Flags

```text
-R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

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
