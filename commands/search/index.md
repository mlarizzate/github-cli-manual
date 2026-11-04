# `gh search`

> Search across all of GitHub.

## Description

Excluding search results that match a qualifier

In a browser, the GitHub search syntax supports excluding results that match a search qualifier
by prefixing the qualifier with a hyphen. For example, to search for issues that
do not have the label "bug", you would use `-label:bug` as a search qualifier.

`gh` supports this syntax in `gh search` as well, but it requires extra
command line arguments to avoid the hyphen being interpreted as a command line flag because it begins with a hyphen.

On Unix-like systems, you can use the `--` argument to indicate that
the arguments that follow are not a flag, but rather a query string. For example:

$ gh search issues -- "my-search-query -label:bug"

On PowerShell, you must use both the `--%` argument and the `--` argument to
produce the same effect. For example:

$ gh --% search issues -- "my search query -label:bug"

See the following for more information:
- GitHub search syntax: <https://docs.github.com/en/search-github/getting-started-with-searching-on-github/understanding-the-search-syntax#exclude-results-that-match-a-qualifier>
- The PowerShell stop parse flag `--%`: <https://learn.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_parsing?view=powershell-7.5#the-stop-parsing-token>
- The Unix-like `--` argument: <https://www.gnu.org/software/bash/manual/bash.html#Shell-Builtin-Commands-1>

## Synopsis

```bash
gh search <command> [flags]

AVAILABLE COMMANDS
  code:          Search within code
  commits:       Search for commits
  issues:        Search for issues
  prs:           Search for pull requests
  repos:         Search for repositories
```

## Subcommands

| Command | Description |
| :--- | :--- |
| [`gh search code`](./code.md) | Search within code |
| [`gh search commits`](./commits.md) | Search for commits |
| [`gh search issues`](./issues.md) | Search for issues |
| [`gh search prs`](./prs.md) | Search for pull requests |
| [`gh search repos`](./repos.md) | Search for repositories |

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
