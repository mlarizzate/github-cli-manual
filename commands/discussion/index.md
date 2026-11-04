# `gh discussion`

> Working with discussions in the GitHub CLI is in preview and subject to change without notice.

## Synopsis

```bash
gh discussion <command> [flags]

GENERAL COMMANDS
  create:        Create a new discussion (preview)
  list:          List discussions in a repository (preview)

TARGETED COMMANDS
  comment:       Add, edit, or delete a comment or a reply on a discussion (preview)
  edit:          Edit a discussion (preview)
  view:          View a discussion (preview)
```

## Subcommands

| Command | Description |
| :--- | :--- |
| [`gh discussion create`](./create.md) | Create a new discussion (preview) |
| [`gh discussion list`](./list.md) | List discussions in a repository (preview) |
| [`gh discussion comment`](./comment.md) | Add, edit, or delete a comment or a reply on a discussion (preview) |
| [`gh discussion edit`](./edit.md) | Edit a discussion (preview) |
| [`gh discussion view`](./view.md) | View a discussion (preview) |

## Flags

```text
-R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

## Inherited Flags

```text
--help   Show help for command
```

## Arguments

```text
A discussion can be supplied as argument in any of the following formats:
  - by number, e.g. "123"; or
  - by URL, e.g. "https://github.com/OWNER/REPO/discussions/123".
```

## Examples

```bash
$ gh discussion list
  $ gh discussion create --category "General" --title "Hello" --body "Hello World!"
  $ gh discussion view 123
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
