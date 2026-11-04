# `gh pr review`

> Add a review to a pull request.

## Description

Without an argument, the pull request that belongs to the current branch is reviewed.

## Synopsis

```bash
gh pr review [<number> | <url> | <branch>] [flags]
```

## Flags

```text
-a, --approve           Approve pull request
  -b, --body string       Specify the body of a review
  -F, --body-file file    Read body text from file (use "-" to read from standard input)
  -c, --comment           Comment on a pull request
  -r, --request-changes   Request changes on a pull request
```

## Inherited Flags

```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

## Examples

```bash
# Approve the pull request of the current branch
  $ gh pr review --approve
  
  # Leave a review comment for the current branch
  $ gh pr review --comment -b "interesting"
  
  # Add a review for a specific pull request
  $ gh pr review 123
  
  # Request changes on a specific pull request
  $ gh pr review 123 -r -b "needs more ASCII art"
```

## AI Agent Automation Tips

- **Explicit Parameters**: In automation pipelines, explicitly pass flags like `--title`, `--body`, or `--body-file -` to bypass editor popups.
- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh pr`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
