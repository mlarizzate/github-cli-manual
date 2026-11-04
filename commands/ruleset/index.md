# `gh ruleset`

> Repository rulesets are a way to define a set of rules that apply to a repository.

## Description

These commands allow you to view information about them.

## Synopsis

```bash
gh ruleset <command> [flags]
```

## Aliases

- `gh rs`
- `AVAILABLE COMMANDS`
- `check:         View rules that would apply to a given branch`
- `list:          List rulesets for a repository or organization`
- `view:          View information about a ruleset`

## Subcommands

| Command | Description |
| :--- | :--- |
| [`gh ruleset check`](./check.md) | View rules that would apply to a given branch |
| [`gh ruleset list`](./list.md) | List rulesets for a repository or organization |
| [`gh ruleset view`](./view.md) | View information about a ruleset |

## Flags

```text
-R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
$ gh ruleset list
  $ gh ruleset view --repo OWNER/REPO --web
  $ gh ruleset check branch-name
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
