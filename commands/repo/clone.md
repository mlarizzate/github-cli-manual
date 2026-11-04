# `gh repo clone`

> Clone a GitHub repository locally. Pass additional `git clone` flags by listing

## Description

them after `--`.

If the `OWNER/` portion of the `OWNER/REPO` repository argument is omitted, it
defaults to the name of the authenticating user.

When a protocol scheme is not provided in the repository argument, the `git_protocol` will be
chosen from your configuration, which can be checked via `gh config get git_protocol`. If the protocol
scheme is provided, the repository will be cloned using the specified protocol.

If the repository is a fork, its parent repository will be added as an additional
git remote called `upstream`. The remote name can be configured using `--upstream-remote-name`.
The `--upstream-remote-name` option supports an `@owner` value which will name
the remote after the owner of the parent repository.

If the repository is a fork, its parent repository will be set as the default remote repository.
To skip this behavior, use `--no-upstream`.

## Synopsis

```bash
gh repo clone <repository> [<directory>] [-- <gitflags>...]
```

## Flags

```text
--no-upstream                   Do not add an upstream remote when cloning a fork
  -u, --upstream-remote-name string   Upstream remote name when cloning a fork (default "upstream")
```

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
# Clone a repository from a specific org
  $ gh repo clone cli/cli
  
  # Clone a repository from your own account
  $ gh repo clone myrepo
  
  # Clone a repo, overriding git protocol configuration
  $ gh repo clone https://github.com/cli/cli
  $ gh repo clone git@github.com:cli/cli.git
  
  # Clone a repository to a custom directory
  $ gh repo clone cli/cli workspace/cli
  
  # Clone a repository with additional git clone flags
  $ gh repo clone cli/cli -- --depth=1
  
  # Clone a fork without adding an upstream remote
  $ gh repo clone myfork --no-upstream
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh repo`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
