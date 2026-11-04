# `gh ssh-key`

> Manage SSH keys registered with your GitHub account.

## Synopsis

```bash
gh ssh-key <command> [flags]

AVAILABLE COMMANDS
  add:           Add an SSH key to your GitHub account
  delete:        Delete an SSH key from your GitHub account
  list:          Lists SSH keys in your GitHub account
```

## Subcommands

| Command | Description |
| :--- | :--- |
| [`gh ssh-key add`](./add.md) | Add an SSH key to your GitHub account |
| [`gh ssh-key delete`](./delete.md) | Delete an SSH key from your GitHub account |
| [`gh ssh-key list`](./list.md) | Lists SSH keys in your GitHub account |

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
