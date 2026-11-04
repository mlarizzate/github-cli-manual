# `gh extension create`

> Create a new extension

## Synopsis

```bash
gh extension create [<name>] [flags]
```

## Flags

```text
--precompiled string   Create a precompiled extension. Possible values: go, other
```

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
# Use interactively
  $ gh extension create
  
  # Create a script-based extension
  $ gh extension create foobar
  
  # Create a Go extension
  $ gh extension create --precompiled=go foobar
  
  # Create a non-Go precompiled extension
  $ gh extension create --precompiled=other foobar
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh extension`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
