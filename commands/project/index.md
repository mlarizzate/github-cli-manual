# `gh project`

> Work with GitHub Projects.

## Description

The minimum required scope for the token is: `project`.
You can verify your token scope by running `gh auth status` and
add the `project` scope by running `gh auth refresh -s project`.

## Synopsis

```bash
gh project <command> [flags]

AVAILABLE COMMANDS
  close:         Close a project
  copy:          Copy a project
  create:        Create a project
  delete:        Delete a project
  edit:          Edit a project
  field-create:  Create a field in a project
  field-delete:  Delete a field in a project
  field-list:    List the fields in a project
  item-add:      Add a pull request or an issue to a project
  item-archive:  Archive an item in a project
  item-create:   Create a draft issue item in a project
  item-delete:   Delete an item from a project by ID
  item-edit:     Edit an item in a project
  item-list:     List the items in a project
  link:          Link a project to a repository or a team
  list:          List the projects for an owner
  mark-template: Mark a project as a template
  unlink:        Unlink a project from a repository or a team
  view:          View a project
```

## Subcommands

| Command | Description |
| :--- | :--- |
| [`gh project close`](./close.md) | Close a project |
| [`gh project copy`](./copy.md) | Copy a project |
| [`gh project create`](./create.md) | Create a project |
| [`gh project delete`](./delete.md) | Delete a project |
| [`gh project edit`](./edit.md) | Edit a project |
| [`gh project field-create`](./field-create.md) | Create a field in a project |
| [`gh project field-delete`](./field-delete.md) | Delete a field in a project |
| [`gh project field-list`](./field-list.md) | List the fields in a project |
| [`gh project item-add`](./item-add.md) | Add a pull request or an issue to a project |
| [`gh project item-archive`](./item-archive.md) | Archive an item in a project |
| [`gh project item-create`](./item-create.md) | Create a draft issue item in a project |
| [`gh project item-delete`](./item-delete.md) | Delete an item from a project by ID |
| [`gh project item-edit`](./item-edit.md) | Edit an item in a project |
| [`gh project item-list`](./item-list.md) | List the items in a project |
| [`gh project link`](./link.md) | Link a project to a repository or a team |
| [`gh project list`](./list.md) | List the projects for an owner |
| [`gh project mark-template`](./mark-template.md) | Mark a project as a template |
| [`gh project unlink`](./unlink.md) | Unlink a project from a repository or a team |
| [`gh project view`](./view.md) | View a project |

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
$ gh project create --owner monalisa --title "Roadmap"
  $ gh project view 1 --owner cli --web
  $ gh project field-list 1 --owner cli
  $ gh project item-list 1 --owner cli
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
