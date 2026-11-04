# `gh repo sync`

> Sync destination repository from source repository. Syncing uses the default branch

## Description

of the source repository to update the matching branch on the destination
repository so they are equal. A fast forward update will be used except when the
`--force` flag is specified, then the two branches will
be synced using a hard reset.

Without an argument, the local repository is selected as the destination repository.

The source repository is the parent of the destination repository by default.
This can be overridden with the `--source` flag.

## Synopsis

```bash
gh repo sync [<destination-repository>] [flags]
```

## Flags

```text
-b, --branch string   Branch to sync (default [default branch])
      --force           Hard reset the branch of the destination repository to match the source repository
  -s, --source string   Source repository
```

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
# Sync local repository from remote parent
  $ gh repo sync
  
  # Sync local repository from remote parent on specific branch
  $ gh repo sync --branch v1
  
  # Sync remote fork from its parent
  $ gh repo sync owner/cli-fork
  
  # Sync remote repository from another remote repository
  $ gh repo sync owner/repo --source owner2/repo2
```

## AI Agent Automation Tips

- **Non-Interactive Execution**: Always pass affirmative flags (e.g., `--yes` or `--confirm`) to prevent hanging in interactive prompts.
- **Explicit Parameters**: In automation pipelines, explicitly pass flags like `--title`, `--body`, or `--body-file -` to bypass editor popups.
- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh repo`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
