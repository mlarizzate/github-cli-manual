# `gh extension upgrade`

> Upgrade installed extensions

## Synopsis

```bash
gh extension upgrade {<name> | --all} [flags]
```

## Flags

```text
--all       Upgrade all extensions
  --dry-run   Only display upgrades
  --force     Force upgrade extension
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
- [`gh extension`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
