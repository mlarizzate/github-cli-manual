# `gh release verify-asset`

> Verify that a given asset file originated from a specific GitHub Release using cryptographically signed attestations.

## Description

An attestation is a claim made by GitHub regarding a release and its assets.

		This command checks that the asset you provide matches a valid attestation for the specified release (or the latest release, if no tag is given).
It ensures the asset's integrity by validating that the asset's digest matches the subject in the attestation and that the attestation is associated with the release.

For more information about output formatting flags, see `gh help formatting`.

## Synopsis

```bash
gh release verify-asset [<tag>] <file-path> [flags]
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
# Verify an asset from the latest release
  $ gh release verify-asset ./dist/my-asset.zip
  
  # Verify an asset from a specific release tag
  $ gh release verify-asset v1.2.3 ./dist/my-asset.zip
  
  # Verify an asset from a specific release tag and output the attestation in JSON format
  $ gh release verify-asset v1.2.3 ./dist/my-asset.zip --format json
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
