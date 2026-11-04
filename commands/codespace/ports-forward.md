# `gh codespace ports forward`

> Forward ports from a codespace to your local machine.

## Description

Ports bind to loopback (`127.0.0.1`) by default. Use `--all-interfaces`
to bind to all interfaces.

## Synopsis

```bash
gh codespace ports forward <remote-port>:<local-port>... [flags]
```

## Flags

```text
--all-interfaces   Listen on all network interfaces
```

## Inherited Flags

```text
-c, --codespace string    Name of the codespace
      --help                Show help for command
  -R, --repo string         Filter codespace selection by repository name (user/repo)
      --repo-owner string   Filter codespace selection by repository owner (username or org)
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh codespace`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
