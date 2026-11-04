# `gh issue artifact download`

> Download issue artifacts to files. Without artifact numbers, every artifact

## Description

on the issue is downloaded. Artifacts can also be named by their URLs, which
must all be on one issue. `<issue>` is an issue number or URL.

Each file is named `<number>-<name>`. Markdown documents end in `.md`, HTML
documents in `.html`, and links are saved as `.url` Internet Shortcut files.
If a file already exists, that artifact fails unless you use `--clobber` to
overwrite it or `--skip-existing` to skip it.

Use `--dir` to choose the directory to download files into, `--output` to
choose the path for a single artifact, or `--output -` to print its content.
Use `--version` with a single artifact to download an earlier version from
its edit history.

## Synopsis

```bash
gh issue artifact download {<issue> [<artifact-number>...] | <artifact-url>...} [flags]
```

## Flags

```text
--clobber          Overwrite existing files of the same name
  -D, --dir directory    The directory to download files into (default ".")
  -O, --output file      The file to write a single artifact to (use "-" to write to standard output)
      --skip-existing    Skip downloading when files of the same name exist
      --version number   Download the version with this number from the edit history
```

## Inherited Flags

```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

## Examples

```bash
# Download every artifact on issue 142
  $ gh issue artifact download 142
  
  # Download two artifacts into a folder
  $ gh issue artifact download 142 2 5 --dir notes
  
  # Print one artifact's content
  $ gh issue artifact download 142 2 --output -
  
  # Download an earlier version of one artifact
  $ gh issue artifact download 142 2 --version 5
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh issue`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
