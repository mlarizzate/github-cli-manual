# `gh attestation download`

> ### NOTE: This feature is currently in public preview, and subject to change.

## Description

Download attestations associated with an artifact for offline use.

The command requires either:
* a file path to an artifact, or
* a container image URI (e.g. `oci://<image-uri>`)
  * (note that if you provide an OCI URL, you must already be authenticated with
its container registry)

In addition, the command requires either:
* the `--repo` flag (e.g. --repo github/example).
* the `--owner` flag (e.g. --owner github), or

The `--repo` flag value must match the name of the GitHub repository
that the artifact is linked with.

The `--owner` flag value must match the name of the GitHub organization
that the artifact's linked repository belongs to.

Any associated bundle(s) will be written to a file in the
current directory named after the artifact's digest. For example, if the
digest is "sha256:1234", the file will be named "sha256:1234.jsonl".

Colons are special characters on Windows and cannot be used in
file names. To accommodate, a dash will be used to separate the algorithm
from the digest in the attestations file name. For example, if the digest
is "sha256:1234", the file will be named "sha256-1234.jsonl".

## Synopsis

```bash
gh attestation download [<file-path> | oci://<image-uri>] [--owner | --repo] [flags]
```

## Flags

```text
-d, --digest-alg string       The algorithm used to compute a digest of the artifact: {sha256|sha512} (default "sha256")
      --hostname string         Configure host to use
  -L, --limit int               Maximum number of attestations to fetch (default 30)
  -o, --owner string            GitHub organization to scope attestation lookup by
      --predicate-type string   Filter attestations by provided predicate type
  -R, --repo string             Repository name in the format <owner>/<repo>
```

## Inherited Flags

```text
--help   Show help for command
```

## Examples

```bash
# Download attestations for a local artifact linked with an organization
  $ gh attestation download example.bin -o github
  
  # Download attestations for a local artifact linked with a repository
  $ gh attestation download example.bin -R github/example
  
  # Download attestations for an OCI image linked with an organization
  $ gh attestation download oci://example.com/foo/bar:latest -o github
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
