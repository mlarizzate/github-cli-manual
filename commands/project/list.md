# `gh project list`

> List the projects for an owner

## Description

For more information about output formatting flags, see `gh help formatting`.

## Synopsis

```bash
gh project list [flags]
```

## Aliases

- `gh project ls`

## Flags

```text
--closed            Include closed projects
      --format string     Output format: {json}
  -q, --jq expression     Filter JSON output using a jq expression
  -L, --limit int         Maximum number of projects to fetch (default 30)
      --owner string      Login of the owner
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
  -w, --web               Open projects list in the browser
```

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
# List the current user's projects
  $ gh project list
  
  # List the projects for org github including closed projects
  $ gh project list --owner github --closed
```

## AI Agent Automation Tips

- **Explicit Parameters**: In automation pipelines, explicitly pass flags like `--title`, `--body`, or `--body-file -` to bypass editor popups.
- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh project`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
