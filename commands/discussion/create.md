# `gh discussion create`

> Create a new GitHub Discussion in a repository.

## Description

With `--title`, `--body` (or `--body-file`), and `--category`, a discussion is created non-interactively.
Omitting any of these flags triggers interactive prompts when connected to a terminal.

## Synopsis

```bash
gh discussion create [flags]
```

## Flags

```text
-b, --body string              Body for the discussion
  -F, --body-file string         Read body text from file (use "-" to read from stdin)
  -c, --category string          Category name or slug for the discussion
  -l, --label strings            Labels to apply to the discussion
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
  -t, --title string             Title for the discussion
```

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
# Create interactively
  $ gh discussion create
  
  # Create non-interactively
  $ gh discussion create --title "My question" --category "Q&A" --body "Details here"
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
