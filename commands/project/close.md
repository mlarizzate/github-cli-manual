# `gh project close`

> Close a project

## Description

For more information about output formatting flags, see `gh help formatting`.

## Synopsis

```bash
gh project close [<number>] [flags]
```

## Flags

```text
--format string     Output format: {json}
  -q, --jq expression     Filter JSON output using a jq expression
      --owner string      Login of the owner. Use "@me" for the current user.
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
      --undo              Reopen a closed project
```

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
# Close project "1" owned by monalisa
  $ gh project close 1 --owner monalisa
  
  # Reopen closed project "1" owned by github
  $ gh project close 1 --owner github --undo
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
