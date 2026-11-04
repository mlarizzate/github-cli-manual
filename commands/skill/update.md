# `gh skill update`

> Checks installed skills for available updates by comparing the local

## Description

tree SHA (from `SKILL.md` frontmatter) against the remote repository.

Scans all known agent host directories (including Copilot, Claude, Cursor,
Gemini, Antigravity, Grok, and others) in both project and user scope automatically.

Without arguments, checks all installed skills. With skill names,
checks only those specific skills.

Pinned skills (installed with `--pin`) are skipped with a notice.
Use `--unpin` to clear the pinned version and include those skills
in the update.

Skills without GitHub metadata (e.g. installed manually or by another
tool) are prompted for their source repository in interactive mode.
With `--all` or in non-interactive mode, they are skipped with a notice.
The update re-downloads the skill with metadata injected, so future
updates work automatically.

With `--force`, re-downloads skills even when the remote version matches
the local tree SHA. This overwrites locally modified skill files with
their original content, but does not remove extra files added locally.

In interactive mode, shows which skills have updates and asks for
confirmation before proceeding. With `--all`, updates without prompting.
With `--dry-run`, reports available updates without modifying any files.

## Synopsis

```bash
gh skill update [<skill>...] [flags]
```

## Flags

```text
--all          Update all skills without prompting
  --dir string   Scan a custom directory for installed skills
  --dry-run      Report available updates without modifying files
  --force        Re-download even if already up to date
  --unpin        Clear pinned version and include pinned skills in update
```

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
# Check and update all skills interactively
  $ gh skill update
  
  # Update specific skills
  $ gh skill update mcp-cli git-commit
  
  # Update all without prompting
  $ gh skill update --all
  
  # Re-download all skills (restore locally modified files)
  $ gh skill update --force --all
  
  # Check for updates without applying (read-only)
  $ gh skill update --dry-run
  
  # Unpin skills and update them to latest
  $ gh skill update --unpin
```

## AI Agent Automation Tips

- **Non-Interactive Execution**: Always pass affirmative flags (e.g., `--yes` or `--confirm`) to prevent hanging in interactive prompts.
- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh skill`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
