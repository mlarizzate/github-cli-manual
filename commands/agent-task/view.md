# `gh agent-task view`

> View an agent task session.

## Description

For more information about output formatting flags, see `gh help formatting`.

## Synopsis

```bash
gh agent-task view [<session-id> | <pr-number> | <pr-url> | <pr-branch>] [flags]
```

## Flags

```text
--follow                   Follow agent session logs
  -q, --jq expression            Filter JSON output using a jq expression
      --json fields              Output JSON with the specified fields
      --log                      Show agent session logs
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
  -t, --template string          Format JSON output using a Go template; see "gh help formatting"
  -w, --web                      Open agent task in the browser
```

## Inherited Flags

```text
--help   Show help for command

JSON FIELDS
  completedAt, createdAt, id, name, pullRequestNumber, pullRequestState,
  pullRequestTitle, pullRequestUrl, repository, state, updatedAt, user
```

## Examples

```bash
# View an agent task by session ID
  $ gh agent-task view e2fa49d2-f164-4a56-ab99-498090b8fcdf
  
  # View an agent task by pull request number in current repo
  $ gh agent-task view 12345
  
  # View an agent task by pull request number
  $ gh agent-task view --repo OWNER/REPO 12345
  
  # View an agent task by pull request reference
  $ gh agent-task view OWNER/REPO#12345
  
  # View a pull request agents tasks in the browser
  $ gh agent-task view 12345 --web
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
