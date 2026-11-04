# `gh run watch`

> Watch a run until it completes, showing its progress.

## Description

By default, all steps are displayed. The `--compact` option can be used to only
show the relevant/failed steps.

This command does not support authenticating via fine grained PATs
as it is not currently possible to create a PAT with the `checks:read` permission.

## Synopsis

```bash
gh run watch <run-id> [flags]
```

## Flags

```text
--compact        Show only relevant/failed steps
      --exit-status    Exit with non-zero status if run fails
  -i, --interval int   Refresh interval in seconds (default 3)
```

## Inherited Flags

```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

## Examples

```bash
# Watch a run until it's done
  $ gh run watch
  
  # Watch a run in compact mode
  $ gh run watch --compact
  
  # Run some other command when the run is finished
  $ gh run watch && notify-send 'run is done!'
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh run`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
