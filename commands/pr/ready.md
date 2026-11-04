# `gh pr ready`

> Mark a pull request as ready for review.

## Description

Without an argument, the pull request that belongs to the current branch
is marked as ready.

If supported by your plan, convert to draft with `--undo`

## Synopsis

```bash
gh pr ready [<number> | <url> | <branch>] [flags]
```

## Flags

```text
--undo   Convert a pull request to "draft"
```

## Inherited Flags

```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh pr`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
