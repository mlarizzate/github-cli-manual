# `gh repo`

> Work with GitHub repositories.

## Synopsis

```bash
gh repo <command> [flags]

GENERAL COMMANDS
  create:        Create a new repository
  list:          List repositories owned by user or organization

TARGETED COMMANDS
  archive:       Archive a repository
  autolink:      Manage autolink references
  clone:         Clone a repository locally
  delete:        Delete a repository
  deploy-key:    Manage deploy keys in a repository
  edit:          Edit repository settings
  fork:          Create a fork of a repository
  gitignore:     List and view available repository gitignore templates
  license:       Explore repository licenses
  read-dir:      List a directory in a repository (preview)
  read-file:     Read a file from a repository (preview)
  rename:        Rename a repository
  set-default:   Configure default repository for this directory
  sync:          Sync a repository
  unarchive:     Unarchive a repository
  view:          View a repository
```

## Subcommands

| Command | Description |
| :--- | :--- |
| [`gh repo create`](./create.md) | Create a new repository |
| [`gh repo list`](./list.md) | List repositories owned by user or organization |
| [`gh repo archive`](./archive.md) | Archive a repository |
| [`gh repo autolink`](./autolink.md) | Manage autolink references |
| [`gh repo clone`](./clone.md) | Clone a repository locally |
| [`gh repo delete`](./delete.md) | Delete a repository |
| [`gh repo deploy-key`](./deploy-key.md) | Manage deploy keys in a repository |
| [`gh repo edit`](./edit.md) | Edit repository settings |
| [`gh repo fork`](./fork.md) | Create a fork of a repository |
| [`gh repo gitignore`](./gitignore.md) | List and view available repository gitignore templates |
| [`gh repo license`](./license.md) | Explore repository licenses |
| [`gh repo read-dir`](./read-dir.md) | List a directory in a repository (preview) |
| [`gh repo read-file`](./read-file.md) | Read a file from a repository (preview) |
| [`gh repo rename`](./rename.md) | Rename a repository |
| [`gh repo set-default`](./set-default.md) | Configure default repository for this directory |
| [`gh repo sync`](./sync.md) | Sync a repository |
| [`gh repo unarchive`](./unarchive.md) | Unarchive a repository |
| [`gh repo view`](./view.md) | View a repository |

## Inherited Flags

```text
--help   Show help for command
```

## Arguments

```text
A repository can be supplied as an argument in any of the following formats:
  - "OWNER/REPO"
  - by URL, e.g. "https://github.com/OWNER/REPO"
```

## Examples

```bash
$ gh repo create
  $ gh repo clone cli/cli
  $ gh repo view --web
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
