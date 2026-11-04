# `gh project copy`

> Copy a project

## Description

For more information about output formatting flags, see `gh help formatting`.

## Synopsis

```bash
gh project copy [<number>] [flags]
```

## Flags

```text
--drafts                Include draft issues when copying
      --format string         Output format: {json}
  -q, --jq expression         Filter JSON output using a jq expression
      --source-owner string   Login of the source owner. Use "@me" for the current user.
      --target-owner string   Login of the target owner. Use "@me" for the current user.
  -t, --template string       Format JSON output using a Go template; see "gh help formatting"
      --title string          Title for the new project
```

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
# Copy project "1" owned by monalisa to github
  $ gh project copy 1 --source-owner monalisa --target-owner github --title "a new project"
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
