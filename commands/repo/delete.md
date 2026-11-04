# `gh repo delete`

> Delete a GitHub repository.

## Description

With no argument, deletes the current repository. Otherwise, deletes the specified repository.

For safety, when no repository argument is provided, the `--yes` flag is ignored 
and you will be prompted for confirmation. To delete the current repository non-interactively, 
specify it explicitly (e.g., `gh repo delete owner/repo --yes`).

Deletion requires authorization with the `delete_repo` scope.
To authorize, run `gh auth refresh -s delete_repo`

## Synopsis

```bash
gh repo delete [<repository>] [flags]
```

## Flags

```text
--yes   Confirm deletion without prompting
```

## Inherited Flags

```text
--help   Show help for command
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
