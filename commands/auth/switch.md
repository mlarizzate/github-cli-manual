# `gh auth switch`

> Switch the active account for a GitHub host.

## Description

This command changes the authentication configuration that will
be used when running commands targeting the specified GitHub host.

If the specified host has two accounts, the active account will be switched
automatically. If there are more than two accounts, disambiguation will be
required either through the `--user` flag or an interactive prompt.

For a list of authenticated accounts you can run `gh auth status`.

## Synopsis

```bash
gh auth switch [flags]
```

## Flags

```text
-h, --hostname string   The hostname of the GitHub instance to switch account for
  -u, --user string       The account to switch to
```

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
# Select what host and account to switch to via a prompt
  $ gh auth switch
  
  # Switch the active account on a specific host to a specific user
  $ gh auth switch --hostname enterprise.internal --user monalisa
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh auth`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
