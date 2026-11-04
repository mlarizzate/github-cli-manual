# `gh codespace stop`

> Stop a running codespace

## Synopsis

```bash
gh codespace stop [flags]
```

## Flags

```text
-c, --codespace string    Name of the codespace
  -o, --org login           The login handle of the organization (admin-only)
  -R, --repo string         Filter codespace selection by repository name (user/repo)
      --repo-owner string   Filter codespace selection by repository owner (username or org)
  -u, --user username       The username to stop codespace for (used with --org)
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
