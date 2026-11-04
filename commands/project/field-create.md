# `gh project field-create`

> Create a field in a project

## Description

For more information about output formatting flags, see `gh help formatting`.

## Synopsis

```bash
gh project field-create [<number>] [flags]
```

## Flags

```text
--data-type string                DataType of the new field.: {TEXT|SINGLE_SELECT|DATE|NUMBER}
      --format string                   Output format: {json}
  -q, --jq expression                   Filter JSON output using a jq expression
      --name string                     Name of the new field
      --owner string                    Login of the owner. Use "@me" for the current user.
      --single-select-options strings   Options for SINGLE_SELECT data type
  -t, --template string                 Format JSON output using a Go template; see "gh help formatting"
```

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
# Create a field in the current user's project "1"
  $ gh project field-create 1 --owner "@me" --name "new field" --data-type "text"
  
  # Create a field with three options to select from for owner monalisa
  $ gh project field-create 1 --owner monalisa --name "new field" --data-type "SINGLE_SELECT" --single-select-options "one,two,three"
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
