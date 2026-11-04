# `gh pr revert`

> Revert a pull request

## Synopsis

```bash
gh pr revert {<number> | <url> | <branch>} [flags]
```

## Flags

```text
-b, --body string      Body for the revert pull request
  -F, --body-file file   Read body text from file (use "-" to read from standard input)
  -d, --draft            Mark revert pull request as a draft
  -t, --title string     Title for the revert pull request
```

## Inherited Flags

```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

## AI Agent Automation Tips

- **Explicit Parameters**: In automation pipelines, explicitly pass flags like `--title`, `--body`, or `--body-file -` to bypass editor popups.
- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh pr`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
