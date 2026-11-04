# `gh attestation`

> Download and verify artifact attestations.

## Synopsis

```bash
gh attestation [subcommand] [flags]
```

## Aliases

- `gh at`
- `AVAILABLE COMMANDS`
- `download:      Download an artifact's attestations for offline use`
- `trusted-root:  Output trusted_root.jsonl contents, likely for offline verification`
- `verify:        Verify an artifact's integrity using attestations`

## Subcommands

| Command | Description |
| :--- | :--- |
| [`gh attestation download`](./download.md) | Download an artifact's attestations for offline use |
| [`gh attestation trusted-root`](./trusted-root.md) | Output trusted_root.jsonl contents, likely for offline verification |
| [`gh attestation verify`](./verify.md) | Verify an artifact's integrity using attestations |

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
