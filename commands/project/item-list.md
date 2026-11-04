# `gh project item-list`

> List the items in a project.

## Description

If supported by the API host, the --query option can be used to perform
advanced search. For the full syntax, see:
https://docs.github.com/en/issues/planning-and-tracking-with-projects/customizing-views-in-your-project/filtering-projects

For more information about output formatting flags, see `gh help formatting`.

## Synopsis

```bash
gh project item-list [<number>] [flags]
```

## Flags

```text
--field stringArray      Name of a field to show as an extra column
      --field-id stringArray   ID of a field to show as an extra column
      --format string          Output format: {json}
  -q, --jq expression          Filter JSON output using a jq expression
  -L, --limit int              Maximum number of items to fetch (default 30)
      --owner string           Login of the owner. Use "@me" for the current user
      --query string           Filter items using the Projects filter syntax, e.g. "assignee:octocat -status:Done"
  -t, --template string        Format JSON output using a Go template; see "gh help formatting"
```

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
# List the items in the current users's project "1"
  $ gh project item-list 1 --owner "@me"
  
  # List items assigned to a specific user
  $ gh project item-list 1 --owner "@me" --query "assignee:monalisa"
  
  # List open issues assigned to yourself
  $ gh project item-list 1 --owner "@me" --query "assignee:@me is:issue is:open"
  
  # List items with the "bug" label that are not done
  $ gh project item-list 1 --owner "@me" --query "label:bug -status:Done"
  
  # Show the "Status" and "Priority" field values as extra columns
  $ gh project item-list 1 --owner "@me" --field "Status" --field "Priority"
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
