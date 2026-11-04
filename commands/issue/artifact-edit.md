# `gh issue artifact edit`

> Rename an issue artifact or replace its content. The type never changes, so a

## Description

link's new content must be an http(s) URL or a `.url` Internet Shortcut file.

Name the artifact by its issue and number, or by its URL. `<issue>` is an
issue number or URL.

With only `--attach`, the attachments are appended to the current content.

With `--restore-version`, an earlier version's name and content are saved as a
new version. `gh issue artifact view` shows the edit history.

## Synopsis

```bash
gh issue artifact edit {<issue> <artifact-number> | <artifact-url>} [flags]
```

## Flags

```text
--attach file              Attach an image or video file, in '<file>#<image alt text>' format
  -b, --body string              New content; for a link, a URL
  -F, --body-file file           Read new content from file (use "-" to read from standard input)
      --name string              New name
      --restore-version number   Restore the version with this number from the edit history
```

## Inherited Flags

```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

## Examples

```bash
# Rename an artifact
  $ gh issue artifact edit 142 2 --name 'OAuth callback plan v2'
  
  # Replace a document's content with a file
  $ gh issue artifact edit 142 2 --body-file 2-OAuth-callback-plan.md
  
  # Point a link at a new URL
  $ gh issue artifact edit 142 3 --body https://github.com/monalisa/monas-cafe/wiki/OAuth-runbook-v2
  
  # Append an image to a document
  $ gh issue artifact edit 142 2 --attach ./signin-flow.png
  
  # Restore an earlier version
  $ gh issue artifact edit 142 2 --restore-version 5
```

## AI Agent Automation Tips

- **Explicit Parameters**: In automation pipelines, explicitly pass flags like `--title`, `--body`, or `--body-file -` to bypass editor popups.
- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh issue`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
