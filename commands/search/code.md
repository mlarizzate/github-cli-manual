# `gh search code`

> Search within code in GitHub repositories.

## Description

The search syntax is documented at:
<https://docs.github.com/search-github/searching-on-github/searching-code>

Note that these search results are powered by what is now a legacy GitHub code search engine.
The results might not match what is seen on `github.com`, and new features like regex search
are not yet available via the GitHub API.

For more information on handling search queries containing a hyphen, run `gh search --help`.

For more information about output formatting flags, see `gh help formatting`.

## Synopsis

```bash
gh search code <query> [flags]
```

## Flags

```text
--extension string   Filter on file extension
      --filename string    Filter on filename
  -q, --jq expression      Filter JSON output using a jq expression
      --json fields        Output JSON with the specified fields
      --language string    Filter results by language
  -L, --limit int          Maximum number of code results to fetch (default 30)
      --match strings      Restrict search to file contents or file path: {file|path}
      --owner strings      Filter on owner
  -R, --repo OWNER/REPO    Filter on repository, in OWNER/REPO format
      --size string        Filter on size range, in kilobytes
  -t, --template string    Format JSON output using a Go template; see "gh help formatting"
  -w, --web                Open the search query in the web browser
```

## Inherited Flags

```text
--help   Show help for command

JSON FIELDS
  path, repository, sha, textMatches, url
```

## Examples

```bash
# Search code matching "react" and "lifecycle"
  $ gh search code react lifecycle
  
  # Search code matching "error handling"
  $ gh search code "error handling"
  
  # Search code using raw search qualifiers as separate arguments
  $ gh search code panic path:pkg language:go
  
  # Search code matching "deque" in Python files
  $ gh search code deque --language=python
  
  # Search code matching "cli" in repositories owned by microsoft organization
  $ gh search code cli --owner=microsoft
  
  # Search code matching "panic" in the GitHub CLI repository
  $ gh search code panic --repo cli/cli
  
  # Search code matching keyword "lint" in package.json files
  $ gh search code lint --filename package.json
```

## AI Agent Automation Tips

- **Machine-Readable Output**: Use `--json <fields>` and `--jq '<filter>'` for deterministic, parseable JSON output rather than text scraping.
- **Explicit Parameters**: In automation pipelines, explicitly pass flags like `--title`, `--body`, or `--body-file -` to bypass editor popups.
- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh search`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
