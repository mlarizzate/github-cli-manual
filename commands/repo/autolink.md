# `gh repo autolink`

> Autolinks link issues, pull requests, commit messages, and release descriptions to external third-party services.

## Description

Autolinks require `admin` role to view or manage.

For more information, see <https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/managing-repository-settings/configuring-autolinks-to-reference-external-resources>

## Synopsis

```bash
gh repo autolink <command> [flags]

AVAILABLE COMMANDS
  create:        Create a new autolink reference
  delete:        Delete an autolink reference
  list:          List autolink references for a GitHub repository
  view:          View an autolink reference
```

## Subcommands

| Command | Description |
| :--- | :--- |
| [`gh repo autolink create`](./autolink-create.md) | Create a new autolink reference |
| [`gh repo autolink delete`](./autolink-delete.md) | Delete an autolink reference |
| [`gh repo autolink list`](./autolink-list.md) | List autolink references for a GitHub repository |
| [`gh repo autolink view`](./autolink-view.md) | View an autolink reference |

## Flags

```text
-R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

## Inherited Flags

```text
--help   Show help for command
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh repo`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
