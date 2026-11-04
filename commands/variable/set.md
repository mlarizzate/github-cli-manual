# `gh variable set`

> Set a value for a variable on one of the following levels:

## Description

- repository (default): available to GitHub Actions runs or Dependabot in a repository
- environment: available to GitHub Actions runs for a deployment environment in a repository
- organization: available to GitHub Actions runs or Dependabot within an organization

Organization variable can optionally be restricted to only be available to
specific repositories.

## Synopsis

```bash
gh variable set <variable-name> [flags]
```

## Flags

```text
-b, --body string          The value for the variable (reads from standard input if not specified)
  -e, --env environment      Set deployment environment variable
  -f, --env-file file        Load variable names and values from a dotenv-formatted file
  -o, --org organization     Set organization variable
  -r, --repos repositories   List of repositories that can access an organization variable
  -v, --visibility string    Set visibility for an organization variable: {all|private|selected} (default "private")
```

## Inherited Flags

```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

## Examples

```bash
# Add variable value for the current repository in an interactive prompt
  $ gh variable set MYVARIABLE
  
  # Read variable value from an environment variable
  $ gh variable set MYVARIABLE --body "$ENV_VALUE"
  
  # Read variable value from a file
  $ gh variable set MYVARIABLE < myfile.txt
  
  # Set variable for a deployment environment in the current repository
  $ gh variable set MYVARIABLE --env myenvironment
  
  # Set organization-level variable visible to both public and private repositories
  $ gh variable set MYVARIABLE --org myOrg --visibility all
  
  # Set organization-level variable visible to specific repositories
  $ gh variable set MYVARIABLE --org myOrg --repos repo1,repo2,repo3
  
  # Set multiple variables imported from the ".env" file
  $ gh variable set -f .env
```

## AI Agent Automation Tips

- **Explicit Parameters**: In automation pipelines, explicitly pass flags like `--title`, `--body`, or `--body-file -` to bypass editor popups.
- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh variable`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
