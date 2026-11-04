# `gh codespace delete`

> Delete codespaces based on selection criteria.

## Description

All codespaces for the authenticated user can be deleted, as well as codespaces for a
specific repository. Alternatively, only codespaces older than N days can be deleted.

Organization administrators may delete any codespace billed to the organization.

## Synopsis

```bash
gh codespace delete [flags]
```

## Flags

```text
--all                 Delete all codespaces
  -c, --codespace string    Name of the codespace
      --days N              Delete codespaces older than N days
  -f, --force               Skip confirmation for codespaces that contain unsaved changes
  -o, --org login           The login handle of the organization (admin-only)
  -R, --repo string         Filter codespace selection by repository name (user/repo)
      --repo-owner string   Filter codespace selection by repository owner (username or org)
  -u, --user username       The username to delete codespaces for (used with --org)
```

## Inherited Flags

```text
--help   Show help for command
```

## AI Agent Automation Tips

- **Non-Interactive Execution**: Always pass affirmative flags (e.g., `--yes` or `--confirm`) to prevent hanging in interactive prompts.
- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh codespace`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
