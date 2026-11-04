# `gh auth refresh`

> Expand or fix the permission scopes for stored credentials for active account.

## Description

The `--scopes` flag accepts a comma separated list of scopes you want
your gh credentials to have. If no scopes are provided, the command
maintains previously added scopes.

The `--remove-scopes` flag accepts a comma separated list of scopes you
want to remove from your gh credentials. Scope removal is idempotent.
The minimum set of scopes (`repo`, `read:org`, and `gist`) cannot be removed.

The `--reset-scopes` flag resets the scopes for your gh credentials to
the default set of scopes for your auth flow.

If you have multiple accounts in `gh auth status` and want to refresh the credentials for an
inactive account, you will have to use `gh auth switch` to that account first before using
this command, and then switch back when you are done.

Use `--expiring` to prefer expiring credentials that gh refreshes automatically, or
`--expiring=false` to prefer a non-expiring token. This is a preference, not a guarantee:
whether expiring tokens are issued depends on the host and the OAuth app configuration. A host
without support issues a non-expiring token instead, and a host configured for them may issue
expiring tokens even without the flag. Without the flag, refresh keeps the current token's kind,
so an expiring token stays expiring and a non-expiring token stays non-expiring.
When using expiring credentials for git operations, git 2.46 or newer is recommended so
gh can mark the token as non-cacheable; with older git a credential caching helper may store
and reuse an expired token.

For more information on OAuth scopes, see
<https://docs.github.com/en/developers/apps/building-oauth-apps/scopes-for-oauth-apps/>.

## Synopsis

```bash
gh auth refresh [flags]
```

## Flags

```text
-c, --clipboard               Copy one-time OAuth device code to clipboard
      --expiring                Prefer expiring credentials that gh refreshes automatically, if the host supports them
  -h, --hostname string         The GitHub host to use for authentication
      --insecure-storage        Save authentication credentials in plain text instead of credential store
  -r, --remove-scopes strings   Authentication scopes to remove from gh
      --reset-scopes            Reset authentication scopes to the default minimum set of scopes
  -s, --scopes strings          Additional authentication scopes for gh to have
```

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
# Open a browser to add write:org and read:public_key scopes
  $ gh auth refresh --scopes write:org,read:public_key
  
  # Open a browser to ensure your authentication credentials have the correct minimum scopes
  $ gh auth refresh
  
  # Open a browser to idempotently remove the delete_repo scope
  $ gh auth refresh --remove-scopes delete_repo
  
  # Open a browser to re-authenticate with the default minimum scopes
  $ gh auth refresh --reset-scopes
  
  # Open a browser to re-authenticate and copy one-time OAuth code to clipboard
  $ gh auth refresh --clipboard
```

## AI Agent Automation Tips

- **Explicit Parameters**: In automation pipelines, explicitly pass flags like `--title`, `--body`, or `--body-file -` to bypass editor popups.
- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh auth`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
