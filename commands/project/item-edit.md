# `gh project item-edit`

> Edit a draft issue or a project item.

## Description

The usual way to select the item and field is by name: pass the project
`number` plus `--owner`, point at the item with its issue or pull
request `--url`, and name the field with `--field`. For single-select
fields, `--value` is the option name.

For scripts and machine use, you can also pass GraphQL node IDs directly with
`--id`, `--field-id` and `--project-id` (and, for single-select
fields, `--single-select-option-id`).

Note that `--url` is the issue or pull request URL, not a project URL, so its
owner may differ from the project's; `--owner` selects the project.

For non-draft issues, only a single field value can be updated per invocation.

Remove a project item field value with `--clear`.

For more information about output formatting flags, see `gh help formatting`.

## Synopsis

```bash
gh project item-edit [<number>] [flags]
```

## Flags

```text
--body string                      Body of the draft issue item
      --clear                            Remove field value
      --date string                      Date value for the field (YYYY-MM-DD)
      --field string                     Name of the field to update
      --field-id string                  ID of the field to update
      --format string                    Output format: {json}
      --id string                        ID of the item to edit
      --iteration-id string              ID of the iteration value to set on the field
  -q, --jq expression                    Filter JSON output using a jq expression
      --number float                     Number value for the field
      --owner string                     Login of the owner. Use "@me" for the current user.
      --project-id string                ID of the project to which the field belongs to
      --single-select-option-id string   ID of the single select option value to set on the field
  -t, --template string                  Format JSON output using a Go template; see "gh help formatting"
      --text string                      Text value for the field
      --title string                     Title of the draft issue item
      --url string                       URL of the issue or pull request whose project item to edit
      --value --field                    Value to set on the field named by --field
```

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
# Set the "Status" field to "In Progress" for an issue on monalisa's project 1
  $ gh project item-edit 1 --owner monalisa --url https://github.com/monalisa/myproject/issues/23 --field "Status" --value "In Progress"
  
  # Edit an item's text field value by node ID (machine / scripted use)
  $ gh project item-edit --id <item-id> --field-id <field-id> --project-id <project-id> --text "new text"
  
  # Clear an item's field value by node ID
  $ gh project item-edit --id <item-id> --field-id <field-id> --project-id <project-id> --clear
```

## AI Agent Automation Tips

- **Explicit Parameters**: In automation pipelines, explicitly pass flags like `--title`, `--body`, or `--body-file -` to bypass editor popups.
- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh project`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
