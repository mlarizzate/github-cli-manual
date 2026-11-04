# `gh gist view`

> View the given gist or select from recent gists.

## Synopsis

```bash
gh gist view [<id> | <url>] [flags]
```

## Flags

```text
--allow-escape-sequences   Allow printing terminal escape sequences
  -f, --filename string          Display a single file from the gist
      --files                    List file names from the gist
  -r, --raw                      Print raw instead of rendered gist contents
  -w, --web                      Open gist in the browser
```

## Inherited Flags

```text
--help   Show help for command
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh gist`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
