# `gh ruleset list`

> List GitHub rulesets for a repository or organization.

## Description

If no options are provided, the current repository's rulesets are listed. You can query a different
repository's rulesets by using the `--repo` flag. You can also use the `--org` flag to list rulesets
configured for the provided organization.

Use the `--parents` flag to control whether rulesets configured at higher levels that also apply to the provided
repository or organization should be returned. The default is `true`.

Your access token must have the `admin:org` scope to use the `--org` flag, which can be granted by running `gh auth refresh -s admin:org`.

## Synopsis

```bash
gh ruleset list [flags]
```

## Aliases

- `gh rs ls, gh ruleset ls`

## Flags

```text
-L, --limit int    Maximum number of rulesets to list (default 30)
  -o, --org string   List organization-wide rulesets for the provided organization
  -p, --parents      Whether to include rulesets configured at higher levels that also apply (default true)
  -w, --web          Open the list of rulesets in the web browser
```

## Inherited Flags

```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

## Examples

```bash
# List rulesets in the current repository
  $ gh ruleset list
  
  # List rulesets in a different repository, including those configured at higher levels
  $ gh ruleset list --repo owner/repo --parents
  
  # List rulesets in an organization
  $ gh ruleset list --org org-name
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh ruleset`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
