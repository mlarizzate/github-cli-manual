# `gh issue status`

> Show status of relevant issues

## Description

For more information about output formatting flags, see `gh help formatting`.

## Synopsis

```bash
gh issue status [flags]
```

## Flags

```text
-q, --jq expression     Filter JSON output using a jq expression
      --json fields       Output JSON with the specified fields
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
```

## Inherited Flags

```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format

JSON FIELDS
  assignees, author, blockedBy, blocking, body, closed, closedAt,
  closedByPullRequestsReferences, comments, createdAt, id, isPinned, issueType,
  labels, milestone, number, parent, projectCards, projectItems, reactionGroups,
  state, stateReason, subIssues, subIssuesSummary, title, updatedAt, url
```

## AI Agent Automation Tips

- **Machine-Readable Output**: Use `--json <fields>` and `--jq '<filter>'` for deterministic, parseable JSON output rather than text scraping.
- **Explicit Parameters**: In automation pipelines, explicitly pass flags like `--title`, `--body`, or `--body-file -` to bypass editor popups.
- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh issue`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
