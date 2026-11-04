# `gh label clone`

> Clones labels from a source repository to a destination repository on GitHub.

## Description

By default, the destination repository is the current repository.

All labels from the source repository will be copied to the destination
repository. Labels in the destination repository that are not in the source
repository will not be deleted or modified.

Labels from the source repository that already exist in the destination
repository will be skipped. You can overwrite existing labels in the
destination repository using the `--force` flag.

## Synopsis

```bash
gh label clone <source-repository> [flags]
```

## Flags

```text
-f, --force   Overwrite labels in the destination repository
```

## Inherited Flags

```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

## Examples

```bash
# Clone and overwrite labels from cli/cli repository into the current repository
  $ gh label clone cli/cli --force
  
  # Clone labels from cli/cli repository into octocat/cli repository
  $ gh label clone cli/cli --repo octocat/cli
```

## AI Agent Automation Tips

- **Non-Interactive Execution**: Always pass affirmative flags (e.g., `--yes` or `--confirm`) to prevent hanging in interactive prompts.
- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh label`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
