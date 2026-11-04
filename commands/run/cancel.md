# `gh run cancel`

> Cancel a workflow run

## Synopsis

```bash
gh run cancel [<run-id>] [flags]
```

## Flags

```text
--force   Force cancel a workflow run
```

## Inherited Flags

```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

## AI Agent Automation Tips

- **Non-Interactive Execution**: Always pass affirmative flags (e.g., `--yes` or `--confirm`) to prevent hanging in interactive prompts.
- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh run`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
