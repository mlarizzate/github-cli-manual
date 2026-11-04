# `gh gpg-key delete`

> Delete a GPG key from your GitHub account

## Synopsis

```bash
gh gpg-key delete <key-id> [flags]
```

## Flags

```text
-y, --yes   Skip the confirmation prompt
```

## Inherited Flags

```text
--help   Show help for command
```

## AI Agent Automation Tips

- **Non-Interactive Execution**: Always pass affirmative flags (e.g., `--yes` or `--confirm`) to prevent hanging in interactive prompts.
- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh gpg-key`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
