# `gh cache`

> Work with GitHub Actions caches.

## Synopsis

```bash
gh cache <command> [flags]

AVAILABLE COMMANDS
  delete:        Delete GitHub Actions caches
  list:          List GitHub Actions caches
```

## Subcommands

| Command | Description |
| :--- | :--- |
| [`gh cache delete`](./delete.md) | Delete GitHub Actions caches |
| [`gh cache list`](./list.md) | List GitHub Actions caches |

## Flags

```text
-R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
$ gh cache list
  $ gh cache delete --all
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
