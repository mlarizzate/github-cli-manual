# `gh skill search`

> Search across all public GitHub repositories for skills matching a keyword.

## Description

Uses the GitHub Code Search API to find `SKILL.md` files whose name or
description matches the query term.

Results are ranked by relevance: skills whose name contains the query
term appear first.

Use `--owner` to scope results to a specific GitHub user or organization.

In interactive mode, you can select skills from the results to install directly.

For more information about output formatting flags, see `gh help formatting`.

## Synopsis

```bash
gh skill search <query> [flags]
```

## Flags

```text
-q, --jq expression     Filter JSON output using a jq expression
      --json fields       Output JSON with the specified fields
  -L, --limit int         Maximum number of results per page (default 15)
      --owner string      Filter results to a specific GitHub user or organization
      --page int          Page number of results to fetch (default 1)
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
```

## Inherited Flags

```text
--help   Show help for command

JSON FIELDS
  description, namespace, path, repo, skillName, stars
```

## Examples

```bash
# Search for skills related to terraform
  $ gh skill search terraform
  
  # Search for skills from a specific owner
  $ gh skill search terraform --owner hashicorp
  
  # View the second page of results
  $ gh skill search terraform --page 2
  
  # Limit results to 5
  $ gh skill search terraform --limit 5
```

## AI Agent Automation Tips

- **Machine-Readable Output**: Use `--json <fields>` and `--jq '<filter>'` for deterministic, parseable JSON output rather than text scraping.
- **Explicit Parameters**: In automation pipelines, explicitly pass flags like `--title`, `--body`, or `--body-file -` to bypass editor popups.
- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh skill`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
