# `gh alias set`

> Define a word that will expand to a full gh command when invoked.

## Description

The expansion may specify additional arguments and flags. If the expansion includes
positional placeholders such as `$1`, extra arguments that follow the alias will be
inserted appropriately. Otherwise, extra arguments will be appended to the expanded
command.

Use `-` as expansion argument to read the expansion string from standard input. This
is useful to avoid quoting issues when defining expansions.

If the expansion starts with `!` or if `--shell` was given, the expansion is a shell
expression that will be evaluated through the `sh` interpreter when the alias is
invoked. This allows for chaining multiple commands via piping and redirection.

## Synopsis

```bash
gh alias set <alias> <expansion> [flags]
```

## Flags

```text
--clobber   Overwrite existing aliases of the same name
  -s, --shell     Declare an alias to be passed through a shell interpreter
```

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
# Note: Command Prompt on Windows requires using double quotes for arguments
  $ gh alias set pv 'pr view'
  $ gh pv -w 123  #=> gh pr view -w 123
  
  $ gh alias set bugs 'issue list --label=bugs'
  $ gh bugs
  
  $ gh alias set homework 'issue list --assignee @me'
  $ gh homework
  
  $ gh alias set 'issue mine' 'issue list --mention @me'
  $ gh issue mine
  
  $ gh alias set epicsBy 'issue list --author="$1" --label="epic"'
  $ gh epicsBy vilmibm  #=> gh issue list --author="vilmibm" --label="epic"
  
  $ gh alias set --shell igrep 'gh issue list --label="$1" | grep "$2"'
  $ gh igrep epic foo  #=> gh issue list --label="epic" | grep "foo"
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh alias`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
