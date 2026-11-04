# `gh discussion edit`

> Edit a GitHub Discussion.

## Description

Without flags, the command runs interactively when connected to a terminal.
Use flags to update specific fields non-interactively.

## Synopsis

```bash
gh discussion edit {<number> | <discussion-url>} [flags]
```

## Flags

```text
--add-label name           Add labels by name
  -b, --body string              New body for the discussion
  -F, --body-file string         Read body text from file (use "-" to read from standard input)
  -c, --category string          New category name or slug for the discussion
      --remove-label name        Remove labels by name
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
  -t, --title string             New title for the discussion
```

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
# Edit interactively
  $ gh discussion edit 123
  
  # Update title, body, and category
  $ gh discussion edit 123 --title "Updated title" --body "Updated body" --category "Ideas"
  
  # Update body from a file
  $ gh discussion edit 123 --body-file body.md
  
  # Add and remove labels
  $ gh discussion edit 123 --add-label "bug,help wanted" --remove-label "stale"
```

## AI Agent Automation Tips

- **Explicit Parameters**: In automation pipelines, explicitly pass flags like `--title`, `--body`, or `--body-file -` to bypass editor popups.
- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh discussion`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
