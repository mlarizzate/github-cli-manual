# `gh repo deploy-key add`

> Add a deploy key to a GitHub repository.

## Description

Note that any key added by gh will be associated with the current authentication token.
If you de-authorize the GitHub CLI app or authentication token from your account, any
deploy keys added by GitHub CLI will be removed as well.

## Synopsis

```bash
gh repo deploy-key add <key-file> [flags]
```

## Flags

```text
-w, --allow-write    Allow write access for the key
  -t, --title string   Title of the new key
```

## Inherited Flags

```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

## Examples

```bash
# Generate a passwordless SSH key and add it as a deploy key to a repository
  $ ssh-keygen -t ed25519 -C "my description" -N "" -f ~/.ssh/gh-test
  $ gh repo deploy-key add ~/.ssh/gh-test.pub
```

## AI Agent Automation Tips

- **Explicit Parameters**: In automation pipelines, explicitly pass flags like `--title`, `--body`, or `--body-file -` to bypass editor popups.
- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh repo`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
