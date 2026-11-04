# `gh gpg-key`

> Manage GPG keys registered with your GitHub account.

## Synopsis

```bash
gh gpg-key <command> [flags]

AVAILABLE COMMANDS
  add:           Add a GPG key to your GitHub account
  delete:        Delete a GPG key from your GitHub account
  list:          Lists GPG keys in your GitHub account
```

## Subcommands

| Command | Description |
| :--- | :--- |
| [`gh gpg-key add`](./add.md) | Add a GPG key to your GitHub account |
| [`gh gpg-key delete`](./delete.md) | Delete a GPG key from your GitHub account |
| [`gh gpg-key list`](./list.md) | Lists GPG keys in your GitHub account |

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
