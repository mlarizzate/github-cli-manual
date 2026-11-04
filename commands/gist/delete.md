# `gh gist delete`

> Delete a GitHub gist.

## Description

To delete a gist interactively, use `gh gist delete` with no arguments.

To delete a gist non-interactively, supply the gist id or url.

## Synopsis

```bash
gh gist delete {<id> | <url>} [flags]
```

## Flags

```text
--yes   Confirm deletion without prompting
```

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
# Delete a gist interactively
  $ gh gist delete
  
  # Delete a gist non-interactively
  $ gh gist delete 1234
```

## AI Agent Automation Tips

- **Non-Interactive Execution**: Always pass affirmative flags (e.g., `--yes` or `--confirm`) to prevent hanging in interactive prompts.
- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh gist`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
