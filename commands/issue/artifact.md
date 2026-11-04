# `gh issue artifact`

> Working with issue artifacts in the GitHub CLI is in preview and subject to change without notice.

## Description

Issue artifacts are Markdown documents, HTML documents and links attached to an issue.
They are not GitHub Actions artifacts; to download those, use `gh run download`.

## Synopsis

```bash
gh issue artifact <command> [flags]

AVAILABLE COMMANDS
  create:        Create issue artifacts (preview)
  delete:        Delete issue artifacts (preview)
  download:      Download issue artifacts (preview)
  edit:          Edit an issue artifact (preview)
  list:          List artifacts on an issue (preview)
  view:          View an issue artifact (preview)
```

## Subcommands

| Command | Description |
| :--- | :--- |
| [`gh issue artifact create`](./artifact-create.md) | Create issue artifacts (preview) |
| [`gh issue artifact delete`](./artifact-delete.md) | Delete issue artifacts (preview) |
| [`gh issue artifact download`](./artifact-download.md) | Download issue artifacts (preview) |
| [`gh issue artifact edit`](./artifact-edit.md) | Edit an issue artifact (preview) |
| [`gh issue artifact list`](./artifact-list.md) | List artifacts on an issue (preview) |
| [`gh issue artifact view`](./artifact-view.md) | View an issue artifact (preview) |

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
- [`gh issue`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
