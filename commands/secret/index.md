# `gh secret`

> Secrets can be set at the repository, or organization level for use in

## Description

GitHub Actions, Agents, or Dependabot. User, organization, and repository secrets can be set for
use in GitHub Codespaces. Environment secrets can be set for use in
GitHub Actions. Run `gh help secret set` to learn how to get started.

## Synopsis

```bash
gh secret <command> [flags]

AVAILABLE COMMANDS
  delete:        Delete secrets
  list:          List secrets
  set:           Create or update secrets
```

## Subcommands

| Command | Description |
| :--- | :--- |
| [`gh secret delete`](./delete.md) | Delete secrets |
| [`gh secret list`](./list.md) | List secrets |
| [`gh secret set`](./set.md) | Create or update secrets |

## Flags

```text
-R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
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
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
