# `gh workflow run`

> Create a `workflow_dispatch` event for a given workflow.

## Description

This command will trigger GitHub Actions to run a given workflow file. The given workflow file must
support an `on.workflow_dispatch` trigger in order to be run in this way.

If the workflow file supports inputs, they can be specified in a few ways:

- Interactively
- Via `-f/--raw-field` or `-F/--field` flags
- As JSON, via standard input

The created workflow run URL will be returned if available.

## Synopsis

```bash
gh workflow run [<workflow-id> | <workflow-name>] [flags]
```

## Flags

```text
-F, --field key=value       Add a string parameter in key=value format, respecting @ syntax (see "gh help api").
      --json                  Read workflow inputs as JSON via STDIN
  -f, --raw-field key=value   Add a string parameter in key=value format
  -r, --ref string            Branch or tag name which contains the version of the workflow file you'd like to run
```

## Inherited Flags

```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

## Examples

```bash
# Have gh prompt you for what workflow you'd like to run and interactively collect inputs
  $ gh workflow run
  
  # Run the workflow file 'triage.yml' at the remote's default branch
  $ gh workflow run triage.yml
  
  # Run the workflow file 'triage.yml' at a specified ref
  $ gh workflow run triage.yml --ref my-branch
  
  # Run the workflow file 'triage.yml' with command line inputs
  $ gh workflow run triage.yml -f name=scully -f greeting=hello
  
  # Run the workflow file 'triage.yml' with JSON via standard input
  $ echo '{"name":"scully", "greeting":"hello"}' | gh workflow run triage.yml --json
```

## AI Agent Automation Tips

- **Machine-Readable Output**: Use `--json <fields>` and `--jq '<filter>'` for deterministic, parseable JSON output rather than text scraping.
- **Explicit Parameters**: In automation pipelines, explicitly pass flags like `--title`, `--body`, or `--body-file -` to bypass editor popups.
- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh workflow`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
