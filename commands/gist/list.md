# `gh gist list`

> List gists from your user account.

## Description

You can use a regular expression to filter the description, file names,
or even the content of files in the gist using `--filter`.

For supported regular expression syntax, see <https://pkg.go.dev/regexp/syntax>.

Use `--include-content` to include content of files, noting that
this will be slower and increase the rate limit used. Instead of printing a table,
code will be printed with highlights similar to `gh search code`:

	{{gist ID}} {{file name}}
	    {{description}}
	        {{matching lines from content}}

No highlights or other color is printed when output is redirected.

## Synopsis

```bash
gh gist list [flags]
```

## Aliases

- `gh gist ls`

## Flags

```text
--filter expression   Filter gists using a regular expression
      --include-content     Include gists' file content when filtering
  -L, --limit int           Maximum number of gists to fetch (default 10)
      --public              Show only public gists
      --secret              Show only secret gists
```

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
# List all secret gists from your user account
  $ gh gist list --secret
  
  # Find all gists from your user account mentioning "octo" anywhere
  $ gh gist list --filter octo --include-content
```

## AI Agent Automation Tips

- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh gist`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
