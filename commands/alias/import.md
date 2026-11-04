# `gh alias import`

> Import aliases from the contents of a YAML file.

## Description

Aliases should be defined as a map in YAML, where the keys represent aliases and
the values represent the corresponding expansions. An example file should look like
the following:

    bugs: issue list --label=bug
    igrep: '!gh issue list --label="$1" | grep "$2"'
    features: |-
        issue list
        --label=enhancement

Use `-` to read aliases (in YAML format) from standard input.

The output from `gh alias list` can be used to produce a YAML file
containing your aliases, which you can use to import them from one machine to
another. Run `gh help alias list` to learn more.

## Synopsis

```bash
gh alias import [<filename> | -] [flags]
```

## Flags

```text
--clobber   Overwrite existing aliases of the same name
```

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
# Import aliases from a file
  $ gh alias import aliases.yml
  
  # Import aliases from standard input
  $ gh alias import -
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh alias`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
