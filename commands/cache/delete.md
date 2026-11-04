# `gh cache delete`

> Delete GitHub Actions caches.

## Description

Deletion requires authorization with the `repo` scope.

## Synopsis

```bash
gh cache delete [<cache-id> | <cache-key> | --all] [flags]
```

## Flags

```text
-a, --all                          Delete all caches, can be used with --ref to delete all caches for a specific ref
  -r, --ref string                   Delete by cache key and ref, formatted as refs/heads/<branch name> or refs/pull/<number>/merge
      --succeed-on-no-caches --all   Return exit code 0 if no caches found. Must be used in conjunction with --all
```

## Inherited Flags

```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

## Examples

```bash
# Delete a cache by id
  $ gh cache delete 1234
  
  # Delete a cache by key
  $ gh cache delete cache-key
  
  # Delete a cache by id in a specific repo
  $ gh cache delete 1234 --repo cli/cli
  
  # Delete a cache by key and branch ref
  $ gh cache delete cache-key --ref refs/heads/feature-branch
  
  # Delete a cache by key and PR ref
  $ gh cache delete cache-key --ref refs/pull/<PR-number>/merge
  
  # Delete all caches (exit code 1 on no caches)
  $ gh cache delete --all
  
  # Delete all caches for a specific ref
  $ gh cache delete --all --ref refs/pull/<PR-number>/merge
  
  # Delete all caches (exit code 0 on no caches)
  $ gh cache delete --all --succeed-on-no-caches
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh cache`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
