# `gh auth`

> Authenticate gh and git with GitHub

## Synopsis

```bash
gh auth <command> [flags]

AVAILABLE COMMANDS
  login:         Log in to a GitHub account
  logout:        Log out of a GitHub account
  refresh:       Refresh stored authentication credentials
  setup-git:     Setup git with GitHub CLI
  status:        Display active account and authentication state on each known GitHub host
  switch:        Switch active GitHub account
  token:         Print the authentication token gh uses for a hostname and account
```

## Subcommands

| Command | Description |
| :--- | :--- |
| [`gh auth login`](./login.md) | Log in to a GitHub account |
| [`gh auth logout`](./logout.md) | Log out of a GitHub account |
| [`gh auth refresh`](./refresh.md) | Refresh stored authentication credentials |
| [`gh auth setup-git`](./setup-git.md) | Setup git with GitHub CLI |
| [`gh auth status`](./status.md) | Display active account and authentication state on each known GitHub host |
| [`gh auth switch`](./switch.md) | Switch active GitHub account |
| [`gh auth token`](./token.md) | Print the authentication token gh uses for a hostname and account |

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
