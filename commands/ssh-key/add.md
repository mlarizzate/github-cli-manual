# `gh ssh-key add`

> Add an SSH key to your GitHub account

## Synopsis

```bash
gh ssh-key add [<key-file>] [flags]
```

## Flags

```text
-t, --title string   Title for the new key
      --type string    Type of the ssh key: {authentication|signing} (default "authentication")
```

## Inherited Flags

```text
--help   Show help for command
```

## AI Agent Automation Tips

- **Explicit Parameters**: In automation pipelines, explicitly pass flags like `--title`, `--body`, or `--body-file -` to bypass editor popups.
- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh ssh-key`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
