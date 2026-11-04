# `gh release download`

> Download assets from a GitHub release.

## Description

Without an explicit tag name argument, assets are downloaded from the
latest release in the project. In this case, `--pattern` or `--archive`
is required.

## Synopsis

```bash
gh release download [<tag>] [flags]
```

## Flags

```text
--allow-escape-sequences   Allow printing terminal escape sequences when writing an asset to standard output
  -A, --archive format           Download the source code archive in the specified format (zip or tar.gz)
      --clobber                  Overwrite existing files of the same name
  -D, --dir directory            The directory to download files into (default ".")
  -O, --output file              The file to write a single asset to (use "-" to write to standard output)
  -p, --pattern stringArray      Download only assets that match a glob pattern
      --skip-existing            Skip downloading when files of the same name exist
```

## Inherited Flags

```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

## Examples

```bash
# Download all assets from a specific release
  $ gh release download v1.2.3
  
  # Download only Debian packages for the latest release
  $ gh release download --pattern '*.deb'
  
  # Specify multiple file patterns
  $ gh release download -p '*.deb' -p '*.rpm'
  
  # Download the archive of the source code for a release
  $ gh release download v1.2.3 --archive=zip
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh release`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
