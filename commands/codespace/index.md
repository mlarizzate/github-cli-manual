# `gh codespace`

> Connect to and manage codespaces

## Synopsis

```bash
gh codespace [flags]
```

## Aliases

- `gh cs`
- `AVAILABLE COMMANDS`
- `code:          Open a codespace in Visual Studio Code`
- `cp:            Copy files between local and remote file systems`
- `create:        Create a codespace`
- `delete:        Delete codespaces`
- `edit:          Edit a codespace`
- `jupyter:       Open a codespace in JupyterLab`
- `list:          List codespaces`
- `logs:          Access codespace logs`
- `ports:         List ports in a codespace`
- `rebuild:       Rebuild a codespace`
- `ssh:           SSH into a codespace`
- `stop:          Stop a running codespace`
- `view:          View details about a codespace`

## Subcommands

| Command | Description |
| :--- | :--- |
| [`gh codespace code`](./code.md) | Open a codespace in Visual Studio Code |
| [`gh codespace cp`](./cp.md) | Copy files between local and remote file systems |
| [`gh codespace create`](./create.md) | Create a codespace |
| [`gh codespace delete`](./delete.md) | Delete codespaces |
| [`gh codespace edit`](./edit.md) | Edit a codespace |
| [`gh codespace jupyter`](./jupyter.md) | Open a codespace in JupyterLab |
| [`gh codespace list`](./list.md) | List codespaces |
| [`gh codespace logs`](./logs.md) | Access codespace logs |
| [`gh codespace ports`](./ports.md) | List ports in a codespace |
| [`gh codespace rebuild`](./rebuild.md) | Rebuild a codespace |
| [`gh codespace ssh`](./ssh.md) | SSH into a codespace |
| [`gh codespace stop`](./stop.md) | Stop a running codespace |
| [`gh codespace view`](./view.md) | View details about a codespace |

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
