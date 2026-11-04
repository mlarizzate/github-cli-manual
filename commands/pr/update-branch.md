# `gh pr update-branch`

> Update a pull request branch with latest changes of the base branch.

## Description

Without an argument, the pull request that belongs to the current branch is selected.

The default behavior is to update with a merge commit (i.e., merging the base branch
into the PR's branch). To reconcile the changes with rebasing on top of the base
branch, the `--rebase` option should be provided.

## Synopsis

```bash
gh pr update-branch [<number> | <url> | <branch>] [flags]
```

## Flags

```text
--rebase   Update PR branch by rebasing on top of latest base branch
```

## Inherited Flags

```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

## Examples

```bash
$ gh pr update-branch 23
  $ gh pr update-branch 23 --rebase
  $ gh pr update-branch 23 --repo owner/repo
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh pr`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
