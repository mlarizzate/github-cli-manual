# `gh auth setup-git`

> This command configures `git` to use GitHub CLI as a credential helper.

## Description

For more information on git credential helpers please reference:
<https://git-scm.com/docs/gitcredentials>.

By default, GitHub CLI will be set as the credential helper for all authenticated hosts.
If there is no authenticated hosts the command fails with an error.

Alternatively, use the `--hostname` flag to specify a single host to be configured.
If the host is not authenticated with, the command fails with an error.

## Synopsis

```bash
gh auth setup-git [flags]
```

## Flags

```text
-f, --force --hostname   Force setup even if the host is not known. Must be used in conjunction with --hostname
  -h, --hostname string    The hostname to configure git for
```

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
# Configure git to use GitHub CLI as the credential helper for all authenticated hosts
  $ gh auth setup-git
  
  # Configure git to use GitHub CLI as the credential helper for enterprise.internal host
  $ gh auth setup-git --hostname enterprise.internal
```

## AI Agent Automation Tips

- **Non-Interactive Execution**: Always pass affirmative flags (e.g., `--yes` or `--confirm`) to prevent hanging in interactive prompts.
- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh auth`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
