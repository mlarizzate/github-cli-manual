# `gh issue develop`

> Manage linked branches for an issue.

## Description

When using the `--base` flag, the new development branch will be created from the specified
remote branch. The new branch will be configured as the base branch for pull requests created using
`gh pr create`.

## Synopsis

```bash
gh issue develop {<number> | <url>} [flags]
```

## Flags

```text
-b, --base string          Name of the remote branch you want to make your new branch from
      --branch-repo string   Name or URL of the repository where you want to create your new branch
  -c, --checkout             Checkout the branch after creating it
  -l, --list                 List linked branches for the issue
  -n, --name string          Name of the branch to create
      --worktree path        Check out the branch into a worktree at the given path
```

## Inherited Flags

```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

## Examples

```bash
# List branches for issue 123
  $ gh issue develop --list 123
  
  # List branches for issue 123 in repo cli/cli
  $ gh issue develop --list --repo cli/cli 123
  
  # Create a branch for issue 123 based on the my-feature branch
  $ gh issue develop 123 --base my-feature
  
  # Create a branch for issue 123 and check it out
  $ gh issue develop 123 --checkout
  
  # Create a branch for issue 123 and check it out in a worktree
  $ gh issue develop 123 --checkout --worktree /path/to/wt-feature
  
  # Create a branch in repo monalisa/cli for issue 123 in repo cli/cli
  $ gh issue develop 123 --repo cli/cli --branch-repo monalisa/cli
```

## AI Agent Automation Tips

- **Explicit Parameters**: In automation pipelines, explicitly pass flags like `--title`, `--body`, or `--body-file -` to bypass editor popups.
- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh issue`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
