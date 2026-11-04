<div align="center">

# 🚀 GitHub CLI (`gh`) Offline Manual & Cheat Sheet
### *The Ultimate Headless Reference for AI Agents, LLM Contexts & DevOps Engineers*

[![GitHub CLI](https://img.shields.io/badge/GitHub%20CLI-v2.x+-2ea44f?logo=github&logoColor=white)](https://cli.github.com/)
[![LLM & Agent Ready](https://img.shields.io/badge/Optimized%20for-AI%20Agents%20%7C%20RAG-8A2BE2?logo=openai&logoColor=white)](#-ai-agent-automation--headless-best-practices)
[![Offline Docs](https://img.shields.io/badge/Docs-100%25%20Offline%20Markdown-blue)](#-quick-navigation)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](#-contributing)

<p align="center">
  <b>A comprehensive, offline-first manual and command cheat sheet for the official GitHub CLI (<code>gh</code>).</b><br>
  Structured specifically for autonomous AI agents, LLM prompts, headless CI/CD runners, and developers seeking fast, zero-latency command lookups.
</p>

[Quick Start](#-quick-start-in-60-seconds) •
[Agent Best Practices](#-ai-agent-automation--headless-best-practices) •
[Command Directory](#-command-directory--matrix) •
[Topics & Guides](#-guides--deep-dive-topics) •
[Single-File Manual](./FULL_REFERENCE.md)

---

</div>

## 📌 Table of Contents

- [Why This Manual?](#-why-this-manual)
- [Quick Start in 60 Seconds](#-quick-start-in-60-seconds)
- [Quick Navigation](#-quick-navigation)
- [AI Agent Automation & Headless Best Practices](#-ai-agent-automation--headless-best-practices)
  - [1. Deterministic JSON Output (`--json` & `--jq`)](#1-deterministic-json-output---json----jq)
  - [2. Preventing Interactive Prompts & Hangs](#2-preventing-interactive-prompts--hangs)
  - [3. Non-Interactive Authentication](#3-non-interactive-authentication)
  - [4. Querying Repositories Without `git clone`](#4-querying-repositories-without-git-clone)
  - [5. Pipelining & Stdin Support (`-F -`)](#5-pipelining--stdin-support---f--)
  - [6. Integrating with LLM Prompts & RAG Systems](#6-integrating-with-llm-prompts--rag-systems)
- [Command Directory & Matrix](#-command-directory--matrix)
  - [Core Workflows (PRs, Issues, Repos)](#core-workflows)
  - [GitHub Actions & CI/CD](#github-actions--cicd)
  - [Configuration, Secrets & Environment](#configuration-secrets--environment)
  - [Platform, Search & Developer Capabilities](#platform-search--developer-capabilities)
- [Guides & Deep-Dive Topics](#-guides--deep-dive-topics)
- [Using with AI Coding Tools (Cursor, Claude, Copilot, LangChain)](#-using-with-ai-coding-tools)
- [Contributing](#-contributing)
- [License](#-license)

---

## 💡 Why This Manual?

While the official documentation is online, modern software engineering requires **offline availability**, **low-token documentation**, and **automation-first patterns**:

| Feature | Standard `gh --help` / Web Docs | This Repository |
| :--- | :--- | :--- |
| **Offline & Local** | Requires internet or noisy man pages | 100% clean Markdown, searchable locally with `grep`/`ripgrep` |
| **LLM & Agent Ready** | High token bloat, interactive prompts | Lean, prompt-friendly snippets, headless flags, and single-file RAG reference |
| **Automation First** | Emphasizes interactive terminal usage | Built for zero-prompt scripting, CI/CD pipelines, and autonomous agents |
| **Output Parsing** | Plain text output by default | Production `--json` + `--jq` recipes for machine consumers |
| **Scope Coverage** | Fragmented across web pages | Core commands + preview features (`agent-task`, `attestation`, `skill`) |

---

## ⚡ Quick Start in 60 Seconds

Common high-frequency commands with headless best practices:

```bash
# 1. Non-interactive PR Creation from commits
gh pr create --fill --assignee "@me"

# 2. Extract deterministic JSON without scraping terminal output
gh pr list --state open --json number,title,author --jq '.[] | {number: .number, title: .title, author: .author.login}'

# 3. Check status of latest CI/CD workflow run
gh run list --limit 1 --json status,conclusion,url --jq '.[0]'

# 4. View an issue across any repository without cloning
gh issue view 42 -R owner/repo --json title,body,comments

# 5. Set an Actions repository secret non-interactively
echo "SECRET_VALUE" | gh secret set MY_SECRET -R owner/repo
```

---

## 📖 Quick Navigation

* 📖 **[Consolidated Single-File Reference](./FULL_REFERENCE.md)**: The entire 300KB+ manual compiled into one file. Ideal for uploading to LLM context windows (Cursor, Claude, ChatGPT) or global indexing.
* 📑 **[Alphabetical Command Index](./INDEX.md)**: Instant lookup for all 40+ commands and subcommands.
* ⚙️ **[Environment Variables Reference](./topics/environment.md)**: Master list of authentication tokens, hosts, and behavior toggles.
* 📊 **[JSON Formatting & jq Guide](./topics/formatting.md)**: Deep dive into `--json`, `--jq`, and Go formatting templates.
* 🚦 **[Exit Codes & Troubleshooting](./topics/exit-codes.md)**: Complete guide to CLI return codes and handling errors.
* 🚀 **[GitHub Actions Integration](./topics/actions.md)**: Using `gh` in workflows with `GITHUB_TOKEN`.

---

## 🤖 AI Agent Automation & Headless Best Practices

When integrating `gh` into autonomous coding agents (Antigravity, AutoGPT, CrewAI, LangChain, Cursor, Windsurf) or CI/CD pipelines, adhere to these strict rules:

### 1. Deterministic JSON Output (`--json` & `--jq`)
> [!IMPORTANT]
> **Never scrape plain text terminal output.** Tables and human-readable formatting change across versions. Always request structured fields with `--json` and filter with `--jq`:

```bash
# Get open PRs as clean JSON objects
gh pr list --state open --json number,title,headRefName,isDraft --jq '.[]'

# Query latest deployment or run conclusion
gh run list --limit 1 --json databaseId,status,conclusion --jq '.[0] | {id: .databaseId, result: .conclusion}'
```

### 2. Preventing Interactive Prompts & Hangs
By default, the GitHub CLI opens interactive selection menus or pauses execution if required flags are missing. In headless environments, this **causes agent processes to hang indefinitely**.

Prevent hangs using:
- **Environment Variable**: Export `GH_PROMPT_DISABLED=1` in your container or agent runtime.
- **Explicit Flags**: Always supply required parameters (e.g. `--title`, `--body`, `--repo`).
- **Confirmation Flags**: Add `--yes`, `--confirm`, or `--force` for destructive operations.
- **Automatic Fills**: Use `gh pr create --fill` to populate titles/bodies directly from git commit messages.

### 3. Non-Interactive Authentication
Authenticate headless runners without launching a browser or OAuth device flow:

```bash
# GitHub.com Personal Access Token (PAT)
export GH_TOKEN="ghp_yourTokenHere"

# GitHub Enterprise Server
export GH_ENTERPRISE_TOKEN="ghp_yourEnterpriseToken"
export GH_HOST="github.mycompany.com"
```

### 4. Querying Repositories Without `git clone`
AI agents often operate across multiple repositories without having local clones. Target remote repositories directly via the `-R` / `--repo` flag or the `GH_REPO` variable:

```bash
# Fetch issue details without cloning
gh issue view 128 -R facebook/react --json title,body

# Target all commands in a session to a remote repository
export GH_REPO="cli/cli"
gh pr list --limit 5
```

### 5. Pipelining & Stdin Support (`-F -`)
For multiline markdown comments, release notes, or dynamic agent-generated summaries, pass data through `stdin` using `-F -` or `--body-file -`:

```bash
# Create an issue with an agent-generated markdown report
cat << 'EOF' | gh issue create -R owner/repo -t "Bug: Memory Leak in Worker" -F -
### Agent Diagnostic Report
- **Failure:** Process terminated unexpectedly
- **Memory trace:** Peak consumption 1.4GB
- **Suggested Fix:** Add garbage collection trigger
EOF
```

### 6. Integrating with LLM Prompts & RAG Systems
- **For Single-Turn Prompts**: Pass the specific markdown file from `commands/<group>/<subcommand>.md` into your LLM prompt context to keep token consumption minimal (~500 tokens).
- **For RAG & Embeddings**: Chunk files by command level or ingest `FULL_REFERENCE.md` directly.
- **For Agent Tool Calling**: Wrap `gh <command> --json <fields>` inside custom tool definitions (MCP servers, Python subprocess, or shell tools).

---

## 🗺️ Command Directory & Matrix

### Core Workflows
| Command Group | Description | Key Subcommands |
| :--- | :--- | :--- |
| **[`auth`](./commands/auth/index.md)** | Authenticate `gh` and `git` | [`login`](./commands/auth/login.md), [`logout`](./commands/auth/logout.md), [`status`](./commands/auth/status.md), [`token`](./commands/auth/token.md), [`refresh`](./commands/auth/refresh.md), [`setup-git`](./commands/auth/setup-git.md), [`switch`](./commands/auth/switch.md) |
| **[`pr`](./commands/pr/index.md)** | Pull request lifecycle management | [`create`](./commands/pr/create.md), [`checkout`](./commands/pr/checkout.md), [`checks`](./commands/pr/checks.md), [`diff`](./commands/pr/diff.md), [`merge`](./commands/pr/merge.md), [`review`](./commands/pr/review.md), [`status`](./commands/pr/status.md), [`view`](./commands/pr/view.md), [`list`](./commands/pr/list.md) |
| **[`issue`](./commands/issue/index.md)** | Issues & project task tracking | [`create`](./commands/issue/create.md), [`view`](./commands/issue/view.md), [`list`](./commands/issue/list.md), [`close`](./commands/issue/close.md), [`comment`](./commands/issue/comment.md), [`develop`](./commands/issue/develop.md), [`edit`](./commands/issue/edit.md), [`transfer`](./commands/issue/transfer.md) |
| **[`repo`](./commands/repo/index.md)** | Manage repositories & remotes | [`clone`](./commands/repo/clone.md), [`create`](./commands/repo/create.md), [`fork`](./commands/repo/fork.md), [`view`](./commands/repo/view.md), [`list`](./commands/repo/list.md), [`sync`](./commands/repo/sync.md), [`edit`](./commands/repo/edit.md), [`deploy-key`](./commands/repo/deploy-key.md) |
| **[`release`](./commands/release/index.md)** | Create and publish releases & assets | [`create`](./commands/release/create.md), [`download`](./commands/release/download.md), [`upload`](./commands/release/upload.md), [`list`](./commands/release/list.md), [`view`](./commands/release/view.md) |
| **[`project`](./commands/project/index.md)** | GitHub Projects (v2) boards | [`list`](./commands/project/list.md), [`view`](./commands/project/view.md), [`item-add`](./commands/project/item-add.md), [`item-list`](./commands/project/item-list.md), [`field-list`](./commands/project/field-list.md) |
| **[`org`](./commands/org/index.md)** | Organization management | [`list`](./commands/org/list.md) |
| **[`gist`](./commands/gist/index.md)** | Manage snippets & GitHub Gists | [`create`](./commands/gist/create.md), [`list`](./commands/gist/list.md), [`view`](./commands/gist/view.md), [`clone`](./commands/gist/clone.md) |

---

### GitHub Actions & CI/CD
| Command Group | Description | Key Subcommands |
| :--- | :--- | :--- |
| **[`run`](./commands/run/index.md)** | Inspect, trigger, and rerun workflow runs | [`list`](./commands/run/list.md), [`view`](./commands/run/view.md), [`watch`](./commands/run/watch.md), [`rerun`](./commands/run/rerun.md), [`cancel`](./commands/run/cancel.md), [`download`](./commands/run/download.md) |
| **[`workflow`](./commands/workflow/index.md)** | List, view, and manually trigger workflows | [`list`](./commands/workflow/list.md), [`run`](./commands/workflow/run.md), [`view`](./commands/workflow/view.md), [`enable`](./commands/workflow/enable.md), [`disable`](./commands/workflow/disable.md) |
| **[`cache`](./commands/cache/index.md)** | Manage GitHub Actions dependency caches | [`list`](./commands/cache/list.md), [`delete`](./commands/cache/delete.md) |

---

### Configuration, Secrets & Environment
| Command Group | Description | Key Subcommands |
| :--- | :--- | :--- |
| **[`secret`](./commands/secret/index.md)** | Manage encrypted repository & org secrets | [`set`](./commands/secret/set.md), [`list`](./commands/secret/list.md), [`delete`](./commands/secret/delete.md) |
| **[`variable`](./commands/variable/index.md)** | Non-sensitive environment variables | [`set`](./commands/variable/set.md), [`get`](./commands/variable/get.md), [`list`](./commands/variable/list.md), [`delete`](./commands/variable/delete.md) |
| **[`config`](./commands/config/index.md)** | Global and local CLI preferences | [`get`](./commands/config/get.md), [`set`](./commands/config/set.md), [`list`](./commands/config/list.md), [`clear-cache`](./commands/config/clear-cache.md) |
| **[`alias`](./commands/alias/index.md)** | Custom command aliases & shortcuts | [`set`](./commands/alias/set.md), [`list`](./commands/alias/list.md), [`delete`](./commands/alias/delete.md), [`import`](./commands/alias/import.md) |

---

### Platform, Search & Developer Capabilities
| Command | Description | Link |
| :--- | :--- | :--- |
| **`api`** | Direct authenticated REST and GraphQL calls | [`commands/api.md`](./commands/api.md) |
| **`codespace`** | Cloud developer environments management | [`commands/codespace/index.md`](./commands/codespace/index.md) |
| **`copilot`** | GitHub Copilot CLI interface & explanations | [`commands/copilot.md`](./commands/copilot.md) |
| **`search`** | Search across code, commits, issues, PRs, and repos | [`commands/search/index.md`](./commands/search/index.md) |
| **`attestation`** | Build artifact provenance and signing verification | [`commands/attestation/index.md`](./commands/attestation/index.md) |
| **`skill`** | Manage and run agent skills | [`commands/skill/index.md`](./commands/skill/index.md) |
| **`agent-task`** | Autonomous task runner (preview) | [`commands/agent-task/index.md`](./commands/agent-task/index.md) |
| **`ruleset`** | Inspect repository branch protection rulesets | [`commands/ruleset/index.md`](./commands/ruleset/index.md) |
| **`label`** | Manage repository labels and taxonomy | [`commands/label/index.md`](./commands/label/index.md) |
| **`discussion`** | GitHub Team & Community Discussions | [`commands/discussion/index.md`](./commands/discussion/index.md) |
| **`ssh-key`** / **`gpg-key`** | Key management for git commit signing & SSH auth | [`commands/ssh-key/index.md`](./commands/ssh-key/index.md) • [`commands/gpg-key/index.md`](./commands/gpg-key/index.md) |
| **`extension`** | Install, update, and manage community CLI extensions | [`commands/extension/index.md`](./commands/extension/index.md) |
| **`browse`** | Open repository pages in default browser | [`commands/browse.md`](./commands/browse.md) |
| **`status`** | Aggregated status overview across your tracked repos | [`commands/status.md`](./commands/status.md) |
| **`completion`** | Shell autocompletion scripts (bash, zsh, fish, pwsh) | [`commands/completion.md`](./commands/completion.md) |
| **`preview`** | Access preview and beta CLI features | [`commands/preview/index.md`](./commands/preview/index.md) |
| **`licenses`** | Third-party license attributions | [`commands/licenses.md`](./commands/licenses.md) |

---

## 📚 Guides & Deep-Dive Topics

- 📊 **[Output Formatting (`--json`, `--jq`, `--template`)](./topics/formatting.md)**: How to extract exact fields and write Go templates.
- ⚙️ **[Environment Variables Reference](./topics/environment.md)**: Full list of variables (`GH_TOKEN`, `GH_HOST`, `GH_REPO`, `GH_DEBUG`, `GH_PAGER`, etc.).
- 🚀 **[GitHub Actions Integration Guide](./topics/actions.md)**: Using `gh` in workflows without storing manual secrets.
- 🚦 **[CLI Exit Codes](./topics/exit-codes.md)**: How to trap errors and handle exit codes cleanly in scripts.
- ♿ **[Terminal Accessibility & Colors](./topics/accessibility.md)**: Handling `NO_COLOR` and terminal accessibility options.
- 📈 **[Telemetry & Diagnostics](./topics/telemetry.md)**: Diagnostic logging and GitHub CLI telemetry behavior.

---

## 🤖 Using with AI Coding Tools

### Cursor, Windsurf & Claude Code
Add this repository to your AI tool's context or indexing path:
1. In Cursor / Windsurf: add `FULL_REFERENCE.md` or this repository folder as a context source.
2. In agent rules (e.g. `.cursorrules`, `CLAUDE.md`, or `AGENTS.md`), add:
   ```markdown
   When interacting with GitHub CLI (`gh`), follow the headless patterns in github-cli-manual/README.md:
   - Always append `--json <fields>` and `--jq` for parsing.
   - Never run interactive commands; use `--fill`, `--yes`, or pass standard input.
   - Reference github-cli-manual/FULL_REFERENCE.md for exact flags.
   ```

### Claude Desktop & ChatGPT Projects
Upload [`FULL_REFERENCE.md`](./FULL_REFERENCE.md) to your Project Knowledge base to turn any LLM into a GitHub CLI power assistant without token limits or hallucinations.

---

## 🤝 Contributing

Contributions, updates, and improvements are always welcome!
- Found a missing command or outdated flag? Open a PR or Issue.
- Have a high-utility `--json` / `--jq` recipe? Add it to [`topics/formatting.md`](./topics/formatting.md).
- Follow standard Markdown formatting and keep token density tight for LLMs.

---

## 📄 License

This manual is open-source documentation provided under the [MIT License](https://opensource.org/licenses/MIT). Refer to the official [GitHub CLI Repository](https://github.com/cli/cli) for official binary licensing.

<div align="center">
  <sub>Built with ❤️ for developers, DevOps engineers, and autonomous AI agents.</sub>
</div>
