# `gh repo read-dir`

> List the contents of a directory in a GitHub repository without cloning it.

## Description

This command is in preview and subject to change without notice.

By default, the directory is listed from the default branch. Use the `--ref` flag to
list from a specific branch, tag, or commit. When no path is given, the repository root
is listed.

For more information about output formatting flags, see `gh help formatting`.

## Synopsis

```bash
gh repo read-dir [<path>] [flags]
```

## Flags

```text
-q, --jq expression            Filter JSON output using a jq expression
      --json fields              Output JSON with the specified fields
      --ref string               The branch, tag, or commit to list from
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
  -t, --template string          Format JSON output using a Go template; see "gh help formatting"
```

## Inherited Flags

```text
--help   Show help for command

JSON FIELDS
  gitSHA, gitType, mode, modeOctal, name, nameRaw, path, pathRaw, size, submodule,
  type
```

## Examples

```bash
# List the root of the default branch
  $ gh repo read-dir --repo cli/cli
  
  # List a subdirectory
  $ gh repo read-dir docs --repo cli/cli
  
  # List a directory at a specific ref
  $ gh repo read-dir docs --repo cli/cli --ref v2.50.0
  
  # Print selected fields as JSON
  $ gh repo read-dir docs --repo cli/cli --json name,path,type,size
```

## AI Agent Automation Tips

- **Machine-Readable Output**: Use `--json <fields>` and `--jq '<filter>'` for deterministic, parseable JSON output rather than text scraping.
- **Explicit Parameters**: In automation pipelines, explicitly pass flags like `--title`, `--body`, or `--body-file -` to bypass editor popups.
- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh repo`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
