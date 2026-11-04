# `gh agent-task list`

> List agent tasks (preview)

## Description

For more information about output formatting flags, see `gh help formatting`.

## Synopsis

```bash
gh agent-task list [flags]
```

## Flags

```text
-q, --jq expression     Filter JSON output using a jq expression
      --json fields       Output JSON with the specified fields
  -L, --limit int         Maximum number of agent tasks to fetch (default 30)
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
  -w, --web               Open agent tasks in the browser
```

## Inherited Flags

```text
--help   Show help for command

JSON FIELDS
  completedAt, createdAt, id, name, pullRequestNumber, pullRequestState,
  pullRequestTitle, pullRequestUrl, repository, state, updatedAt, user
```

## AI Agent Automation Tips

- **Machine-Readable Output**: Use `--json <fields>` and `--jq '<filter>'` for deterministic, parseable JSON output rather than text scraping.
- **Explicit Parameters**: In automation pipelines, explicitly pass flags like `--title`, `--body`, or `--body-file -` to bypass editor popups.
- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh agent-task`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
