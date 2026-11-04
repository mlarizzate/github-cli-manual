# `gh project link`

> Link a project to a repository or a team

## Synopsis

```bash
gh project link [<number>] [flags]
```

## Flags

```text
--owner string   Login of the owner. Use "@me" for the current user.
  -R, --repo string    The repository to be linked to this project
  -T, --team string    The team to be linked to this project
```

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
# Link monalisa's project 1 to her repository "my_repo"
  $ gh project link 1 --owner monalisa --repo my_repo
  
  # Link monalisa's organization's project 1 to her team "my_team"
  $ gh project link 1 --owner my_organization --team my_team
  
  # Link monalisa's project 1 to the repository of current directory if neither --repo nor --team is specified
  $ gh project link 1
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
