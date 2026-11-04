# `gh skill`

> Install and manage agent skills from GitHub repositories.

## Description

Working with agent skills in the GitHub CLI is in preview and
subject to change without notice.

## Synopsis

```bash
gh skill <command> [flags]
```

## Aliases

- `gh skills`
- `AVAILABLE COMMANDS`
- `install:       Install agent skills from a GitHub repository (preview)`
- `list:          List installed skills (preview)`
- `preview:       Preview a skill from a GitHub repository (preview)`
- `publish:       Validate and publish skills to a GitHub repository (preview)`
- `search:        Search for skills across GitHub (preview)`
- `update:        Update installed skills to their latest versions (preview)`

## Subcommands

| Command | Description |
| :--- | :--- |
| [`gh skill install`](./install.md) | Install agent skills from a GitHub repository (preview) |
| [`gh skill list`](./list.md) | List installed skills (preview) |
| [`gh skill preview`](./preview.md) | Preview a skill from a GitHub repository (preview) |
| [`gh skill publish`](./publish.md) | Validate and publish skills to a GitHub repository (preview) |
| [`gh skill search`](./search.md) | Search for skills across GitHub (preview) |
| [`gh skill update`](./update.md) | Update installed skills to their latest versions (preview) |

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
# Search for skills
  $ gh skill search terraform
  
  # Install a skill
  $ gh skill install github/awesome-copilot documentation-writer
  
  # List installed skills
  $ gh skill list
  
  # Preview a skill before installing
  $ gh skill preview github/awesome-copilot documentation-writer
  
  # Update all installed skills
  $ gh skill update --all
  
  # Validate skills for publishing
  $ gh skill publish --dry-run
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
