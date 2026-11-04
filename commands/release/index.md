# `gh release`

> Manage releases

## Synopsis

```bash
gh release <command> [flags]

GENERAL COMMANDS
  create:        Create a new release
  list:          List releases in a repository

TARGETED COMMANDS
  delete:        Delete a release
  delete-asset:  Delete an asset from a release
  download:      Download release assets
  edit:          Edit a release
  upload:        Upload assets to a release
  verify:        Verify the attestation for a release
  verify-asset:  Verify that a given asset originated from a release
  view:          View information about a release
```

## Subcommands

| Command | Description |
| :--- | :--- |
| [`gh release create`](./create.md) | Create a new release |
| [`gh release list`](./list.md) | List releases in a repository |
| [`gh release delete`](./delete.md) | Delete a release |
| [`gh release delete-asset`](./delete-asset.md) | Delete an asset from a release |
| [`gh release download`](./download.md) | Download release assets |
| [`gh release edit`](./edit.md) | Edit a release |
| [`gh release upload`](./upload.md) | Upload assets to a release |
| [`gh release verify`](./verify.md) | Verify the attestation for a release |
| [`gh release verify-asset`](./verify-asset.md) | Verify that a given asset originated from a release |
| [`gh release view`](./view.md) | View information about a release |

## Flags

```text
-R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

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
