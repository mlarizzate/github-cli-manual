# `gh codespace code`

> Open a codespace in Visual Studio Code

## Synopsis

```bash
gh codespace code [flags]
```

## Flags

```text
-c, --codespace string    Name of the codespace
      --insiders            Use the insiders version of Visual Studio Code
  -R, --repo string         Filter codespace selection by repository name (user/repo)
      --repo-owner string   Filter codespace selection by repository owner (username or org)
  -w, --web                 Use the web version of Visual Studio Code
```

## Inherited Flags

```text
--help   Show help for command
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh codespace`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
