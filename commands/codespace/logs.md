# `gh codespace logs`

> Access codespace logs

## Synopsis

```bash
gh codespace logs [flags]
```

## Flags

```text
-c, --codespace string    Name of the codespace
  -f, --follow              Tail and follow the logs
  -R, --repo string         Filter codespace selection by repository name (user/repo)
      --repo-owner string   Filter codespace selection by repository owner (username or org)
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
- [`gh codespace`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
