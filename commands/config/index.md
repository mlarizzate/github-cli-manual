# `gh config`

> Display or change configuration settings for gh.

## Description

Current respected settings:
- `api_host`: experimental: the hostname to use when making API requests for a GitHub host. Note: this is not a security boundary and requests to the canonical host will remain authenticated
- `git_protocol`: the protocol to use for git clone and push operations `{https | ssh}` (default `https`)
- `editor`: the text editor program to use for authoring text
- `prompt`: toggle interactive prompting in the terminal `{enabled | disabled}` (default `enabled`)
- `prefer_editor_prompt`: toggle preference for editor-based interactive prompting in the terminal `{enabled | disabled}` (default `disabled`)
- `expiring_credentials`: toggle preference for expiring credentials that gh refreshes automatically when logging in `{enabled | disabled}` (default `disabled`)
- `pager`: the terminal pager program to send standard output to
- `http_unix_socket`: the path to a Unix socket through which to make an HTTP connection
- `browser`: the web browser to use for opening URLs
- `clipboard`: whether to copy one-time OAuth device codes to the clipboard `{enabled | disabled}` (default `enabled`)
- `color_labels`: whether to display labels using their RGB hex color codes in terminals that support truecolor `{enabled | disabled}` (default `disabled`)
- `accessible_colors`: whether customizable, 4-bit accessible colors should be used `{enabled | disabled}` (default `disabled`)
- `accessible_prompter`: whether an accessible prompter should be used `{enabled | disabled}` (default `disabled`)
- `spinner`: whether to use an animated spinner as a progress indicator `{enabled | disabled}` (default `enabled`)
- `telemetry`: whether telemetry is enabled, disabled, or logging `{enabled | disabled | log}` (default `enabled`)

## Synopsis

```bash
gh config <command> [flags]

AVAILABLE COMMANDS
  clear-cache:   Clear the cli cache
  get:           Print the value of a given configuration key
  list:          Print a list of configuration keys and values
  set:           Update configuration with a value for the given key
```

## Subcommands

| Command | Description |
| :--- | :--- |
| [`gh config clear-cache`](./clear-cache.md) | Clear the cli cache |
| [`gh config get`](./get.md) | Print the value of a given configuration key |
| [`gh config list`](./list.md) | Print a list of configuration keys and values |
| [`gh config set`](./set.md) | Update configuration with a value for the given key |

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
