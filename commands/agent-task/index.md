# `gh agent-task`

> Working with agent tasks in the GitHub CLI is in preview and

## Description

subject to change without notice.

## Synopsis

```bash
gh agent-task <command> [flags]
```

## Aliases

- `gh agent-tasks, gh agent, gh agents`
- `AVAILABLE COMMANDS`
- `create:        Create an agent task (preview)`
- `list:          List agent tasks (preview)`
- `view:          View an agent task session (preview)`

## Subcommands

| Command | Description |
| :--- | :--- |
| [`gh agent-task create`](./create.md) | Create an agent task (preview) |
| [`gh agent-task list`](./list.md) | List agent tasks (preview) |
| [`gh agent-task view`](./view.md) | View an agent task session (preview) |

## Inherited Flags

```text
--help   Show help for command
```

## Arguments

```text
A task can be identified as argument in any of the following formats:
  - by pull request number, e.g. "123"; or
  - by session ID, e.g. "12345abc-12345-12345-12345-12345abc"; or
  - by URL, e.g. "https://github.com/OWNER/REPO/pull/123/agent-sessions/12345abc-12345-12345-12345-12345abc";
  
  Identifying tasks by pull request is not recommended for non-interactive use cases as
  there may be multiple tasks for a given pull request that require disambiguation.
```

## Examples

```bash
# List your most recent agent tasks
  $ gh agent-task list
  
  # Create a new agent task on the current repository
  $ gh agent-task create "Improve the performance of the data processing pipeline"
  
  # View details about agent tasks associated with a pull request
  $ gh agent-task view 123
  
  # View details about a specific agent task
  $ gh agent-task view 12345abc-12345-12345-12345-12345abc
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
