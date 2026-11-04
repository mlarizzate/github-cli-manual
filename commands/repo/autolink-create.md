# `gh repo autolink create`

> Create a new autolink reference for a repository.

## Description

The `keyPrefix` argument specifies the prefix that will generate a link when it is appended by certain characters.

The `urlTemplate` argument specifies the target URL that will be generated when the keyPrefix is found, which
must contain `<num>` variable for the reference number.

By default, autolinks are alphanumeric with `--numeric` flag used to create a numeric autolink.

The `<num>` variable behavior differs depending on whether the autolink is alphanumeric or numeric:

- alphanumeric: matches `A-Z` (case insensitive), `0-9`, and `-`
- numeric: matches `0-9`

If the template contains multiple instances of `<num>`, only the first will be replaced.

## Synopsis

```bash
gh repo autolink create <keyPrefix> <urlTemplate> [flags]
```

## Aliases

- `gh repo autolink new`

## Flags

```text
-n, --numeric   Mark autolink as numeric
```

## Inherited Flags

```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

## Examples

```bash
# Create an alphanumeric autolink to example.com for the key prefix "TICKET-".
  # Generates https://example.com/TICKET?query=123abc from "TICKET-123abc".
  $ gh repo autolink create TICKET- "https://example.com/TICKET?query=<num>"
  
  # Create a numeric autolink to example.com for the key prefix "STORY-".
  # Generates https://example.com/STORY?id=123 from "STORY-123".
  $ gh repo autolink create STORY- "https://example.com/STORY?id=<num>" --numeric
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh repo`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
