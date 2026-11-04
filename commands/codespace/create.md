# `gh codespace create`

> Create a codespace

## Synopsis

```bash
gh codespace create [flags]
```

## Flags

```text
-b, --branch string               Repository branch
      --default-permissions         Do not prompt to accept additional permissions requested by the codespace
      --devcontainer-path string    Path to the devcontainer.json file to use when creating codespace
  -d, --display-name string         Display name for the codespace (48 characters or less)
      --idle-timeout duration       Allowed inactivity before codespace is stopped, e.g. "10m", "1h"
  -l, --location string             Location: {EastUs|SouthEastAsia|WestEurope|WestUs2} (determined automatically if not provided)
  -m, --machine string              Hardware specifications for the VM
  -R, --repo string                 Repository name with owner: user/repo
      --retention-period duration   Allowed time after shutting down before the codespace is automatically deleted (maximum 30 days), e.g. "1h", "72h"
  -s, --status                      Show status of post-create command and dotfiles
  -w, --web                         Create codespace from browser, cannot be used with --display-name, --idle-timeout, or --retention-period
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
- [`gh codespace`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
