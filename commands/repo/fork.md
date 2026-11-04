# `gh repo fork`

> Create a fork of a repository.

## Description

With no argument, creates a fork of the current repository. Otherwise, forks
the specified repository.

By default, the new fork is set to be your `origin` remote and any existing
origin remote is renamed to `upstream`. To alter this behavior, you can set
a name for the new fork's remote with `--remote-name`.

The `upstream` remote will be set as the default remote repository.

Additional `git clone` flags can be passed after `--`.

## Synopsis

```bash
gh repo fork [<repository>] [-- <gitflags>...] [flags]
```

## Flags

```text
--clone                 Clone the fork
  --default-branch-only   Only include the default branch in the fork
  --fork-name string      Rename the forked repository
  --org string            Create the fork in an organization
  --remote                Add a git remote for the fork
  --remote-name string    Specify the name for the new remote (default "origin")
```

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
# Fork a repository
  $ gh repo fork owner/repo
  
  # Fork a repository and clone it locally
  $ gh repo fork owner/repo --clone
  
  # Fork a repository without cloning it, skip the prompt
  $ gh repo fork owner/repo --clone=false
```

## AI Agent Automation Tips

- **Explicit Parameters**: In automation pipelines, explicitly pass flags like `--title`, `--body`, or `--body-file -` to bypass editor popups.
- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh repo`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
