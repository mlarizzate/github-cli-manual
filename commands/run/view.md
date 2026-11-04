# `gh run view`

> View a summary of a workflow run.

## Description

Due to platform limitations, `gh` may not always be able to associate jobs with their
corresponding logs when using the primary method of fetching logs in zip format.

In such cases, `gh` will attempt to fetch logs for each job individually via the API.
This fallback is slower and more resource-intensive. If more than 25 job logs are missing,
the operation will fail with an error.

Additionally, due to similar platform constraints, some log lines may not be
associated with a specific step within a job. In these cases, the step name will
appear as `UNKNOWN STEP` in the log output.

For more information about output formatting flags, see `gh help formatting`.

## Synopsis

```bash
gh run view [<run-id>] [flags]
```

## Flags

```text
-a, --attempt uint      The attempt number of the workflow run
      --exit-status       Exit with non-zero status if run failed
  -j, --job string        View a specific job ID from a run
  -q, --jq expression     Filter JSON output using a jq expression
      --json fields       Output JSON with the specified fields
      --log               View full log for either a run or specific job
      --log-failed        View the log for any failed steps in a run or specific job
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
  -v, --verbose           Show job steps
  -w, --web               Open run in the browser
```

## Inherited Flags

```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format

JSON FIELDS
  attempt, conclusion, createdAt, databaseId, displayTitle, event, headBranch,
  headSha, jobs, name, number, startedAt, status, updatedAt, url,
  workflowDatabaseId, workflowName
```

## Examples

```bash
# Interactively select a run to view, optionally selecting a single job
  $ gh run view
  
  # View a specific run
  $ gh run view 12345
  
  # View a specific run with specific attempt number
  $ gh run view 12345 --attempt 3
  
  # View a specific job within a run
  $ gh run view --job 456789
  
  # View the full log for a specific job
  $ gh run view --log --job 456789
  
  # Exit non-zero if a run failed
  $ gh run view 0451 --exit-status && echo "run pending or passed"
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
