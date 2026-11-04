# `gh gist`

> Work with GitHub gists.

## Synopsis

```bash
gh gist <command> [flags]

AVAILABLE COMMANDS
  clone:         Clone a gist locally
  create:        Create a new gist
  delete:        Delete a gist
  edit:          Edit one of your gists
  list:          List your gists
  rename:        Rename a file in a gist
  view:          View a gist
```

## Subcommands

| Command | Description |
| :--- | :--- |
| [`gh gist clone`](./clone.md) | Clone a gist locally |
| [`gh gist create`](./create.md) | Create a new gist |
| [`gh gist delete`](./delete.md) | Delete a gist |
| [`gh gist edit`](./edit.md) | Edit one of your gists |
| [`gh gist list`](./list.md) | List your gists |
| [`gh gist rename`](./rename.md) | Rename a file in a gist |
| [`gh gist view`](./view.md) | View a gist |

## Inherited Flags

```text
--help   Show help for command
```

## Arguments

```text
A gist can be supplied as argument in either of the following formats:
  - by ID, e.g. 5b0e0062eb8e9654adad7bb1d81cc75f
  - by URL, e.g. "https://gist.github.com/OWNER/5b0e0062eb8e9654adad7bb1d81cc75f"
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
