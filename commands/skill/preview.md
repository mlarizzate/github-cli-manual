# `gh skill preview`

> Render a skill's `SKILL.md` content in the terminal. This fetches the

## Description

skill file from the repository and displays it using the configured
pager, without installing anything.

A file tree is shown first, followed by the rendered `SKILL.md` content.
When running interactively and the skill contains additional files
(scripts, references, etc.), a file picker lets you browse them
individually.

When run with only a repository argument, lists available skills and
prompts for selection.

The skill argument can be a name, a namespaced name (`author/skill`),
or an exact path within the repository (`skills/author/skill`,
`packages/agent-skills/code-review`, or any `.../SKILL.md` path).
Namespaced names with one slash are matched by name. Use a `SKILL.md`
suffix to force a one-directory path outside the standard conventions.

To preview a specific version of the skill, append `@VERSION` to the
skill name. The version is resolved as a git tag, branch, or commit SHA.

## Synopsis

```bash
gh skill preview <repository> [<skill>] [flags]
```

## Aliases

- `gh skill show, gh skills show`

## Flags

```text
--allow-hidden-dirs   Include skills in hidden directories (e.g. .claude/skills/, .agents/skills/)
```

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
# Preview a specific skill
  $ gh skill preview github/awesome-copilot documentation-writer
  
  # Preview a skill at a specific version
  $ gh skill preview github/awesome-copilot documentation-writer@v1.2.0
  
  # Preview a skill at a specific commit SHA
  $ gh skill preview github/awesome-copilot documentation-writer@abc123def456
  
  # Preview from a non-standard nested path (efficient, skips full discovery)
  $ gh skill preview monalisa/skills-repo packages/agent-skills/code-review
  
  # Browse and preview interactively
  $ gh skill preview github/awesome-copilot
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh skill`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
