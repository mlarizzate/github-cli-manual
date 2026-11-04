# `gh issue`

> Work with GitHub issues.

## Synopsis

```bash
gh issue <command> [flags]

GENERAL COMMANDS
  create:        Create a new issue
  list:          List issues in a repository
  status:        Show status of relevant issues

TARGETED COMMANDS
  artifact:      Work with issue artifacts (preview)
  close:         Close issue
  comment:       Add a comment to an issue
  delete:        Delete issue
  develop:       Manage linked branches for an issue
  edit:          Edit issues
  lock:          Lock issue conversation
  pin:           Pin an issue
  reopen:        Reopen issue
  transfer:      Transfer issue to another repository
  unlock:        Unlock issue conversation
  unpin:         Unpin an issue
  view:          View an issue
```

## Subcommands

| Command | Description |
| :--- | :--- |
| [`gh issue create`](./create.md) | Create a new issue |
| [`gh issue list`](./list.md) | List issues in a repository |
| [`gh issue status`](./status.md) | Show status of relevant issues |
| [`gh issue artifact`](./artifact.md) | Work with issue artifacts (preview) |
| [`gh issue close`](./close.md) | Close issue |
| [`gh issue comment`](./comment.md) | Add a comment to an issue |
| [`gh issue delete`](./delete.md) | Delete issue |
| [`gh issue develop`](./develop.md) | Manage linked branches for an issue |
| [`gh issue edit`](./edit.md) | Edit issues |
| [`gh issue lock`](./lock.md) | Lock issue conversation |
| [`gh issue pin`](./pin.md) | Pin an issue |
| [`gh issue reopen`](./reopen.md) | Reopen issue |
| [`gh issue transfer`](./transfer.md) | Transfer issue to another repository |
| [`gh issue unlock`](./unlock.md) | Unlock issue conversation |
| [`gh issue unpin`](./unpin.md) | Unpin an issue |
| [`gh issue view`](./view.md) | View an issue |

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
An issue can be supplied as argument in any of the following formats:
  - by number, e.g. "123"; or
  - by URL, e.g. "https://github.com/OWNER/REPO/issues/123".
```

## Examples

```bash
$ gh issue list
  $ gh issue create --label bug
  $ gh issue view 123 --web
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
