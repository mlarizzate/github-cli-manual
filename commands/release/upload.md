# `gh release upload`

> Upload asset files to a GitHub Release.

## Description

To define a display label for an asset, append text starting with `#` after the
file name.

When using `--clobber`, existing assets are deleted before new assets are uploaded.
If the upload fails, the original assets will be lost.

## Synopsis

```bash
gh release upload <tag> <files>... [flags]
```

## Flags

```text
--clobber   Delete and re-upload existing assets of the same name
```

## Inherited Flags

```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh release`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
