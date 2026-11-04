# `gh preview prompter`

> Execute a test program to preview the prompter.

## Description

Without an argument, all prompts will be run.

Available prompt types:
- select
- multi-select
- multi-select-with-search
- input
- password
- confirm
- auth-token
- confirm-deletion
- input-hostname
- markdown-editor

## Synopsis

```bash
gh preview prompter [prompt type] [flags]
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
- [`gh preview`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
