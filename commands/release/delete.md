# `gh release delete`

> Delete a release

## Synopsis

```bash
gh release delete <tag> [flags]
```

## Flags

```text
--cleanup-tag   Delete the specified tag in addition to its release
  -y, --yes           Skip the confirmation prompt
```

## Inherited Flags

```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

## AI Agent Automation Tips

- **Non-Interactive Execution**: Always pass affirmative flags (e.g., `--yes` or `--confirm`) to prevent hanging in interactive prompts.
- **Explicit Parameters**: In automation pipelines, explicitly pass flags like `--title`, `--body`, or `--body-file -` to bypass editor popups.
- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh release`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
