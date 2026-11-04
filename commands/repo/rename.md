# `gh repo rename`

> Rename a GitHub repository.

## Description

`<new-name>` is the desired repository name without the owner.

By default, the current repository is renamed. Otherwise, the repository specified
with `--repo` is renamed.

To transfer repository ownership to another user account or organization,
you must follow additional steps on `github.com`.

For more information on transferring repository ownership, see:
<https://docs.github.com/en/repositories/creating-and-managing-repositories/transferring-a-repository>

## Synopsis

```bash
gh repo rename [<new-name>] [flags]
```

## Flags

```text
-R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
  -y, --yes                      Skip the confirmation prompt
```

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
# Rename the current repository (foo/bar -> foo/baz)
  $ gh repo rename baz
  
  # Rename the specified repository (qux/quux -> qux/baz)
  $ gh repo rename -R qux/quux baz
```

## AI Agent Automation Tips

- **Non-Interactive Execution**: Always pass affirmative flags (e.g., `--yes` or `--confirm`) to prevent hanging in interactive prompts.
- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh repo`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
