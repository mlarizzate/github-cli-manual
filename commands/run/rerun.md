# `gh run rerun`

> Rerun an entire run, only failed jobs, or a specific job from a run.

## Description

Note that due to historical reasons, the `--job` flag may not take what you expect.
Specifically, when navigating to a job in the browser, the URL looks like this:
`https://github.com/<owner>/<repo>/actions/runs/<run-id>/jobs/<number>`.

However, this `<number>` should not be used with the `--job` flag and will result in the
API returning `404 NOT FOUND`. Instead, you can get the correct job IDs using the following command:

	gh run view <run-id> --json jobs --jq '.jobs[] | {name, databaseId}'

You will need to use databaseId field for triggering job re-runs.

## Synopsis

```bash
gh run rerun [<run-id>] [flags]
```

## Flags

```text
-d, --debug        Rerun with debug logging
      --failed       Rerun only failed jobs, including dependencies
  -j, --job string   Rerun a specific job ID from a run, including dependencies
```

## Inherited Flags

```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh run`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
