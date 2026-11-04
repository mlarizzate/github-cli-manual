# `gh issue unpin`

> Unpin an issue from a repository.

## Description

The issue can be specified by issue number or URL.

## Synopsis

```bash
gh issue unpin {<number> | <url>} [flags]
```

## Inherited Flags

```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

## Examples

```bash
# Unpin issue from the current repository
  $ gh issue unpin 23
  
  # Unpin issue by URL
  $ gh issue unpin https://github.com/owner/repo/issues/23
  
  # Unpin an issue from specific repository
  $ gh issue unpin 23 --repo owner/repo
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh issue`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
