# `gh repo gitignore view`

> View an available repository `.gitignore` template.

## Description

`<template>` is a case-sensitive `.gitignore` template name.

For a list of available templates, run `gh repo gitignore list`.

## Synopsis

```bash
gh repo gitignore view <template> [flags]
```

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
# View the Go gitignore template
  $ gh repo gitignore view Go
  
  # View the Python gitignore template
  $ gh repo gitignore view Python
  
  # Create a new .gitignore file using the Go template
  $ gh repo gitignore view Go > .gitignore
  
  # Create a new .gitignore file using the Python template
  $ gh repo gitignore view Python > .gitignore
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh repo`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
