# `gh project item-create`

> Create a draft issue item in a project

## Description

For more information about output formatting flags, see `gh help formatting`.

## Synopsis

```bash
gh project item-create [<number>] [flags]
```

## Flags

```text
--body string       Body for the draft issue
      --format string     Output format: {json}
  -q, --jq expression     Filter JSON output using a jq expression
      --owner string      Login of the owner. Use "@me" for the current user.
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
      --title string      Title for the draft issue
```

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
# Create a draft issue in the current user's project "1"
  $ gh project item-create 1 --owner "@me" --title "new item" --body "new item body"
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
