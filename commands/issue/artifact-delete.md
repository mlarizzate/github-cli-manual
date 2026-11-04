# `gh issue artifact delete`

> Delete artifacts from an issue. A deleted artifact can't be restored.

## Description

Name artifacts by their issue and numbers, or by their URLs, which must all be
on one issue. `<issue>` is an issue number or URL.

In a terminal, deletion requires confirmation. `--yes` skips the prompt and is
required when prompting is unavailable.

## Synopsis

```bash
gh issue artifact delete {<issue> <artifact-number>... | <artifact-url>...} [flags]
```

## Flags

```text
--yes   Confirm deletion without prompting
```

## Inherited Flags

```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

## Examples

```bash
# Delete artifact 2 from issue 142
  $ gh issue artifact delete 142 2
  
  # Delete two artifacts without a prompt
  $ gh issue artifact delete 142 2 5 --yes
```

## AI Agent Automation Tips

- **Non-Interactive Execution**: Always pass affirmative flags (e.g., `--yes` or `--confirm`) to prevent hanging in interactive prompts.
- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh issue`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
