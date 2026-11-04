# `gh repo license view`

> View a specific repository license by license key or SPDX ID.

## Description

Run `gh repo license list` to see available commonly used licenses. For even more licenses, visit <https://choosealicense.com/appendix>.

## Synopsis

```bash
gh repo license view {<license-key> | <spdx-id>} [flags]
```

## Flags

```text
-w, --web   Open https://choosealicense.com/ in the browser
```

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
# View the MIT license from SPDX ID
  $ gh repo license view MIT
  
  # View the MIT license from license key
  $ gh repo license view mit
  
  # View the GNU AGPL-3.0 license from SPDX ID
  $ gh repo license view AGPL-3.0
  
  # View the GNU AGPL-3.0 license from license key
  $ gh repo license view agpl-3.0
  
  # Create a LICENSE.md with the MIT license
  $ gh repo license view MIT > LICENSE.md
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh repo`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
