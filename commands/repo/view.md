# `gh repo view`

> Display the description and the README of a GitHub repository.

## Description

With no argument, the repository for the current directory is displayed.

With `--web`, open the repository in a web browser instead.

With `--branch`, view a specific branch of the repository.

For more information about output formatting flags, see `gh help formatting`.

## Synopsis

```bash
gh repo view [<repository>] [flags]
```

## Flags

```text
-b, --branch string     View a specific branch of the repository
  -q, --jq expression     Filter JSON output using a jq expression
      --json fields       Output JSON with the specified fields
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
  -w, --web               Open a repository in the browser
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
