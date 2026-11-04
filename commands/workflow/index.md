# `gh workflow`

> List, view, and run workflows in GitHub Actions.

## Synopsis

```bash
gh workflow <command> [flags]

AVAILABLE COMMANDS
  disable:       Disable a workflow
  enable:        Enable a workflow
  list:          List workflows
  run:           Run a workflow by creating a workflow_dispatch event
  view:          View the summary of a workflow
```

## Subcommands

| Command | Description |
| :--- | :--- |
| [`gh workflow disable`](./disable.md) | Disable a workflow |
| [`gh workflow enable`](./enable.md) | Enable a workflow |
| [`gh workflow list`](./list.md) | List workflows |
| [`gh workflow run`](./run.md) | Run a workflow by creating a workflow_dispatch event |
| [`gh workflow view`](./view.md) | View the summary of a workflow |

## Flags

```text
-R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
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
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
