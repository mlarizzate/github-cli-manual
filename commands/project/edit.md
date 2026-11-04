# `gh project edit`

> Edit a project

## Description

For more information about output formatting flags, see `gh help formatting`.

## Synopsis

```bash
gh project edit [<number>] [flags]
```

## Flags

```text
-d, --description string   New description of the project
      --format string        Output format: {json}
  -q, --jq expression        Filter JSON output using a jq expression
      --owner string         Login of the owner. Use "@me" for the current user.
      --readme string        New readme for the project
  -t, --template string      Format JSON output using a Go template; see "gh help formatting"
      --title string         New title for the project
      --visibility string    Change project visibility: {PUBLIC|PRIVATE}
```

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
# Edit the title of monalisa's project "1"
  $ gh project edit 1 --owner monalisa --title "New title"
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
