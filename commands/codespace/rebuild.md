# `gh codespace rebuild`

> Rebuilding recreates your codespace.

## Description

Your code and any current changes will be preserved. Your codespace will be rebuilt using
your working directory's dev container. A full rebuild also removes cached Docker images.

## Synopsis

```bash
gh codespace rebuild [flags]
```

## Flags

```text
-c, --codespace string    Name of the codespace
      --full                Perform a full rebuild
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
