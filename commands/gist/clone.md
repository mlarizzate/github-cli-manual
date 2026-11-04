# `gh gist clone`

> Clone a GitHub gist locally.

## Description

A gist can be supplied as argument in either of the following formats:
- by ID, e.g. `5b0e0062eb8e9654adad7bb1d81cc75f`
- by URL, e.g. `https://gist.github.com/OWNER/5b0e0062eb8e9654adad7bb1d81cc75f`

Pass additional `git clone` flags by listing them after `--`.

## Synopsis

```bash
gh gist clone <gist> [<directory>] [-- <gitflags>...]
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
- [`gh gist`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
