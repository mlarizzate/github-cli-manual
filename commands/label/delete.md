# `gh label delete`

> Delete a label from a repository

## Synopsis

```bash
gh label delete <name> [flags]
```

## Flags

```text
--yes   Confirm deletion without prompting
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
- [`gh label`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
