# `gh status`

> The status command prints information about your work on GitHub across all the repositories you're subscribed to, including:

## Description

- Assigned Issues
- Assigned Pull Requests
- Review Requests
- Mentions
- Repository Activity (new issues/pull requests, comments)

## Synopsis

```bash
gh status [flags]
```

## Flags

```text
-e, --exclude strings   Comma separated list of repos to exclude in owner/name format
  -o, --org string        Report status within an organization
```

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
$ gh status -e cli/cli -e cli/go-gh # Exclude multiple repositories
  $ gh status -o cli # Limit results to a single organization
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
