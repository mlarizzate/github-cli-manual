# `gh preview`

> Preview commands are for testing, demonstrative, and development purposes only.

## Description

They should be considered unstable and can change at any time.

## Synopsis

```bash
gh preview <command> [flags]

AVAILABLE COMMANDS
  prompter:      Execute a test program to preview the prompter
```

## Subcommands

| Command | Description |
| :--- | :--- |
| [`gh preview prompter`](./prompter.md) | Execute a test program to preview the prompter |

## Inherited Flags

```text
--help   Show help for command
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
