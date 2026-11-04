# `gh extension browse`

> This command will take over your terminal and run a fully interactive

## Description

interface for browsing, adding, and removing gh extensions. A terminal
width greater than 100 columns is recommended. Narrow terminals
automatically use a single-column layout.

To learn how to control this interface, press `?` after running to see
the help text.

Press `q` to quit.

Running this command with `--single-column` should make this command
more intelligible for users who rely on assistive technology like screen
readers or high zoom.

For a more traditional way to discover extensions, see:

	gh ext search

along with `gh ext install`, `gh ext remove`, and `gh repo view`.

## Synopsis

```bash
gh extension browse [flags]
```

## Flags

```text
--debug           Log to /tmp/extBrowse-*
  -s, --single-column   Render TUI with only one column of text
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
- [`gh extension`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
