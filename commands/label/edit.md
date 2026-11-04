# `gh label edit`

> Update a label on GitHub.

## Description

A label can be renamed using the `--name` flag.

The label color needs to be 6 character hex value.

## Synopsis

```bash
gh label edit <name> [flags]
```

## Flags

```text
-c, --color string         Color of the label
  -d, --description string   Description of the label
  -n, --name string          New name of the label
```

## Inherited Flags

```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

## Examples

```bash
# Update the color of the bug label
  $ gh label edit bug --color FF0000
  
  # Rename and edit the description of the bug label
  $ gh label edit bug --name big-bug --description "Bigger than normal bug"
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh label`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
