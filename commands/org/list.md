# `gh org list`

> List organizations for the authenticated user.

## Synopsis

```bash
gh org list [flags]
```

## Aliases

- `gh org ls`

## Flags

```text
-L, --limit int   Maximum number of organizations to list (default 30)
```

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
# List the first 30 organizations
  $ gh org list
  
  # List more organizations
  $ gh org list --limit 100
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh org`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
