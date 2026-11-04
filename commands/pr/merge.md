# `gh pr merge`

> Merge a pull request on GitHub.

## Description

Without an argument, the pull request that belongs to the current branch
is selected.

When targeting a branch that requires a merge queue, no merge strategy is required.
If required checks have not yet passed, auto-merge will be enabled.
If required checks have passed, the pull request will be added to the merge queue.
To bypass a merge queue and merge directly, pass the `--admin` flag.

## Synopsis

```bash
gh pr merge [<number> | <url> | <branch>] [flags]
```

## Flags

```text
--admin                   Use administrator privileges to merge a pull request that does not meet requirements
  -A, --author-email text       Email text for merge commit author
      --auto                    Automatically merge only after necessary requirements are met
  -b, --body text               Body text for the merge commit
  -F, --body-file file          Read body text from file (use "-" to read from standard input)
  -d, --delete-branch           Delete the local and remote branch after merge
      --disable-auto            Disable auto-merge for this pull request
      --match-head-commit SHA   Commit SHA that the pull request head must match to allow merge
  -m, --merge                   Merge the commits with the base branch
  -r, --rebase                  Rebase the commits onto the base branch
  -s, --squash                  Squash the commits into one commit and merge it into the base branch
  -t, --subject text            Subject text for the merge commit
```

## Inherited Flags

```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

## AI Agent Automation Tips

- **Explicit Parameters**: In automation pipelines, explicitly pass flags like `--title`, `--body`, or `--body-file -` to bypass editor popups.
- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh pr`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
