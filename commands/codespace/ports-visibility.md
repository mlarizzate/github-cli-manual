# `gh codespace ports visibility`

> Change the visibility of the forwarded port

## Synopsis

```bash
gh codespace ports visibility <port>:{public|private|org}... [flags]
```

## Inherited Flags

```text
-c, --codespace string    Name of the codespace
      --help                Show help for command
  -R, --repo string         Filter codespace selection by repository name (user/repo)
      --repo-owner string   Filter codespace selection by repository owner (username or org)
```

## Examples

```bash
$ gh codespace ports visibility 80:org 3000:private 8000:public
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh codespace`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
