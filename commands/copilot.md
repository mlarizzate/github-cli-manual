# `gh copilot`

> Runs the GitHub Copilot CLI.

## Description

Executing the Copilot CLI through `gh` is currently in preview and subject to change.

If already installed, `gh` will execute the Copilot CLI found in your `PATH`.
If the Copilot CLI is not installed, it will be downloaded to /Users/martinlarizzate/.local/share/gh/copilot.

Use `--remove` to remove the downloaded Copilot CLI.

This command is only supported on Windows, Linux, and Darwin, on amd64/x64
or arm64 architectures.

To prevent `gh` from interpreting flags intended for Copilot,
use `--` before Copilot flags and args.

Learn more at https://gh.io/copilot-cli

## Synopsis

```bash
gh copilot [flags] [args]
```

## Flags

```text
--remove   Remove the downloaded Copilot CLI
```

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
# Download and run the Copilot CLI
  $ gh copilot
  
  # Run the Copilot CLI
  $ gh copilot -p "Summarize this week's commits" --allow-tool 'shell(git)'
  
  # Remove the Copilot CLI (if installed through gh)
  $ gh copilot --remove
  
  # Run the Copilot CLI help command
  $ gh copilot -- --help
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
