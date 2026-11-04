# `gh issue close`

> Close issue

## Synopsis

```bash
gh issue close {<number> | <url>} [flags]
```

## Flags

```text
-c, --comment string        Leave a closing comment
      --duplicate-of string   Mark as duplicate of another issue by number or URL
  -r, --reason string         Reason for closing: {completed|not planned|duplicate}
```

## Inherited Flags

```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

## Examples

```bash
# Close issue
  $ gh issue close 123
  
  # Close issue and add a closing comment
  $ gh issue close 123 --comment "Closing this issue"
  
  # Close issue as a duplicate of issue #456
  $ gh issue close 123 --duplicate-of 456
  
  # Close issue as not planned
  $ gh issue close 123 --reason "not planned"
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh issue`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
