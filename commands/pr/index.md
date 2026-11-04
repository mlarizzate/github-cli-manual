# `gh pr`

> Work with GitHub pull requests.

## Synopsis

```bash
gh pr <command> [flags]

GENERAL COMMANDS
  create:        Create a pull request
  list:          List pull requests in a repository
  status:        Show status of relevant pull requests

TARGETED COMMANDS
  checkout:      Check out a pull request in git
  checks:        Show CI status for a single pull request
  close:         Close a pull request
  comment:       Add a comment to a pull request
  diff:          View changes in a pull request
  edit:          Edit a pull request
  lock:          Lock pull request conversation
  merge:         Merge a pull request
  ready:         Mark a pull request as ready for review
  reopen:        Reopen a pull request
  revert:        Revert a pull request
  review:        Add a review to a pull request
  unlock:        Unlock pull request conversation
  update-branch: Update a pull request branch
  view:          View a pull request
```

## Subcommands

| Command | Description |
| :--- | :--- |
| [`gh pr create`](./create.md) | Create a pull request |
| [`gh pr list`](./list.md) | List pull requests in a repository |
| [`gh pr status`](./status.md) | Show status of relevant pull requests |
| [`gh pr checkout`](./checkout.md) | Check out a pull request in git |
| [`gh pr checks`](./checks.md) | Show CI status for a single pull request |
| [`gh pr close`](./close.md) | Close a pull request |
| [`gh pr comment`](./comment.md) | Add a comment to a pull request |
| [`gh pr diff`](./diff.md) | View changes in a pull request |
| [`gh pr edit`](./edit.md) | Edit a pull request |
| [`gh pr lock`](./lock.md) | Lock pull request conversation |
| [`gh pr merge`](./merge.md) | Merge a pull request |
| [`gh pr ready`](./ready.md) | Mark a pull request as ready for review |
| [`gh pr reopen`](./reopen.md) | Reopen a pull request |
| [`gh pr revert`](./revert.md) | Revert a pull request |
| [`gh pr review`](./review.md) | Add a review to a pull request |
| [`gh pr unlock`](./unlock.md) | Unlock pull request conversation |
| [`gh pr update-branch`](./update-branch.md) | Update a pull request branch |
| [`gh pr view`](./view.md) | View a pull request |

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
A pull request can be supplied as argument in any of the following formats:
  - by number, e.g. "123";
  - by URL, e.g. "https://github.com/OWNER/REPO/pull/123"; or
  - by the name of its head branch, e.g. "patch-1" or "OWNER:patch-1".
```

## Examples

```bash
$ gh pr checkout 353
  $ gh pr create --fill
  $ gh pr view --web
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
