# `gh ruleset view`

> View information about a GitHub ruleset.

## Description

If no ID is provided, an interactive prompt will be used to choose
the ruleset to view.

Use the `--parents` flag to control whether rulesets configured at higher
levels that also apply to the provided repository or organization should
be returned. The default is `true`.

## Synopsis

```bash
gh ruleset view [<ruleset-id>] [flags]
```

## Flags

```text
-o, --org string   Organization name if the provided ID is an organization-level ruleset
  -p, --parents      Whether to include rulesets configured at higher levels that also apply (default true)
  -w, --web          Open the ruleset in the browser
```

## Inherited Flags

```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

## Examples

```bash
# Interactively choose a ruleset to view from all rulesets that apply to the current repository
  $ gh ruleset view
  
  # Interactively choose a ruleset to view from only rulesets configured in the current repository
  $ gh ruleset view --parents=false
  
  # View a ruleset configured in the current repository or any of its parents
  $ gh ruleset view 43
  
  # View a ruleset configured in a different repository or any of its parents
  $ gh ruleset view 23 --repo owner/repo
  
  # View an organization-level ruleset
  $ gh ruleset view 23 --org my-org
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh ruleset`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
