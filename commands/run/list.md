# `gh run list`

> List recent workflow runs.

## Description

Note that providing the `workflow_name` to the `-w` flag will not fetch disabled workflows.
Also pass the `-a` flag to fetch disabled workflow runs using the `workflow_name` and the `-w` flag.

Runs created by organization and enterprise ruleset workflows will not display a workflow name due to GitHub API limitations.

To see runs associated with a pull request, users should run `gh pr checks`.

For more information about output formatting flags, see `gh help formatting`.

## Synopsis

```bash
gh run list [flags]
```

## Aliases

- `gh run ls`

## Flags

```text
-a, --all               Include disabled workflows
  -b, --branch string     Filter runs by branch
  -c, --commit SHA        Filter runs by the SHA of the commit
      --created date      Filter runs by the date it was created
  -e, --event event       Filter runs by which event triggered the run
  -q, --jq expression     Filter JSON output using a jq expression
      --json fields       Output JSON with the specified fields
  -L, --limit int         Maximum number of runs to fetch (default 20)
  -s, --status string     Filter runs by status: {queued|completed|in_progress|requested|waiting|pending|action_required|cancelled|failure|neutral|skipped|stale|startup_failure|success|timed_out}
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
  -u, --user string       Filter runs by user who triggered the run
  -w, --workflow string   Filter runs by workflow
```

## Inherited Flags

```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format

JSON FIELDS
  attempt, conclusion, createdAt, databaseId, displayTitle, event, headBranch,
  headSha, name, number, startedAt, status, updatedAt, url, workflowDatabaseId,
  workflowName
```

## AI Agent Automation Tips

- **Machine-Readable Output**: Use `--json <fields>` and `--jq '<filter>'` for deterministic, parseable JSON output rather than text scraping.
- **Explicit Parameters**: In automation pipelines, explicitly pass flags like `--title`, `--body`, or `--body-file -` to bypass editor popups.
- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh run`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
