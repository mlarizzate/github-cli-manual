# `gh attestation trusted-root`

> Output contents for a trusted_root.jsonl file, likely for offline verification.

## Description

When using `gh attestation verify`, if your machine is on the internet,
this will happen automatically. But to do offline verification, you need to
supply a trusted root file with `--custom-trusted-root`; this command
will help you fetch a `trusted_root.jsonl` file for that purpose.

You can call this command without any flags to get a trusted root file covering
the Sigstore Public Good Instance as well as GitHub's Sigstore instance.

Otherwise you can use `--tuf-url` to specify the URL of a custom TUF
repository mirror, and `--tuf-root` should be the path to the
`root.json` file that you securely obtained out-of-band.

If you just want to verify the integrity of your local TUF repository, and don't
want the contents of a trusted_root.jsonl file, use `--verify-only`.

## Synopsis

```bash
gh attestation trusted-root [--tuf-url <url> --tuf-root <file-path>] [--verify-only] [flags]
```

## Flags

```text
--hostname string   Configure host to use
  --tuf-root string   Path to the TUF root.json file on disk
  --tuf-url string    URL to the TUF repository mirror
  --verify-only       Don't output trusted_root.jsonl contents
```

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
# Get a trusted_root.jsonl for both Sigstore Public Good and GitHub's instance
  $ gh attestation trusted-root
```

## AI Agent Automation Tips

- **Explicit Parameters**: In automation pipelines, explicitly pass flags like `--title`, `--body`, or `--body-file -` to bypass editor popups.
- **Repository Context**: Supply `-R OWNER/REPO` (or `GH_REPO=OWNER/REPO`) if executing outside a cloned git working directory.
- **Authentication**: Ensure `GH_TOKEN` or `GITHUB_TOKEN` is set in headless environments.

## See Also

- [Index](../../README.md)
- [`gh attestation`](./index.md)
- [Formatting Guide](../../topics/formatting.md)
- [Environment Variables](../../topics/environment.md)
