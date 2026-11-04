# `gh config set`

> Update configuration with a value for the given key

## Synopsis

```bash
gh config set <key> <value> [flags]
```

## Flags

```text
-h, --host string   Set per-host setting
```

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
$ gh config set editor vim
  $ gh config set editor "code --wait"
  $ gh config set git_protocol ssh --host github.com
  $ gh config set api_host api-gateway.example.com --host example.com
  $ gh config set prompt disabled
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh config`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
