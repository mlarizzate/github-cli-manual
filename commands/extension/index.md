# `gh extension`

> GitHub CLI extensions are repositories that provide additional gh commands.

## Description

The name of the extension repository must start with `gh-` and it must contain an
executable of the same name. All arguments passed to the `gh <extname>` invocation
will be forwarded to the `gh-<extname>` executable of the extension.

An extension cannot override any of the core gh commands. If an extension name conflicts
with a core gh command, you can use `gh extension exec <extname>`.

When an extension is executed, gh will check for new versions once every 24 hours and display
an upgrade notice. See `gh help environment` for information on disabling extension notices.

Extensions are not verified, signed, or endorsed by GitHub. When you install or upgrade
		an extension, you are trusting its publisher. It is your responsibility to review the
		source and provenance of any extension before use.

For the list of available extensions, see <https://github.com/topics/gh-extension>.

## Synopsis

```bash
gh extension [flags]
```

## Aliases

- `gh extensions, gh ext`
- `AVAILABLE COMMANDS`
- `browse:        Enter a UI for browsing, adding, and removing extensions`
- `create:        Create a new extension`
- `exec:          Execute an installed extension`
- `install:       Install a gh extension from a repository`
- `list:          List installed extension commands`
- `remove:        Remove an installed extension`
- `search:        Search extensions to the GitHub CLI`
- `upgrade:       Upgrade installed extensions`

## Subcommands

| Command | Description |
| :--- | :--- |
| [`gh extension browse`](./browse.md) | Enter a UI for browsing, adding, and removing extensions |
| [`gh extension create`](./create.md) | Create a new extension |
| [`gh extension exec`](./exec.md) | Execute an installed extension |
| [`gh extension install`](./install.md) | Install a gh extension from a repository |
| [`gh extension list`](./list.md) | List installed extension commands |
| [`gh extension remove`](./remove.md) | Remove an installed extension |
| [`gh extension search`](./search.md) | Search extensions to the GitHub CLI |
| [`gh extension upgrade`](./upgrade.md) | Upgrade installed extensions |

## Inherited Flags

```text
--help   Show help for command
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
