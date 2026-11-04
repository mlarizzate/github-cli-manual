# `gh release verify`

> Verify that a GitHub Release is accompanied by a valid cryptographically signed attestation.

## Description

An attestation is a claim made by GitHub regarding a release and its assets.

This command checks that the specified release (or the latest release, if no tag is given) has a valid attestation. 
It fetches the attestation for the release and prints metadata about all assets referenced in the attestation, including their digests.

For more information about output formatting flags, see `gh help formatting`.

## Synopsis

```bash
gh release verify [<tag>] [flags]
```

## Flags

```text
--format string     Output format: {json}
  -q, --jq expression     Filter JSON output using a jq expression
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
```

## Inherited Flags

```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

## Examples

```bash
# Verify the latest release
  gh release verify
  
  # Verify a specific release by tag
  gh release verify v1.2.3
  
  # Verify a specific release by tag and output the attestation in JSON format
  gh release verify v1.2.3 --format json
```

## AI Agent Automation Tips

- **Explicit Parameters**: In automation pipelines, explicitly pass flags like `--title`, `--body`, or `--body-file -` to bypass editor popups.
- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh release`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
