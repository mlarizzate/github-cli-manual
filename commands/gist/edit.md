# `gh gist edit`

> Edit one of your gists

## Synopsis

```bash
gh gist edit {<id> | <url>} [<filename>] [flags]
```

## Flags

```text
-a, --add string        Add a new file to the gist
  -d, --desc string       New description for the gist
  -f, --filename string   Select a file to edit
  -r, --remove string     Remove a file from the gist
```

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
# Select a gist to edit interactively
  $ gh gist edit
  
  # Edit a gist file in the default editor
  $ gh gist edit 1234567890abcdef1234567890abcdef
  
  # Edit a specific file in the gist
  $ gh gist edit 1234567890abcdef1234567890abcdef --filename hello.py
  
  # Replace a gist file with content from a local file
  $ gh gist edit 1234567890abcdef1234567890abcdef --filename hello.py hello.py
  
  # Add a new file to the gist
  $ gh gist edit 1234567890abcdef1234567890abcdef --add newfile.py
  
  # Change the description of the gist
  $ gh gist edit 1234567890abcdef1234567890abcdef --desc "new description"
  
  # Remove a file from the gist
  $ gh gist edit 1234567890abcdef1234567890abcdef --remove hello.py
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh gist`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
