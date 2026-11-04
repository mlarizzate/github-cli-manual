# `gh release edit`

> Edit a release

## Synopsis

```bash
gh release edit <tag>
```

## Flags

```text
--discussion-category string   Start a discussion in the specified category when publishing a draft
      --draft                        Save the release as a draft instead of publishing it
      --latest                       Explicitly mark the release as "Latest"
  -n, --notes string                 Release notes
  -F, --notes-file file              Read release notes from file (use "-" to read from standard input)
      --prerelease                   Mark the release as a prerelease
      --tag string                   The name of the tag
      --target branch                Target branch or full commit SHA (default [main branch])
  -t, --title string                 Release title
      --verify-tag                   Abort in case the git tag doesn't already exist in the remote repository
```

## Inherited Flags

```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

## Examples

```bash
# Publish a release that was previously a draft
  $ gh release edit v1.0 --draft=false
  
  # Update the release notes from the content of a file
  $ gh release edit v1.0 --notes-file /path/to/release_notes.md
```

## AI Agent Automation Tips

- **Explicit Parameters**: In automation pipelines, explicitly pass flags like `--title`, `--body`, or `--body-file -` to bypass editor popups.
- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh release`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
