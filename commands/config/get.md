# `gh config get`

> Print the value of a given configuration key

## Synopsis

```bash
gh config get <key> [flags]
```

## Flags

```text
-h, --host string   Get per-host setting
```

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
$ gh config get git_protocol
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh config`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
