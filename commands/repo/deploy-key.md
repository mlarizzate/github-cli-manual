# `gh repo deploy-key`

> Manage deploy keys in a repository

## Synopsis

```bash
gh repo deploy-key <command> [flags]

AVAILABLE COMMANDS
  add:           Add a deploy key to a GitHub repository
  delete:        Delete a deploy key from a GitHub repository
  list:          List deploy keys in a GitHub repository
```

## Subcommands

| Command | Description |
| :--- | :--- |
| [`gh repo deploy-key add`](./deploy-key-add.md) | Add a deploy key to a GitHub repository |
| [`gh repo deploy-key delete`](./deploy-key-delete.md) | Delete a deploy key from a GitHub repository |
| [`gh repo deploy-key list`](./deploy-key-list.md) | List deploy keys in a GitHub repository |

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
- [`gh repo`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
