# `gh codespace cp`

> The `cp` command copies files between the local and remote file systems.

## Description

As with the UNIX `cp` command, the first argument specifies the source and the last
specifies the destination; additional sources may be specified after the first,
if the destination is a directory.

The `--recursive` flag is required if any source is a directory.

A `remote:` prefix on any file name argument indicates that it refers to
the file system of the remote (Codespace) machine. It is resolved relative
to the home directory of the remote user.

By default, remote file names are interpreted literally. With the `--expand` flag,
each such argument is treated in the manner of `scp`, as a Bash expression to
be evaluated on the remote machine, subject to expansion of tildes, braces, globs,
environment variables, and backticks. For security, do not use this flag with arguments
provided by untrusted users; see <https://lwn.net/Articles/835962/> for discussion.

By default, the `cp` command will create a public/private ssh key pair to authenticate with
the codespace inside the `~/.ssh directory`.

## Synopsis

```bash
gh codespace cp [-e] [-r] [-- [<scp flags>...]] <sources>... <dest>
```

## Flags

```text
-c, --codespace string    Name of the codespace
  -e, --expand              Expand remote file names on remote shell
  -p, --profile string      Name of the SSH profile to use
  -r, --recursive           Recursively copy directories
  -R, --repo string         Filter codespace selection by repository name (user/repo)
      --repo-owner string   Filter codespace selection by repository owner (username or org)
```

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
$ gh codespace cp -e README.md 'remote:/workspaces/$RepositoryName/'
  $ gh codespace cp -e 'remote:~/*.go' ./gofiles/
  $ gh codespace cp -e 'remote:/workspaces/myproj/go.{mod,sum}' ./gofiles/
  $ gh codespace cp -e -- -F ~/.ssh/codespaces_config 'remote:~/*.go' ./gofiles/
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh codespace`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
