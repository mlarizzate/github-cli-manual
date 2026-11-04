# `gh repo list`

> List repositories owned by a user or organization.

## Description

Note that the list will only include repositories owned by the provided argument,
and the `--fork` or `--source` flags will not traverse ownership boundaries. For example,
when listing the forks in an organization, the output would not include those owned by individual users.

For more information about output formatting flags, see `gh help formatting`.

## Synopsis

```bash
gh repo list [<owner>] [flags]
```

## Aliases

- `gh repo ls`

## Flags

```text
--archived            Show only archived repositories
      --fork                Show only forks
  -q, --jq expression       Filter JSON output using a jq expression
      --json fields         Output JSON with the specified fields
  -l, --language string     Filter by primary coding language
  -L, --limit int           Maximum number of repositories to list (default 30)
      --no-archived         Omit archived repositories
      --source              Show only non-forks
  -t, --template string     Format JSON output using a Go template; see "gh help formatting"
      --topic strings       Filter by topic
      --visibility string   Filter by repository visibility: {public|private|internal}
```

## Inherited Flags

```text
--help   Show help for command

JSON FIELDS
  archivedAt, assignableUsers, codeOfConduct, contactLinks, createdAt,
  defaultBranchRef, deleteBranchOnMerge, description, diskUsage, forkCount,
  fundingLinks, hasDiscussionsEnabled, hasIssuesEnabled, hasProjectsEnabled,
  hasWikiEnabled, homepageUrl, id, isArchived, isBlankIssuesEnabled, isEmpty,
  isFork, isInOrganization, isMirror, isPrivate, isSecurityPolicyEnabled,
  isTemplate, isUserConfigurationRepository, issueTemplates, issues, labels,
  languages, latestRelease, licenseInfo, mentionableUsers, mergeCommitAllowed,
  milestones, mirrorUrl, name, nameWithOwner, openGraphImageUrl, owner, parent,
  primaryLanguage, projects, projectsV2, pullRequestTemplates, pullRequests,
  pushedAt, rebaseMergeAllowed, repositoryTopics, securityPolicyUrl,
  squashMergeAllowed, sshUrl, stargazerCount, templateRepository, updatedAt, url,
  usesCustomOpenGraphImage, viewerCanAdminister, viewerDefaultCommitEmail,
  viewerDefaultMergeMethod, viewerHasStarred, viewerPermission,
  viewerPossibleCommitEmails, viewerSubscription, visibility, watchers
```

## AI Agent Automation Tips

- **Machine-Readable Output**: Use `--json <fields>` and `--jq '<filter>'` for deterministic, parseable JSON output rather than text scraping.
- **Explicit Parameters**: In automation pipelines, explicitly pass flags like `--title`, `--body`, or `--body-file -` to bypass editor popups.
- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh repo`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
