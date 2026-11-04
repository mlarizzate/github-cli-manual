# `gh project unlink`

> Unlink a project from a repository or a team

## Synopsis

```bash
gh project unlink [<number>] [flags]
```

## Flags

```text
--owner string   Login of the owner. Use "@me" for the current user.
  -R, --repo string    The repository to be unlinked from this project
  -T, --team string    The team to be unlinked from this project
```

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
# Unlink monalisa's project 1 from her repository "my_repo"
  $ gh project unlink 1 --owner monalisa --repo my_repo
  
  # Unlink monalisa's organization's project 1 from her team "my_team"
  $ gh project unlink 1 --owner my_organization --team my_team
  
  # Unlink monalisa's project 1 from the repository of current directory if neither --repo nor --team is specified
  $ gh project unlink 1
```

## AI Agent Automation Tips

- **Explicit Parameters**: In automation pipelines, explicitly pass flags like `--title`, `--body`, or `--body-file -` to bypass editor popups.
- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh project`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
