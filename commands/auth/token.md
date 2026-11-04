# `gh auth token`

> This command outputs the authentication token for an account on a given GitHub host.

## Description

Without the `--hostname` flag, the default host is chosen.

Without the `--user` flag, the active account for the host is chosen.

If the token is an expired or near-expiry token that supports refreshing, it is refreshed
automatically before being printed, unless `--no-refresh` is given.

## Synopsis

```bash
gh auth token [flags]
```

## Flags

```text
-h, --hostname string   The hostname of the GitHub instance authenticated with
      --no-refresh        Do not automatically refresh an expired token
  -u, --user string       The account to output the token for
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
- [`gh auth`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
