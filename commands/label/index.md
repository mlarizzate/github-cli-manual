# `gh label`

> Work with GitHub labels.

## Synopsis

```bash
gh label <command> [flags]

AVAILABLE COMMANDS
  clone:         Clones labels from one repository to another
  create:        Create a new label
  delete:        Delete a label from a repository
  edit:          Edit a label
  list:          List labels in a repository
```

## Subcommands

| Command | Description |
| :--- | :--- |
| [`gh label clone`](./clone.md) | Clones labels from one repository to another |
| [`gh label create`](./create.md) | Create a new label |
| [`gh label delete`](./delete.md) | Delete a label from a repository |
| [`gh label edit`](./edit.md) | Edit a label |
| [`gh label list`](./list.md) | List labels in a repository |

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
