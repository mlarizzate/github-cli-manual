# `gh repo set-default`

> This command sets the default remote repository to use when querying the

## Description

GitHub API for the locally cloned repository.

gh uses the default repository for things like:

 - viewing and creating pull requests
 - viewing and creating issues
 - viewing and creating releases
 - working with GitHub Actions

### NOTE: gh does not use the default repository for managing repository and environment secrets.

## Synopsis

```bash
gh repo set-default [<repository>] [flags]
```

## Flags

```text
-u, --unset   Unset the current default repository
  -v, --view    View the current default repository
```

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
# Interactively select a default repository
  $ gh repo set-default
  
  # Set a repository explicitly
  $ gh repo set-default owner/repo
  
  # Set a repository using a git remote name
  $ gh repo set-default origin
  
  # View the current default repository
  $ gh repo set-default --view
  
  # Show more repository options in the interactive picker
  $ git remote add newrepo https://github.com/owner/repo
  $ gh repo set-default
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh repo`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
