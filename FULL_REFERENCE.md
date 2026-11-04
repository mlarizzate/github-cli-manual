# GitHub CLI (gh) Comprehensive Offline Manual & Reference

> Complete offline manual containing every command, subcommand, flag, example, and reference topic for GitHub CLI.
> Generated for AI agents, developers, and automated scripts requiring zero-network documentation.

## Table of Contents

### Help Topics & Guides
- [accessibility](#topic-accessibility): Learn about GitHub CLI's accessibility experiences
- [actions](#topic-actions): Learn about working with GitHub Actions
- [environment](#topic-environment): Environment variables that can be used with gh
- [exit-codes](#topic-exit-codes): Exit codes used by gh
- [formatting](#topic-formatting): Formatting options for JSON data exported from gh
- [mintty](#topic-mintty): Information about using gh with MinTTY
- [telemetry](#topic-telemetry): Information about telemetry in gh

### Command Reference

- [`gh agent-task`](#cmd-agent-task) (3 subcommands)
- [`gh agent-task create`](#cmd-agent-task-create)
- [`gh agent-task list`](#cmd-agent-task-list)
- [`gh agent-task view`](#cmd-agent-task-view)
- [`gh alias`](#cmd-alias) (4 subcommands)
- [`gh alias delete`](#cmd-alias-delete)
- [`gh alias import`](#cmd-alias-import)
- [`gh alias list`](#cmd-alias-list)
- [`gh alias set`](#cmd-alias-set)
- [`gh api`](#cmd-api)
- [`gh attestation`](#cmd-attestation) (3 subcommands)
- [`gh attestation download`](#cmd-attestation-download)
- [`gh attestation trusted-root`](#cmd-attestation-trusted-root)
- [`gh attestation verify`](#cmd-attestation-verify)
- [`gh auth`](#cmd-auth) (7 subcommands)
- [`gh auth login`](#cmd-auth-login)
- [`gh auth logout`](#cmd-auth-logout)
- [`gh auth refresh`](#cmd-auth-refresh)
- [`gh auth setup-git`](#cmd-auth-setup-git)
- [`gh auth status`](#cmd-auth-status)
- [`gh auth switch`](#cmd-auth-switch)
- [`gh auth token`](#cmd-auth-token)
- [`gh browse`](#cmd-browse)
- [`gh cache`](#cmd-cache) (2 subcommands)
- [`gh cache delete`](#cmd-cache-delete)
- [`gh cache list`](#cmd-cache-list)
- [`gh codespace`](#cmd-codespace) (13 subcommands)
- [`gh codespace code`](#cmd-codespace-code)
- [`gh codespace cp`](#cmd-codespace-cp)
- [`gh codespace create`](#cmd-codespace-create)
- [`gh codespace delete`](#cmd-codespace-delete)
- [`gh codespace edit`](#cmd-codespace-edit)
- [`gh codespace jupyter`](#cmd-codespace-jupyter)
- [`gh codespace list`](#cmd-codespace-list)
- [`gh codespace logs`](#cmd-codespace-logs)
- [`gh codespace ports`](#cmd-codespace-ports) (2 subcommands)
- [`gh codespace ports forward`](#cmd-codespace-ports-forward)
- [`gh codespace ports visibility`](#cmd-codespace-ports-visibility)
- [`gh codespace rebuild`](#cmd-codespace-rebuild)
- [`gh codespace ssh`](#cmd-codespace-ssh)
- [`gh codespace stop`](#cmd-codespace-stop)
- [`gh codespace view`](#cmd-codespace-view)
- [`gh completion`](#cmd-completion)
- [`gh config`](#cmd-config) (4 subcommands)
- [`gh config clear-cache`](#cmd-config-clear-cache)
- [`gh config get`](#cmd-config-get)
- [`gh config list`](#cmd-config-list)
- [`gh config set`](#cmd-config-set)
- [`gh copilot`](#cmd-copilot)
- [`gh discussion`](#cmd-discussion) (5 subcommands)
- [`gh discussion comment`](#cmd-discussion-comment)
- [`gh discussion create`](#cmd-discussion-create)
- [`gh discussion edit`](#cmd-discussion-edit)
- [`gh discussion list`](#cmd-discussion-list)
- [`gh discussion view`](#cmd-discussion-view)
- [`gh extension`](#cmd-extension) (8 subcommands)
- [`gh extension browse`](#cmd-extension-browse)
- [`gh extension create`](#cmd-extension-create)
- [`gh extension exec`](#cmd-extension-exec)
- [`gh extension install`](#cmd-extension-install)
- [`gh extension list`](#cmd-extension-list)
- [`gh extension remove`](#cmd-extension-remove)
- [`gh extension search`](#cmd-extension-search)
- [`gh extension upgrade`](#cmd-extension-upgrade)
- [`gh gist`](#cmd-gist) (7 subcommands)
- [`gh gist clone`](#cmd-gist-clone)
- [`gh gist create`](#cmd-gist-create)
- [`gh gist delete`](#cmd-gist-delete)
- [`gh gist edit`](#cmd-gist-edit)
- [`gh gist list`](#cmd-gist-list)
- [`gh gist rename`](#cmd-gist-rename)
- [`gh gist view`](#cmd-gist-view)
- [`gh gpg-key`](#cmd-gpg-key) (3 subcommands)
- [`gh gpg-key add`](#cmd-gpg-key-add)
- [`gh gpg-key delete`](#cmd-gpg-key-delete)
- [`gh gpg-key list`](#cmd-gpg-key-list)
- [`gh issue`](#cmd-issue) (16 subcommands)
- [`gh issue artifact`](#cmd-issue-artifact) (6 subcommands)
- [`gh issue artifact create`](#cmd-issue-artifact-create)
- [`gh issue artifact delete`](#cmd-issue-artifact-delete)
- [`gh issue artifact download`](#cmd-issue-artifact-download)
- [`gh issue artifact edit`](#cmd-issue-artifact-edit)
- [`gh issue artifact list`](#cmd-issue-artifact-list)
- [`gh issue artifact view`](#cmd-issue-artifact-view)
- [`gh issue close`](#cmd-issue-close)
- [`gh issue comment`](#cmd-issue-comment)
- [`gh issue create`](#cmd-issue-create)
- [`gh issue delete`](#cmd-issue-delete)
- [`gh issue develop`](#cmd-issue-develop)
- [`gh issue edit`](#cmd-issue-edit)
- [`gh issue list`](#cmd-issue-list)
- [`gh issue lock`](#cmd-issue-lock)
- [`gh issue pin`](#cmd-issue-pin)
- [`gh issue reopen`](#cmd-issue-reopen)
- [`gh issue status`](#cmd-issue-status)
- [`gh issue transfer`](#cmd-issue-transfer)
- [`gh issue unlock`](#cmd-issue-unlock)
- [`gh issue unpin`](#cmd-issue-unpin)
- [`gh issue view`](#cmd-issue-view)
- [`gh label`](#cmd-label) (5 subcommands)
- [`gh label clone`](#cmd-label-clone)
- [`gh label create`](#cmd-label-create)
- [`gh label delete`](#cmd-label-delete)
- [`gh label edit`](#cmd-label-edit)
- [`gh label list`](#cmd-label-list)
- [`gh licenses`](#cmd-licenses)
- [`gh org`](#cmd-org) (1 subcommands)
- [`gh org list`](#cmd-org-list)
- [`gh pr`](#cmd-pr) (18 subcommands)
- [`gh pr checkout`](#cmd-pr-checkout)
- [`gh pr checks`](#cmd-pr-checks)
- [`gh pr close`](#cmd-pr-close)
- [`gh pr comment`](#cmd-pr-comment)
- [`gh pr create`](#cmd-pr-create)
- [`gh pr diff`](#cmd-pr-diff)
- [`gh pr edit`](#cmd-pr-edit)
- [`gh pr list`](#cmd-pr-list)
- [`gh pr lock`](#cmd-pr-lock)
- [`gh pr merge`](#cmd-pr-merge)
- [`gh pr ready`](#cmd-pr-ready)
- [`gh pr reopen`](#cmd-pr-reopen)
- [`gh pr revert`](#cmd-pr-revert)
- [`gh pr review`](#cmd-pr-review)
- [`gh pr status`](#cmd-pr-status)
- [`gh pr unlock`](#cmd-pr-unlock)
- [`gh pr update-branch`](#cmd-pr-update-branch)
- [`gh pr view`](#cmd-pr-view)
- [`gh preview`](#cmd-preview) (1 subcommands)
- [`gh preview prompter`](#cmd-preview-prompter)
- [`gh project`](#cmd-project) (19 subcommands)
- [`gh project close`](#cmd-project-close)
- [`gh project copy`](#cmd-project-copy)
- [`gh project create`](#cmd-project-create)
- [`gh project delete`](#cmd-project-delete)
- [`gh project edit`](#cmd-project-edit)
- [`gh project field-create`](#cmd-project-field-create)
- [`gh project field-delete`](#cmd-project-field-delete)
- [`gh project field-list`](#cmd-project-field-list)
- [`gh project item-add`](#cmd-project-item-add)
- [`gh project item-archive`](#cmd-project-item-archive)
- [`gh project item-create`](#cmd-project-item-create)
- [`gh project item-delete`](#cmd-project-item-delete)
- [`gh project item-edit`](#cmd-project-item-edit)
- [`gh project item-list`](#cmd-project-item-list)
- [`gh project link`](#cmd-project-link)
- [`gh project list`](#cmd-project-list)
- [`gh project mark-template`](#cmd-project-mark-template)
- [`gh project unlink`](#cmd-project-unlink)
- [`gh project view`](#cmd-project-view)
- [`gh release`](#cmd-release) (10 subcommands)
- [`gh release create`](#cmd-release-create)
- [`gh release delete`](#cmd-release-delete)
- [`gh release delete-asset`](#cmd-release-delete-asset)
- [`gh release download`](#cmd-release-download)
- [`gh release edit`](#cmd-release-edit)
- [`gh release list`](#cmd-release-list)
- [`gh release upload`](#cmd-release-upload)
- [`gh release verify`](#cmd-release-verify)
- [`gh release verify-asset`](#cmd-release-verify-asset)
- [`gh release view`](#cmd-release-view)
- [`gh repo`](#cmd-repo) (18 subcommands)
- [`gh repo archive`](#cmd-repo-archive)
- [`gh repo autolink`](#cmd-repo-autolink) (4 subcommands)
- [`gh repo autolink create`](#cmd-repo-autolink-create)
- [`gh repo autolink delete`](#cmd-repo-autolink-delete)
- [`gh repo autolink list`](#cmd-repo-autolink-list)
- [`gh repo autolink view`](#cmd-repo-autolink-view)
- [`gh repo clone`](#cmd-repo-clone)
- [`gh repo create`](#cmd-repo-create)
- [`gh repo delete`](#cmd-repo-delete)
- [`gh repo deploy-key`](#cmd-repo-deploy-key) (3 subcommands)
- [`gh repo deploy-key add`](#cmd-repo-deploy-key-add)
- [`gh repo deploy-key delete`](#cmd-repo-deploy-key-delete)
- [`gh repo deploy-key list`](#cmd-repo-deploy-key-list)
- [`gh repo edit`](#cmd-repo-edit)
- [`gh repo fork`](#cmd-repo-fork)
- [`gh repo gitignore`](#cmd-repo-gitignore) (2 subcommands)
- [`gh repo gitignore list`](#cmd-repo-gitignore-list)
- [`gh repo gitignore view`](#cmd-repo-gitignore-view)
- [`gh repo license`](#cmd-repo-license) (2 subcommands)
- [`gh repo license list`](#cmd-repo-license-list)
- [`gh repo license view`](#cmd-repo-license-view)
- [`gh repo list`](#cmd-repo-list)
- [`gh repo read-dir`](#cmd-repo-read-dir)
- [`gh repo read-file`](#cmd-repo-read-file)
- [`gh repo rename`](#cmd-repo-rename)
- [`gh repo set-default`](#cmd-repo-set-default)
- [`gh repo sync`](#cmd-repo-sync)
- [`gh repo unarchive`](#cmd-repo-unarchive)
- [`gh repo view`](#cmd-repo-view)
- [`gh ruleset`](#cmd-ruleset) (3 subcommands)
- [`gh ruleset check`](#cmd-ruleset-check)
- [`gh ruleset list`](#cmd-ruleset-list)
- [`gh ruleset view`](#cmd-ruleset-view)
- [`gh run`](#cmd-run) (7 subcommands)
- [`gh run cancel`](#cmd-run-cancel)
- [`gh run delete`](#cmd-run-delete)
- [`gh run download`](#cmd-run-download)
- [`gh run list`](#cmd-run-list)
- [`gh run rerun`](#cmd-run-rerun)
- [`gh run view`](#cmd-run-view)
- [`gh run watch`](#cmd-run-watch)
- [`gh search`](#cmd-search) (5 subcommands)
- [`gh search code`](#cmd-search-code)
- [`gh search commits`](#cmd-search-commits)
- [`gh search issues`](#cmd-search-issues)
- [`gh search prs`](#cmd-search-prs)
- [`gh search repos`](#cmd-search-repos)
- [`gh secret`](#cmd-secret) (3 subcommands)
- [`gh secret delete`](#cmd-secret-delete)
- [`gh secret list`](#cmd-secret-list)
- [`gh secret set`](#cmd-secret-set)
- [`gh skill`](#cmd-skill) (6 subcommands)
- [`gh skill install`](#cmd-skill-install)
- [`gh skill list`](#cmd-skill-list)
- [`gh skill preview`](#cmd-skill-preview)
- [`gh skill publish`](#cmd-skill-publish)
- [`gh skill search`](#cmd-skill-search)
- [`gh skill update`](#cmd-skill-update)
- [`gh ssh-key`](#cmd-ssh-key) (3 subcommands)
- [`gh ssh-key add`](#cmd-ssh-key-add)
- [`gh ssh-key delete`](#cmd-ssh-key-delete)
- [`gh ssh-key list`](#cmd-ssh-key-list)
- [`gh status`](#cmd-status)
- [`gh variable`](#cmd-variable) (4 subcommands)
- [`gh variable delete`](#cmd-variable-delete)
- [`gh variable get`](#cmd-variable-get)
- [`gh variable list`](#cmd-variable-list)
- [`gh variable set`](#cmd-variable-set)
- [`gh workflow`](#cmd-workflow) (5 subcommands)
- [`gh workflow disable`](#cmd-workflow-disable)
- [`gh workflow enable`](#cmd-workflow-enable)
- [`gh workflow list`](#cmd-workflow-list)
- [`gh workflow run`](#cmd-workflow-run)
- [`gh workflow view`](#cmd-workflow-view)

---

# Core Guides & Help Topics

## <a id="topic-accessibility"></a>Topic: `accessibility`

> Learn about GitHub CLI's accessibility experiences

Learn about GitHub CLI's accessibility experiences

As the home for all developers, we want every developer to feel welcome in our
community and be empowered to contribute to the future of global software
development with everything GitHub has to offer including the GitHub CLI.

Customizable and contrasting colors

Text interfaces often use color for various purposes, but insufficient contrast
or customizability can leave some users unable to benefit.

For a more accessible experience, the GitHub CLI can use color palettes
based on terminal background appearance and limit colors to 4-bit ANSI color
palettes, which users can customize within terminal preferences.

With this new experience, the GitHub CLI provides multiple options to address
color usage:

1. The GitHub CLI will use 4-bit color palette for increased color contrast based
   on dark and light backgrounds including rendering Markdown based on the
   GitHub Primer design system.

   To enable this experience, use one of the following methods:
   - Run `gh config set accessible_colors enabled`
   - Set `GH_ACCESSIBLE_COLORS=enabled` environment variable

2. The GitHub CLI will display issue and pull request labels' custom RGB colors
   in terminals with true color support.

   To enable this experience, use one of the following methods:
   - Run `gh config set color_labels enabled`
   - Set `GH_COLOR_LABELS=enabled` environment variable

Non-interactive user input prompting

Interactive text user interfaces manipulate the terminal cursor to redraw parts
of the screen, which can be difficult for speech synthesizers or braille displays
to accurately detect and read.

For a more accessible experience, the GitHub CLI can provide a similar experience using
non-interactive prompts for user input.

To enable this experience, use one of the following methods:
- Run `gh config set accessible_prompter enabled`
- Set `GH_ACCESSIBLE_PROMPTER=enabled` environment variable

Text-based spinners

Motion-based spinners communicate in-progress activity by manipulating the
terminal cursor to create a spinning effect, which may cause discomfort to users
with motion sensitivity or miscommunicate information to speech synthesizers.

For a more accessible experience, this interactivity can be disabled in favor
of text-based progress indicators.

To enable this experience, use one of the following methods:
- Run `gh config set spinner disabled`
- Set `GH_SPINNER_DISABLED=yes` environment variable

Join the conversation

We invite you to join us in improving GitHub CLI accessibility by sharing your
feedback and ideas through GitHub Accessibility feedback channels:

https://github.com/orgs/community/discussions/categories/accessibility


USAGE
  gh accessibility [flags]

ALIASES
  gh a11y

FLAGS
  -w, --web   Open the GitHub Accessibility site in your browser

INHERITED FLAGS
  --help   Show help for command

EXAMPLES
  # Open the GitHub Accessibility site in your browser
  $ gh accessibility --web
  
  # Display color using customizable, 4-bit accessible colors
  $ gh config set accessible_colors enabled
  
  # Use input prompts without redrawing the screen
  $ gh config set accessible_prompter enabled
  
  # Disable motion-based spinners for progress indicators in favor of text
  $ gh config set spinner disabled

LEARN MORE
  Use `gh <command> <subcommand> --help` for more information about a command.
  Read the manual at https://cli.github.com/manual
  Learn about exit codes using `gh help exit-codes`
  Learn about accessibility experiences using `gh help accessibility`

---

## <a id="topic-actions"></a>Topic: `actions`

> Learn about working with GitHub Actions

Welcome to GitHub Actions on the command line.

GitHub CLI integrates with GitHub Actions to help you manage runs and workflows.

Interacting with workflow runs
gh run list:      List recent workflow runs
gh run view:      View details for a workflow run or one of its jobs
gh run watch:     Watch a workflow run while it executes
gh run rerun:     Rerun a failed workflow run
gh run download:  Download artifacts generated by runs

To see more help, run `gh help run <subcommand>`

Interacting with workflow files
gh workflow list:     List workflow files in your repository
gh workflow view:     View details for a workflow file
gh workflow enable:   Enable a workflow file
gh workflow disable:  Disable a workflow file
gh workflow run:      Trigger a workflow_dispatch run for a workflow file

To see more help, run `gh help workflow <subcommand>`

Interacting with the GitHub Actions cache
gh cache list:    List all the caches saved in GitHub Actions for a repository
gh cache delete:  Delete one or all saved caches in GitHub Actions for a repository

To see more help, run `gh help cache <subcommand>`



USAGE
  gh actions [flags]

INHERITED FLAGS
  --help   Show help for command

LEARN MORE
  Use `gh <command> <subcommand> --help` for more information about a command.
  Read the manual at https://cli.github.com/manual
  Learn about exit codes using `gh help exit-codes`
  Learn about accessibility experiences using `gh help accessibility`

---

## <a id="topic-environment"></a>Topic: `environment`

> Environment variables that can be used with gh

`GH_TOKEN`, `GITHUB_TOKEN` (in order of precedence): an authentication token that will be used when
a command targets either `github.com` or a subdomain of `ghe.com`. Setting this avoids being prompted to
authenticate and takes precedence over previously stored credentials.

`GH_ENTERPRISE_TOKEN`, `GITHUB_ENTERPRISE_TOKEN` (in order of precedence): an authentication
token that will be used when a command targets a GitHub Enterprise Server host.

`GH_HOST`: specify the GitHub hostname for commands where a hostname has not been provided, or
cannot be inferred from the context of a local Git repository. If this host was previously
authenticated with, the stored credentials will be used. Otherwise, setting `GH_TOKEN` or
`GH_ENTERPRISE_TOKEN` is required, depending on the targeted host.

`GH_REPO`: specify the GitHub repository in the `[HOST/]OWNER/REPO` format for commands
that otherwise operate on a local repository.

`GH_EDITOR`, `GIT_EDITOR`, `VISUAL`, `EDITOR` (in order of precedence): the editor tool to use
for authoring text.

`GH_BROWSER`, `BROWSER` (in order of precedence): the web browser to use for opening links.

`GH_DEBUG`: set to a truthy value to enable verbose output on standard error. Set to `api`
to additionally log details of HTTP traffic.

`DEBUG` (deprecated): set to `1`, `true`, or `yes` to enable verbose output on standard
error.

`GH_PAGER`, `PAGER` (in order of precedence): a terminal paging program to send standard output
to, e.g. `less`.

`GLAMOUR_STYLE`: the style to use for rendering Markdown. See
<https://github.com/charmbracelet/glamour#styles>

`NO_COLOR`: set to any value to avoid printing ANSI escape sequences for color output.

`CLICOLOR`: set to `0` to disable printing ANSI colors in output.

`CLICOLOR_FORCE`: set to a value other than `0` to keep ANSI colors in output
even when the output is piped.

`GH_COLOR_LABELS`: set to any value to display labels using their RGB hex color codes in terminals that
support truecolor.

`GH_ACCESSIBLE_COLORS` (preview): set to a truthy value to use customizable, 4-bit accessible colors.

`GH_FORCE_TTY`: set to any value to force terminal-style output even when the output is
redirected. When the value is a number, it is interpreted as the number of columns
available in the viewport. When the value is a percentage, it will be applied against
the number of columns available in the current viewport.

`GH_NO_UPDATE_NOTIFIER`: set to any value to disable GitHub CLI update notifications.
When any command is executed, gh checks for new versions once every 24 hours.
If a newer version was found, an upgrade notice is displayed on standard error.

`GH_NO_EXTENSION_UPDATE_NOTIFIER`: set to any value to disable GitHub CLI extension update notifications.
When an extension is executed, gh checks for new versions for the executed extension once every 24 hours.
If a newer version was found, an upgrade notice is displayed on standard error.

`GH_EXTENSION`: set to `1` by gh when it invokes an extension, allowing an extension to
tell whether it was run as `gh <extension>` or directly as a standalone program.

`GH_CONFIG_DIR`: the directory where gh will store configuration files. If not specified,
the default value will be one of the following paths (in order of precedence):
  - `$XDG_CONFIG_HOME/gh` (if `$XDG_CONFIG_HOME` is set),
  - `$AppData/GitHub CLI` (on Windows if `$AppData` is set), or
  - `$HOME/.config/gh`.

`GH_PROMPT_DISABLED`: set to any value to disable interactive prompting in the terminal.

`GH_PATH`: set the path to the gh executable, useful for when gh can not properly determine
its own path such as in the cygwin terminal. gh also sets this when invoking extensions so they
can call back into the same gh executable.

`GH_MDWIDTH`: default maximum width for markdown render wrapping.  The max width of lines
wrapped on the terminal will be taken as the lesser of the terminal width, this value, or 120 if
not specified.  This value is used, for example, with `pr view` subcommand.

`GH_ACCESSIBLE_PROMPTER` (preview): set to a truthy value to enable prompts that are
more compatible with speech synthesis and braille screen readers.

`GH_TELEMETRY`: set to `log` to print telemetry data to standard error instead of sending it.
Set to `false` or `0` to disable telemetry. Takes precedence over `DO_NOT_TRACK`.

`DO_NOT_TRACK`: set to `true` or `1` to disable telemetry. Ignored when
`GH_TELEMETRY` is set, which takes precedence.

`GH_SPINNER_DISABLED`: set to a truthy value to replace the spinner animation with
a textual progress indicator.

---

## <a id="topic-exit-codes"></a>Topic: `exit-codes`

> Exit codes used by gh

gh follows normal conventions regarding exit codes.

- If a command completes successfully, the exit code will be 0

- If a command fails for any reason, the exit code will be 1

- If a command is running but gets cancelled, the exit code will be 2

- If a command requires authentication, the exit code will be 4

NOTE: It is possible that a particular command may have more exit codes, so it is a good
practice to check documentation for the command if you are relying on exit codes to
control some behavior.

---

## <a id="topic-formatting"></a>Topic: `formatting`

> Formatting options for JSON data exported from gh

By default, the result of `gh` commands are output in line-based plain text format.
Some commands support passing the `--json` flag, which converts the output to JSON format.
Once in JSON, the output can be further formatted according to a required formatting string by
adding either the `--jq` or `--template` flag. This is useful for selecting a subset of data,
creating new data structures, displaying the data in a different format, or as input to another
command line script.

The `--json` flag requires a comma separated list of fields to fetch. To view the possible JSON
field names for a command omit the string argument to the `--json` flag when you run the command.
Note that you must pass the `--json` flag and field names to use the `--jq` or `--template` flags.

The `--jq` flag requires a string argument in jq query syntax, and will only print
those JSON values which match the query. jq queries can be used to select elements from an
array, fields from an object, create a new array, and more. The `jq` utility does not need
to be installed on the system to use this formatting directive. When connected to a terminal,
the output is automatically pretty-printed. To learn about jq query syntax, see:
<https://jqlang.github.io/jq/manual/>

The `--template` flag requires a string argument in Go template syntax, and will only print
those JSON values which match the query.

In addition to the Go template functions in the standard library, the following functions can be used
with this formatting directive:
- `autocolor`: like `color`, but only emits color to terminals
- `color <style> <input>`: colorize input using <https://github.com/mgutz/ansi>
- `join <sep> <list>`: joins values in the list using a separator
- `pluck <field> <list>`: collects values of a field from all items in the input
- `tablerow <fields>...`: aligns fields in output vertically as a table
- `tablerender`: renders fields added by tablerow in place
- `timeago <time>`: renders a timestamp as relative to now
- `timefmt <format> <time>`: formats a timestamp using Go's `Time.Format` function
- `truncate <length> <input>`: ensures input fits within length
- `hyperlink <url> <text>`: renders a terminal hyperlink

The following Sprig template library functions can also be used with this formatting directive:
- `contains <arg> <string>`: checks if `string` contains `arg`
- `hasPrefix <prefix> <string>`: checks if `string` starts with `prefix`
- `hasSuffix <suffix> <string>`: checks if `string` ends with `suffix`
- `regexMatch <regex> <string>`: checks if `string` has any matches for `regex`

For more information about the Sprig library, see <https://masterminds.github.io/sprig/>.

To learn more about Go templates, see: <https://golang.org/pkg/text/template/>.


EXAMPLES
  # Default output format
  $ gh pr list
  Showing 23 of 23 open pull requests in cli/cli
  
  #123  A helpful contribution          contribution-branch              about 1 day ago
  #124  Improve the docs                docs-branch                      about 2 days ago
  #125  An exciting new feature         feature-branch                   about 2 days ago
  
  
  # Adding the --json flag with a list of field names
  $ gh pr list --json number,title,author
  [
    {
      "author": {
        "login": "monalisa"
      },
      "number": 123,
      "title": "A helpful contribution"
    },
    {
      "author": {
        "login": "codercat"
      },
      "number": 124,
      "title": "Improve the docs"
    },
    {
      "author": {
        "login": "cli-maintainer"
      },
      "number": 125,
      "title": "An exciting new feature"
    }
  ]
  
  
  # Adding the --jq flag and selecting fields from the array
  $ gh pr list --json author --jq '.[].author.login'
  monalisa
  codercat
  cli-maintainer
  
  
  # --jq can be used to implement more complex filtering and output changes
  $ gh issue list --json number,title,labels --jq \
    'map(select((.labels | length) > 0))    # must have labels
    | map(.labels = (.labels | map(.name))) # show only the label names
    | .[:3]                                 # select the first 3 results'
    [
      {
        "labels": [
          "enhancement",
          "needs triage"
        ],
        "number": 123,
        "title": "A helpful contribution"
      },
      {
        "labels": [
          "help wanted",
          "docs",
          "good first issue"
        ],
        "number": 125,
        "title": "Improve the docs"
      },
      {
        "labels": [
          "enhancement",
        ],
        "number": 7221,
        "title": "An exciting new feature"
      }
    ]
  
  
  # Using the --template flag with the hyperlink helper
  $ gh issue list --json title,url --template '{{range .}}{{hyperlink .url .title}}{{"\n"}}{{end}}'
  
  
  # Adding the --template flag and modifying the display format
  $ gh pr list --json number,title,headRefName,updatedAt --template \
  	'{{range .}}{{tablerow (printf "#%v" .number | autocolor "green") .title .headRefName (timeago .updatedAt)}}{{end}}'
  
  #123  A helpful contribution      contribution-branch       about 1 day ago
  #124  Improve the docs            docs-branch               about 2 days ago
  #125  An exciting new feature     feature-branch            about 2 days ago
  
  
  # A more complex example with the --template flag which formats a pull request using multiple tables with headers
  $ gh pr view 3519 --json number,title,body,reviews,assignees --template \
  '{{printf "#%v" .number}} {{.title}}
  
  {{.body}}
  
  {{tablerow "ASSIGNEE" "NAME"}}{{range .assignees}}{{tablerow .login .name}}{{end}}{{tablerender}}
  {{tablerow "REVIEWER" "STATE" "COMMENT"}}{{range .reviews}}{{tablerow .author.login .state .body}}{{end}}
  '
  
  #3519 Add table and helper template functions
  
  Resolves #3488
  
  ASSIGNEE  NAME
  mislav    Mislav Marohnić
  
  
  REVIEWER  STATE              COMMENT
  mislav    COMMENTED          This is going along great! Thanks for working on this ❤️

---

## <a id="topic-mintty"></a>Topic: `mintty`

> Information about using gh with MinTTY

MinTTY is the terminal emulator that comes by default with Git
for Windows. It has known issues with gh's ability to prompt a
user for input.

There are a few workarounds to make gh work with MinTTY:

- Reinstall Git for Windows, checking "Enable experimental support for pseudo consoles".

- Use a different terminal emulator with Git for Windows like Windows Terminal.
  You can run `C:\Program Files\Git\bin\bash.exe` from any terminal emulator to continue
  using all of the tooling in Git For Windows without MinTTY.

- Prefix invocations of gh with `winpty`, eg: `winpty gh auth login`.
  NOTE: this can lead to some UI bugs.

---

## <a id="topic-telemetry"></a>Topic: `telemetry`

> Information about telemetry in gh

gh collects telemetry to help us understand how the CLI is being used and to improve it.

To learn more about what data is collected, how it is used, and how to opt out, see:
<https://cli.github.com/telemetry>

---

# Complete Command Reference

## <a id="cmd-agent-task"></a>`gh agent-task`

Working with agent tasks in the GitHub CLI is in preview and
subject to change without notice.

### Synopsis
```bash
gh agent-task <command> [flags]
```

### Aliases
`gh agent-tasks, gh agent, gh agents`, ``, `AVAILABLE COMMANDS`, `  create:        Create an agent task (preview)`, `  list:          List agent tasks (preview)`, `  view:          View an agent task session (preview)`

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# List your most recent agent tasks
  $ gh agent-task list
  
  # Create a new agent task on the current repository
  $ gh agent-task create "Improve the performance of the data processing pipeline"
  
  # View details about agent tasks associated with a pull request
  $ gh agent-task view 123
  
  # View details about a specific agent task
  $ gh agent-task view 12345abc-12345-12345-12345-12345abc
```

---

## <a id="cmd-agent-task-create"></a>`gh agent-task create`

Create an agent task (preview)

### Synopsis
```bash
gh agent-task create [<task description>] [flags]
```

### Flags
```text
-b, --base string              Base branch for the pull request (use default branch if not provided)
  -a, --custom-agent string      Use a custom agent for the task. e.g., use 'my-agent' for the 'my-agent.md' agent
      --follow                   Follow agent session logs
  -F, --from-file file           Read task description from file (use "-" to read from standard input)
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Create a task from an inline description
  $ gh agent-task create "build me a new app"
  
  # Create a task from an inline description and follow logs
  $ gh agent-task create "build me a new app" --follow
  
  # Create a task from a file
  $ gh agent-task create -F task-desc.md
  
  # Create a task with problem statement from stdin
  $ echo "build me a new app" | gh agent-task create -F -
  
  # Create a task with an editor
  $ gh agent-task create
  
  # Create a task with an editor and a file as a template
  $ gh agent-task create -F task-desc.md
  
  # Select a different base branch for the PR
  $ gh agent-task create "fix errors" --base branch
  
  # Create a task using the custom agent defined in '.github/agents/my-agent.md'
  $ gh agent-task create "build me a new app" --custom-agent my-agent
```

---

## <a id="cmd-agent-task-list"></a>`gh agent-task list`

List agent tasks (preview)

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh agent-task list [flags]
```

### Flags
```text
-q, --jq expression     Filter JSON output using a jq expression
      --json fields       Output JSON with the specified fields
  -L, --limit int         Maximum number of agent tasks to fetch (default 30)
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
  -w, --web               Open agent tasks in the browser
```

### Inherited Flags
```text
--help   Show help for command

JSON FIELDS
  completedAt, createdAt, id, name, pullRequestNumber, pullRequestState,
  pullRequestTitle, pullRequestUrl, repository, state, updatedAt, user
```

---

## <a id="cmd-agent-task-view"></a>`gh agent-task view`

View an agent task session.

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh agent-task view [<session-id> | <pr-number> | <pr-url> | <pr-branch>] [flags]
```

### Flags
```text
--follow                   Follow agent session logs
  -q, --jq expression            Filter JSON output using a jq expression
      --json fields              Output JSON with the specified fields
      --log                      Show agent session logs
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
  -t, --template string          Format JSON output using a Go template; see "gh help formatting"
  -w, --web                      Open agent task in the browser
```

### Inherited Flags
```text
--help   Show help for command

JSON FIELDS
  completedAt, createdAt, id, name, pullRequestNumber, pullRequestState,
  pullRequestTitle, pullRequestUrl, repository, state, updatedAt, user
```

### Examples
```bash
# View an agent task by session ID
  $ gh agent-task view e2fa49d2-f164-4a56-ab99-498090b8fcdf
  
  # View an agent task by pull request number in current repo
  $ gh agent-task view 12345
  
  # View an agent task by pull request number
  $ gh agent-task view --repo OWNER/REPO 12345
  
  # View an agent task by pull request reference
  $ gh agent-task view OWNER/REPO#12345
  
  # View a pull request agents tasks in the browser
  $ gh agent-task view 12345 --web
```

---

## <a id="cmd-alias"></a>`gh alias`

Aliases can be used to make shortcuts for gh commands or to compose multiple commands.

Run `gh help alias set` to learn more.

### Synopsis
```bash
gh alias <command> [flags]

AVAILABLE COMMANDS
  delete:        Delete set aliases
  import:        Import aliases from a YAML file
  list:          List your aliases
  set:           Create a shortcut for a gh command
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-alias-delete"></a>`gh alias delete`

Delete set aliases

### Synopsis
```bash
gh alias delete {<alias> | --all} [flags]
```

### Flags
```text
--all   Delete all aliases
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-alias-import"></a>`gh alias import`

Import aliases from the contents of a YAML file.

Aliases should be defined as a map in YAML, where the keys represent aliases and
the values represent the corresponding expansions. An example file should look like
the following:

    bugs: issue list --label=bug
    igrep: '!gh issue list --label="$1" | grep "$2"'
    features: |-
        issue list
        --label=enhancement

Use `-` to read aliases (in YAML format) from standard input.

The output from `gh alias list` can be used to produce a YAML file
containing your aliases, which you can use to import them from one machine to
another. Run `gh help alias list` to learn more.

### Synopsis
```bash
gh alias import [<filename> | -] [flags]
```

### Flags
```text
--clobber   Overwrite existing aliases of the same name
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Import aliases from a file
  $ gh alias import aliases.yml
  
  # Import aliases from standard input
  $ gh alias import -
```

---

## <a id="cmd-alias-list"></a>`gh alias list`

This command prints out all of the aliases gh is configured to use.

### Synopsis
```bash
gh alias list [flags]
```

### Aliases
`gh alias ls`

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-alias-set"></a>`gh alias set`

Define a word that will expand to a full gh command when invoked.

The expansion may specify additional arguments and flags. If the expansion includes
positional placeholders such as `$1`, extra arguments that follow the alias will be
inserted appropriately. Otherwise, extra arguments will be appended to the expanded
command.

Use `-` as expansion argument to read the expansion string from standard input. This
is useful to avoid quoting issues when defining expansions.

If the expansion starts with `!` or if `--shell` was given, the expansion is a shell
expression that will be evaluated through the `sh` interpreter when the alias is
invoked. This allows for chaining multiple commands via piping and redirection.

### Synopsis
```bash
gh alias set <alias> <expansion> [flags]
```

### Flags
```text
--clobber   Overwrite existing aliases of the same name
  -s, --shell     Declare an alias to be passed through a shell interpreter
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Note: Command Prompt on Windows requires using double quotes for arguments
  $ gh alias set pv 'pr view'
  $ gh pv -w 123  #=> gh pr view -w 123
  
  $ gh alias set bugs 'issue list --label=bugs'
  $ gh bugs
  
  $ gh alias set homework 'issue list --assignee @me'
  $ gh homework
  
  $ gh alias set 'issue mine' 'issue list --mention @me'
  $ gh issue mine
  
  $ gh alias set epicsBy 'issue list --author="$1" --label="epic"'
  $ gh epicsBy vilmibm  #=> gh issue list --author="vilmibm" --label="epic"
  
  $ gh alias set --shell igrep 'gh issue list --label="$1" | grep "$2"'
  $ gh igrep epic foo  #=> gh issue list --label="epic" | grep "foo"
```

---

## <a id="cmd-api"></a>`gh api`

Makes an authenticated HTTP request to the GitHub API and prints the response.

The endpoint argument should either be a path of a GitHub API v3 endpoint, or
`graphql` to access the GitHub API v4.

Placeholder values `{owner}`, `{repo}`, and `{branch}` in the endpoint
argument will get replaced with values from the repository of the current
directory or the repository specified in the `GH_REPO` environment variable.
Note that in some shells, for example PowerShell, you may need to enclose
any value that contains `{...}` in quotes to prevent the shell from
applying special meaning to curly braces.

The `-p/--preview` flag enables opting into previews, which are feature-flagged,
experimental API endpoints or behaviors. The API expects opt-in via the `Accept`
header with format `application/vnd.github.<preview-name>-preview+json` and this
command facilitates that via `--preview <preview-name>`. To send a request for
the corsair and scarlet witch previews, you could use `-p corsair,scarlet-witch`
or `--preview corsair --preview scarlet-witch`.

The default HTTP request method is `GET` normally and `POST` if any parameters
were added. Override the method with `--method`.

Pass one or more `-f/--raw-field` values in `key=value` format to add static string
parameters to the request payload. To add non-string or placeholder-determined values, see
`-F/--field` below. Note that adding request parameters will automatically switch the
request method to `POST`. To send the parameters as a `GET` query string instead, use
`--method GET`.

The `-F/--field` flag has magic type conversion based on the format of the value:

- literal values `true`, `false`, `null`, and integer numbers get converted to
  appropriate JSON types;
- placeholder values `{owner}`, `{repo}`, and `{branch}` get populated with values
  from the repository of the current directory;
- if the value starts with `@`, the rest of the value is interpreted as a
  filename to read the value from. Pass `-` to read from standard input.

For GraphQL requests, all fields other than `query` and `operationName` are
interpreted as GraphQL variables.

To pass nested parameters in the request payload, use `key[subkey]=value` syntax when
declaring fields. To pass nested values as arrays, declare multiple fields with the
syntax `key[]=value1`, `key[]=value2`. To pass an empty array, use `key[]` without a
value.

To pass pre-constructed JSON or payloads in other formats, a request body may be read
from file specified by `--input`. Use `-` to read from standard input. When passing the
request body this way, any parameters specified via field flags are added to the query
string of the endpoint URL.

In `--paginate` mode, all pages of results will sequentially be requested until
there are no more pages of results. For GraphQL requests, this requires that the
original query accepts an `$endCursor: String` variable and that it fetches the
`pageInfo{ hasNextPage, endCursor }` set of fields from a collection. Each page is a separate
JSON array or object. Pass `--slurp` to wrap all pages of JSON arrays or objects
into an outer JSON array.

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh api <endpoint> [flags]
```

### Flags
```text
--allow-escape-sequences   Allow printing terminal escape sequences
      --cache duration           Cache the response, e.g. "3600s", "60m", "1h"
  -F, --field key=value          Add a typed parameter in key=value format (use "@<path>" or "@-" to read value from file or stdin)
  -H, --header key:value         Add a HTTP request header in key:value format
      --hostname string          The GitHub hostname for the request (default "github.com")
  -i, --include                  Include HTTP response status line and headers in the output
      --input file               The file to use as body for the HTTP request (use "-" to read from standard input)
  -q, --jq string                Query to select values from the response using jq syntax
  -X, --method string            The HTTP method for the request (default "GET")
      --paginate                 Make additional HTTP requests to fetch all pages of results
  -p, --preview strings          Opt into GitHub API previews (names should omit '-preview')
  -f, --raw-field key=value      Add a string parameter in key=value format
      --silent                   Do not print the response body
      --slurp                    Use with "--paginate" to return an array of all pages of either JSON arrays or objects
  -t, --template string          Format JSON output using a Go template; see "gh help formatting"
      --verbose                  Include full HTTP request and response in the output
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# List releases in the current repository
  $ gh api repos/{owner}/{repo}/releases
  
  # Post an issue comment
  $ gh api repos/{owner}/{repo}/issues/123/comments -f body='Hi from CLI'
  
  # Post nested parameter read from a file
  $ gh api gists -F 'files[myfile.txt][content]=@myfile.txt'
  
  # Add parameters to a GET request
  $ gh api -X GET search/issues -f q='repo:cli/cli is:open remote'
  
  # Use a JSON file as request body
  $ gh api repos/{owner}/{repo}/rulesets --input file.json
  
  # Set a custom HTTP header
  $ gh api -H 'Accept: application/vnd.github.v3.raw+json' ...
  
  # Opt into GitHub API previews
  $ gh api --preview baptiste,nebula ...
  
  # Print only specific fields from the response
  $ gh api repos/{owner}/{repo}/issues --jq '.[].title'
  
  # Use a template for the output
  $ gh api repos/{owner}/{repo}/issues --template \
    '{{range .}}{{.title}} ({{.labels | pluck "name" | join ", " | color "yellow"}}){{"\n"}}{{end}}'
  
  # Update allowed values of the "environment" custom property in a deeply nested array
  $ gh api -X PATCH /orgs/{org}/properties/schema \
     -F 'properties[][property_name]=environment' \
     -F 'properties[][default_value]=production' \
     -F 'properties[][allowed_values][]=staging' \
     -F 'properties[][allowed_values][]=production'
  
  # List releases with GraphQL
  $ gh api graphql -F owner='{owner}' -F name='{repo}' -f query='
    query($name: String!, $owner: String!) {
      repository(owner: $owner, name: $name) {
        releases(last: 3) {
          nodes { tagName }
        }
      }
    }
  '
  
  # List all repositories for a user
  $ gh api graphql --paginate -f query='
    query($endCursor: String) {
      viewer {
        repositories(first: 100, after: $endCursor) {
          nodes { nameWithOwner }
          pageInfo {
            hasNextPage
            endCursor
          }
        }
      }
    }
  '
  
  # Get the percentage of forks for the current user
  $ gh api graphql --paginate --slurp -f query='
    query($endCursor: String) {
      viewer {
        repositories(first: 100, after: $endCursor) {
          nodes { isFork }
          pageInfo {
            hasNextPage
            endCursor
          }
        }
      }
    }
  ' | jq 'def count(e): reduce e as $_ (0;.+1);
  [.[].data.viewer.repositories.nodes[]] as $r | count(select($r[].isFork))/count($r[])'

ENVIRONMENT VARIABLES
  GH_TOKEN, GITHUB_TOKEN (in order of precedence): an authentication token for
  `github.com` API requests.
  
  GH_ENTERPRISE_TOKEN, GITHUB_ENTERPRISE_TOKEN (in order of precedence): an
  authentication token for API requests to GitHub Enterprise.
  
  GH_HOST: make the request to a GitHub host other than `github.com`.
```

---

## <a id="cmd-attestation"></a>`gh attestation`

Download and verify artifact attestations.

### Synopsis
```bash
gh attestation [subcommand] [flags]
```

### Aliases
`gh at`, ``, `AVAILABLE COMMANDS`, `  download:      Download an artifact's attestations for offline use`, `  trusted-root:  Output trusted_root.jsonl contents, likely for offline verification`, `  verify:        Verify an artifact's integrity using attestations`

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-attestation-download"></a>`gh attestation download`

### NOTE: This feature is currently in public preview, and subject to change.

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

### Synopsis
```bash
gh attestation download [<file-path> | oci://<image-uri>] [--owner | --repo] [flags]
```

### Flags
```text
-d, --digest-alg string       The algorithm used to compute a digest of the artifact: {sha256|sha512} (default "sha256")
      --hostname string         Configure host to use
  -L, --limit int               Maximum number of attestations to fetch (default 30)
  -o, --owner string            GitHub organization to scope attestation lookup by
      --predicate-type string   Filter attestations by provided predicate type
  -R, --repo string             Repository name in the format <owner>/<repo>
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Download attestations for a local artifact linked with an organization
  $ gh attestation download example.bin -o github
  
  # Download attestations for a local artifact linked with a repository
  $ gh attestation download example.bin -R github/example
  
  # Download attestations for an OCI image linked with an organization
  $ gh attestation download oci://example.com/foo/bar:latest -o github
```

---

## <a id="cmd-attestation-trusted-root"></a>`gh attestation trusted-root`

Output contents for a trusted_root.jsonl file, likely for offline verification.

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

### Synopsis
```bash
gh attestation trusted-root [--tuf-url <url> --tuf-root <file-path>] [--verify-only] [flags]
```

### Flags
```text
--hostname string   Configure host to use
  --tuf-root string   Path to the TUF root.json file on disk
  --tuf-url string    URL to the TUF repository mirror
  --verify-only       Don't output trusted_root.jsonl contents
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Get a trusted_root.jsonl for both Sigstore Public Good and GitHub's instance
  $ gh attestation trusted-root
```

---

## <a id="cmd-attestation-verify"></a>`gh attestation verify`

Verify the integrity and provenance of an artifact using its associated
cryptographically signed attestations.

## Understanding Verification

An attestation is a claim (i.e. a provenance statement) made by an actor
(i.e. a GitHub Actions workflow) regarding a subject (i.e. an artifact).

In order to verify an attestation, you must provide an artifact and validate:
* the identity of the actor that produced the attestation
* the expected attestation predicate type (the nature of the claim)

By default, this command enforces the `https://slsa.dev/provenance/v1`
predicate type. To verify other attestation predicate types use the
`--predicate-type` flag.

The "actor identity" consists of:
* the repository or the repository owner the artifact is linked with
* the Actions workflow that produced the attestation (a.k.a the
  signer workflow)

This identity is then validated against the attestation's certificate's
SourceRepository, SourceRepositoryOwner, and SubjectAlternativeName
(SAN) fields, among others.

It is up to you to decide how precisely you want to enforce this identity.

At a minimum, this command requires either:
* the `--owner` flag (e.g. --owner github), or
* the `--repo` flag (e.g. --repo github/example)

The more precisely you specify the identity, the more control you will
have over the security guarantees offered by the verification process.

Ideally, the path of the signer workflow is also validated using the
`--signer-workflow` or `--cert-identity` flags.

Please note: if your attestation was generated via a reusable workflow then
that reusable workflow is the signer whose identity needs to be validated.
In this situation, you must use either the `--signer-workflow` or
the `--signer-repo` flag.

For more options, see the other available flags.

## Loading Artifacts And Attestations

To specify the artifact, this command requires:
* a file path to an artifact, or
* a container image URI (e.g. `oci://<image-uri>`)
  * (note that if you provide an OCI URL, you must already be authenticated with
its container registry)

By default, this command will attempt to fetch relevant attestations via the
GitHub API using the values provided to `--owner` or  `--repo`.

To instead fetch attestations from your artifact's OCI registry, use the
`--bundle-from-oci` flag.

For offline verification using attestations stored on disk (c.f. the download command)
provide a path to the `--bundle` flag.

When you load attestations with `--bundle` or `--bundle-from-oci`, this command
compares the `--repo` or `--owner` value only with the repository and owner
names recorded in the attestation's certificate when the attestation was
created. It cannot detect whether the repository or owner has since been
renamed, or whether a different repository or owner now uses that name. To
confirm that an attestation belongs to the repository or owner that currently
has the name, omit `--bundle` and `--bundle-from-oci` so that this command
fetches attestations from the GitHub API.

## Additional Policy Enforcement

Given the `--format=json` flag, upon successful verification this
command will output a JSON array containing one entry per verified attestation.

This output can then be used for additional policy enforcement, i.e. by being
piped into a policy engine.

Each object in the array contains two properties:
* an `attestation` object, which contains the bundle that was verified
* a `verificationResult` object, which is a parsed representation of the
  contents of the bundle that was verified.

Within the `verificationResult` object you will find:
* `signature.certificate`, which is a parsed representation of the X.509
  certificate embedded in the attestation,
* `verifiedTimestamps`, an array of objects denoting when the attestation
  was witnessed by a transparency log or a timestamp authority
* `statement`, which contains the `subject` array referencing artifacts,
  the `predicateType` field, and the `predicate` object which contains
  additional, often user-controllable, metadata

IMPORTANT: please note that only the `signature.certificate` and the
`verifiedTimestamps` properties contain values that cannot be
manipulated by the workflow that originated the attestation.

When dealing with attestations created within GitHub Actions, the contents of
`signature.certificate` are populated directly from the OpenID Connect
token that GitHub has generated. The contents of the `verifiedTimestamps`
array are populated from the signed timestamps originating from either a
transparency log or a timestamp authority – and likewise cannot be forged by users.

When designing policy enforcement using this output, special care must be taken
when examining the contents of the `statement.predicate` property:
should an attacker gain access to your workflow's execution context, they
could then falsify the contents of the `statement.predicate`.

To mitigate this attack vector, consider using a "trusted builder": when generating
an artifact, have the build and attestation signing occur within a reusable workflow
whose execution cannot be influenced by input provided through the caller workflow.

See above re: `--signer-workflow`.

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh attestation verify [<file-path> | oci://<image-uri>] [--owner | --repo] [flags]
```

### Flags
```text
-b, --bundle string                Path to bundle on disk, either a single bundle in a JSON file or a JSON lines file with multiple bundles
      --bundle-from-oci              When verifying an OCI image, fetch the attestation bundle from the OCI registry instead of from GitHub
      --cert-identity string         Enforce that the certificate's SubjectAlternativeName matches the provided value exactly
  -i, --cert-identity-regex string   Enforce that the certificate's SubjectAlternativeName matches the provided regex
      --cert-oidc-issuer string      Enforce that the issuer of the OIDC token matches the provided value (default "https://token.actions.githubusercontent.com")
      --custom-trusted-root string   Path to a trusted_root.jsonl file; likely for offline verification
      --deny-self-hosted-runners     Fail verification for attestations generated on self-hosted runners
  -d, --digest-alg string            The algorithm used to compute a digest of the artifact: {sha256|sha512} (default "sha256")
      --format string                Output format: {json}
      --hostname string              Configure host to use
  -q, --jq expression                Filter JSON output using a jq expression
  -L, --limit int                    Maximum number of attestations to fetch (default 30)
      --no-public-good               Do not verify attestations signed with Sigstore public good instance
  -o, --owner string                 GitHub organization to scope attestation lookup by
      --predicate-type string        Enforce that verified attestations' predicate type matches the provided value (default "https://slsa.dev/provenance/v1")
  -R, --repo string                  Repository name in the format <owner>/<repo>
      --signer-digest string         Enforce that the digest associated with the signer workflow matches the provided value
      --signer-repo string           Enforce that the workflow that signed the attestation's repository matches the provided value (<owner>/<repo>)
      --signer-workflow string       Enforce that the workflow that signed the attestation matches the provided value ([host/]<owner>/<repo>/<path>/<to>/<workflow>)
      --source-digest string         Enforce that the digest associated with the source repository matches the provided value
      --source-ref string            Enforce that the git ref associated with the source repository matches the provided value
  -t, --template string              Format JSON output using a Go template; see "gh help formatting"
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Verify an artifact linked with a repository
  $ gh attestation verify example.bin --repo github/example
  
  # Verify an artifact linked with an organization
  $ gh attestation verify example.bin --owner github
  
  # Verify an artifact and output the full verification result
  $ gh attestation verify example.bin --owner github --format json
  
  # Verify an OCI image using attestations stored on disk
  $ gh attestation verify oci://<image-uri> --owner github --bundle sha256:foo.jsonl
  
  # Verify an artifact signed with a reusable workflow
  $ gh attestation verify example.bin --owner github --signer-repo actions/example
```

---

## <a id="cmd-auth"></a>`gh auth`

Authenticate gh and git with GitHub

### Synopsis
```bash
gh auth <command> [flags]

AVAILABLE COMMANDS
  login:         Log in to a GitHub account
  logout:        Log out of a GitHub account
  refresh:       Refresh stored authentication credentials
  setup-git:     Setup git with GitHub CLI
  status:        Display active account and authentication state on each known GitHub host
  switch:        Switch active GitHub account
  token:         Print the authentication token gh uses for a hostname and account
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-auth-login"></a>`gh auth login`

Authenticate with a GitHub host.

The default hostname is `github.com`. This can be overridden using the `--hostname`
flag.

The default authentication mode is a web-based browser flow. After completion, an
authentication token will be stored securely in the system credential store.
If a credential store is not found or there is an issue using it gh will fallback
to writing the token to a plain text file. See `gh auth status` for its
stored location.

Alternatively, use `--with-token` to pass in a personal access token (classic) on standard input.
The minimum required scopes for the token are: `repo`, `read:org`, and `gist`.
Take care when passing a fine-grained personal access token to `--with-token`
as the inherent scoping to certain resources may cause confusing behaviour when interacting with other
resources. Favour setting `GH_TOKEN` for fine-grained personal access token usage.

Alternatively, gh will use the authentication token found in environment variables.
This method is most suitable for "headless" use of gh such as in automation. See
`gh help environment` for more info.

To use gh in GitHub Actions, add `GH_TOKEN: ${{ github.token }}` to `env`.

The git protocol to use for git operations on this host can be set with `--git-protocol`,
or during the interactive prompting. Although login is for a single account on a host, setting
the git protocol will take effect for all users on the host.

Specifying `ssh` for the git protocol will detect existing SSH keys to upload,
prompting to create and upload a new key if one is not found. This can be skipped with
`--skip-ssh-key` flag.

Use `--expiring` to prefer expiring credentials that gh refreshes automatically.
This is a preference, not a guarantee: whether expiring tokens are issued depends on the
host and the OAuth app configuration. A host without support issues a non-expiring token
instead, and a host configured for them may issue expiring tokens even without the flag.
Enable the `expiring_credentials` configuration to prefer expiring credentials
without passing `--expiring` every time, and pass `--expiring=false` to request a
non-expiring token even when that configuration is enabled.
When using expiring credentials for git operations, git 2.46 or newer is recommended so
gh can mark the token as non-cacheable; with older git a credential caching helper may store
and reuse an expired token.

For more information on OAuth scopes, see
<https://docs.github.com/en/developers/apps/building-oauth-apps/scopes-for-oauth-apps/>.

### Synopsis
```bash
gh auth login [flags]
```

### Flags
```text
-c, --clipboard             Copy one-time OAuth device code to clipboard
      --expiring              Prefer expiring credentials that gh refreshes automatically, if the host supports them
  -p, --git-protocol string   The protocol to use for git operations on this host: {ssh|https}
  -h, --hostname string       The hostname of the GitHub instance to authenticate with
      --insecure-storage      Save authentication credentials in plain text instead of credential store
  -s, --scopes strings        Additional authentication scopes to request
      --skip-ssh-key          Skip generate/upload SSH key prompt
  -w, --web                   Open a browser to authenticate
      --with-token            Read token from standard input
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Start interactive setup
  $ gh auth login
  
  # Open a browser to authenticate and copy one-time OAuth code to clipboard
  $ gh auth login --web --clipboard
  
  # Authenticate against github.com by reading the token from a file
  $ gh auth login --with-token < mytoken.txt
  
  # Authenticate with specific host
  $ gh auth login --hostname enterprise.internal
```

---

## <a id="cmd-auth-logout"></a>`gh auth logout`

Remove authentication for a GitHub account.

This command removes the stored authentication configuration
for an account. The authentication configuration is only
removed locally.

This command does not revoke authentication tokens.

To revoke all authentication tokens generated by the GitHub CLI:

1. Visit <https://github.com/settings/applications>
2. Select the "GitHub CLI" application
3. Select "Revoke Access"
4. Select "I understand, revoke access"

Note: this procedure will revoke all authentication tokens ever
generated by the GitHub CLI across all your devices.

For more information about revoking OAuth application tokens, see:
<https://docs.github.com/en/apps/oauth-apps/using-oauth-apps/reviewing-your-authorized-oauth-apps>

### Synopsis
```bash
gh auth logout [flags]
```

### Flags
```text
-h, --hostname string   The hostname of the GitHub instance to log out of
  -u, --user string       The account to log out of
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Select what host and account to log out of via a prompt
  $ gh auth logout
  
  # Log out of a specific host and specific account
  $ gh auth logout --hostname enterprise.internal --user monalisa
```

---

## <a id="cmd-auth-refresh"></a>`gh auth refresh`

Expand or fix the permission scopes for stored credentials for active account.

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

### Synopsis
```bash
gh auth refresh [flags]
```

### Flags
```text
-c, --clipboard               Copy one-time OAuth device code to clipboard
      --expiring                Prefer expiring credentials that gh refreshes automatically, if the host supports them
  -h, --hostname string         The GitHub host to use for authentication
      --insecure-storage        Save authentication credentials in plain text instead of credential store
  -r, --remove-scopes strings   Authentication scopes to remove from gh
      --reset-scopes            Reset authentication scopes to the default minimum set of scopes
  -s, --scopes strings          Additional authentication scopes for gh to have
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
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

---

## <a id="cmd-auth-setup-git"></a>`gh auth setup-git`

This command configures `git` to use GitHub CLI as a credential helper.
For more information on git credential helpers please reference:
<https://git-scm.com/docs/gitcredentials>.

By default, GitHub CLI will be set as the credential helper for all authenticated hosts.
If there is no authenticated hosts the command fails with an error.

Alternatively, use the `--hostname` flag to specify a single host to be configured.
If the host is not authenticated with, the command fails with an error.

### Synopsis
```bash
gh auth setup-git [flags]
```

### Flags
```text
-f, --force --hostname   Force setup even if the host is not known. Must be used in conjunction with --hostname
  -h, --hostname string    The hostname to configure git for
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Configure git to use GitHub CLI as the credential helper for all authenticated hosts
  $ gh auth setup-git
  
  # Configure git to use GitHub CLI as the credential helper for enterprise.internal host
  $ gh auth setup-git --hostname enterprise.internal
```

---

## <a id="cmd-auth-status"></a>`gh auth status`

Display active account and authentication state on each known GitHub host.

For each host, the authentication state of each known account is tested and any issues are included in the output.
Each host section will indicate the active account, which will be used when targeting that host.

If an account on any host (or only the one given via `--hostname`) has authentication issues,
the command will exit with 1 and output to stderr. Note that when using the `--json` option, the command
will always exit with zero regardless of any authentication issues, unless there is a fatal error.

Any expired or near-expiry token that supports refreshing is refreshed automatically, unless `--no-refresh` is given.

To change the active account for a host, see `gh auth switch`.

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh auth status [flags]
```

### Flags
```text
-a, --active            Display the active account only
  -h, --hostname string   Check only a specific hostname's auth status
      --jq expression     Filter JSON output using a jq expression
      --json fields       Output JSON with the specified fields
      --no-refresh        Do not automatically refresh expired tokens
  -t, --show-token        Display the auth token
      --template string   Format JSON output using a Go template; see "gh help formatting"
```

### Inherited Flags
```text
--help   Show help for command

JSON FIELDS
  hosts
```

### Examples
```bash
# Display authentication status for all accounts on all hosts
  $ gh auth status
  
  # Display authentication status for the active account on a specific host
  $ gh auth status --active --hostname github.example.com
  
  # Display tokens in plain text
  $ gh auth status --show-token
  
  # Format authentication status as JSON
  $ gh auth status --json hosts
  
  # Include plain text token in JSON output
  $ gh auth status --json hosts --show-token
  
  # Format hosts as a flat JSON array
  $ gh auth status --json hosts --jq '.hosts | add'
```

---

## <a id="cmd-auth-switch"></a>`gh auth switch`

Switch the active account for a GitHub host.

This command changes the authentication configuration that will
be used when running commands targeting the specified GitHub host.

If the specified host has two accounts, the active account will be switched
automatically. If there are more than two accounts, disambiguation will be
required either through the `--user` flag or an interactive prompt.

For a list of authenticated accounts you can run `gh auth status`.

### Synopsis
```bash
gh auth switch [flags]
```

### Flags
```text
-h, --hostname string   The hostname of the GitHub instance to switch account for
  -u, --user string       The account to switch to
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Select what host and account to switch to via a prompt
  $ gh auth switch
  
  # Switch the active account on a specific host to a specific user
  $ gh auth switch --hostname enterprise.internal --user monalisa
```

---

## <a id="cmd-auth-token"></a>`gh auth token`

This command outputs the authentication token for an account on a given GitHub host.

Without the `--hostname` flag, the default host is chosen.

Without the `--user` flag, the active account for the host is chosen.

If the token is an expired or near-expiry token that supports refreshing, it is refreshed
automatically before being printed, unless `--no-refresh` is given.

### Synopsis
```bash
gh auth token [flags]
```

### Flags
```text
-h, --hostname string   The hostname of the GitHub instance authenticated with
      --no-refresh        Do not automatically refresh an expired token
  -u, --user string       The account to output the token for
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-browse"></a>`gh browse`

Transition from the terminal to the web browser to view and interact with:

- Issues
- Pull requests
- Repository content
- Repository home page
- Repository settings

### Synopsis
```bash
gh browse [<number> | <path> | <commit-sha>] [flags]
```

### Flags
```text
-a, --actions                  Open repository actions
      --blame                    Open blame view for a file
  -b, --branch string            Select another branch by passing in the branch name
  -c, --commit string[="last"]   Select another commit by passing in the commit SHA, default is the last commit
  -n, --no-browser               Print destination URL instead of opening the browser
  -p, --projects                 Open repository projects
  -r, --releases                 Open repository releases
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
  -s, --settings                 Open repository settings
  -w, --wiki                     Open repository wiki
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Open the home page of the current repository
  $ gh browse
  
  # Open the script directory of the current repository
  $ gh browse script/
  
  # Open issue or pull request 217
  $ gh browse 217
  
  # Open commit page
  $ gh browse 77507cd94ccafcf568f8560cfecde965fcfa63
  
  # Open repository settings
  $ gh browse --settings
  
  # Open main.go at line 312
  $ gh browse main.go:312
  
  # Open blame view for main.go at line 312
  $ gh browse main.go:312 --blame
  
  # Open main.go with the repository at head of bug-fix branch
  $ gh browse main.go --branch bug-fix
  
  # Open main.go with the repository at commit 775007cd
  $ gh browse main.go --commit=77507cd94ccafcf568f8560cfecde965fcfa63

ENVIRONMENT VARIABLES
  To configure a web browser other than the default, use the BROWSER environment variable.
```

---

## <a id="cmd-cache"></a>`gh cache`

Work with GitHub Actions caches.

### Synopsis
```bash
gh cache <command> [flags]

AVAILABLE COMMANDS
  delete:        Delete GitHub Actions caches
  list:          List GitHub Actions caches
```

### Flags
```text
-R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
$ gh cache list
  $ gh cache delete --all
```

---

## <a id="cmd-cache-delete"></a>`gh cache delete`

Delete GitHub Actions caches.

Deletion requires authorization with the `repo` scope.

### Synopsis
```bash
gh cache delete [<cache-id> | <cache-key> | --all] [flags]
```

### Flags
```text
-a, --all                          Delete all caches, can be used with --ref to delete all caches for a specific ref
  -r, --ref string                   Delete by cache key and ref, formatted as refs/heads/<branch name> or refs/pull/<number>/merge
      --succeed-on-no-caches --all   Return exit code 0 if no caches found. Must be used in conjunction with --all
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Examples
```bash
# Delete a cache by id
  $ gh cache delete 1234
  
  # Delete a cache by key
  $ gh cache delete cache-key
  
  # Delete a cache by id in a specific repo
  $ gh cache delete 1234 --repo cli/cli
  
  # Delete a cache by key and branch ref
  $ gh cache delete cache-key --ref refs/heads/feature-branch
  
  # Delete a cache by key and PR ref
  $ gh cache delete cache-key --ref refs/pull/<PR-number>/merge
  
  # Delete all caches (exit code 1 on no caches)
  $ gh cache delete --all
  
  # Delete all caches for a specific ref
  $ gh cache delete --all --ref refs/pull/<PR-number>/merge
  
  # Delete all caches (exit code 0 on no caches)
  $ gh cache delete --all --succeed-on-no-caches
```

---

## <a id="cmd-cache-list"></a>`gh cache list`

List GitHub Actions caches

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh cache list [flags]
```

### Aliases
`gh cache ls`

### Flags
```text
-q, --jq expression     Filter JSON output using a jq expression
      --json fields       Output JSON with the specified fields
  -k, --key string        Filter by cache key prefix
  -L, --limit int         Maximum number of caches to fetch (default 30)
  -O, --order string      Order of caches returned: {asc|desc} (default "desc")
  -r, --ref string        Filter by ref, formatted as refs/heads/<branch name> or refs/pull/<number>/merge
  -S, --sort string       Sort fetched caches: {created_at|last_accessed_at|size_in_bytes} (default "last_accessed_at")
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format

JSON FIELDS
  createdAt, id, key, lastAccessedAt, ref, sizeInBytes, version
```

### Examples
```bash
# List caches for current repository
  $ gh cache list
  
  # List caches for specific repository
  $ gh cache list --repo cli/cli
  
  # List caches sorted by least recently accessed
  $ gh cache list --sort last_accessed_at --order asc
  
  # List caches that have keys matching a prefix (or that match exactly)
  $ gh cache list --key key-prefix
  
  # List caches for a specific branch, replace <branch-name> with the actual branch name
  $ gh cache list --ref refs/heads/<branch-name>
  
  # List caches for a specific pull request, replace <pr-number> with the actual pull request number
  $ gh cache list --ref refs/pull/<pr-number>/merge
```

---

## <a id="cmd-codespace"></a>`gh codespace`

Connect to and manage codespaces

### Synopsis
```bash
gh codespace [flags]
```

### Aliases
`gh cs`, ``, `AVAILABLE COMMANDS`, `  code:          Open a codespace in Visual Studio Code`, `  cp:            Copy files between local and remote file systems`, `  create:        Create a codespace`, `  delete:        Delete codespaces`, `  edit:          Edit a codespace`, `  jupyter:       Open a codespace in JupyterLab`, `  list:          List codespaces`, `  logs:          Access codespace logs`, `  ports:         List ports in a codespace`, `  rebuild:       Rebuild a codespace`, `  ssh:           SSH into a codespace`, `  stop:          Stop a running codespace`, `  view:          View details about a codespace`

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-codespace-code"></a>`gh codespace code`

Open a codespace in Visual Studio Code

### Synopsis
```bash
gh codespace code [flags]
```

### Flags
```text
-c, --codespace string    Name of the codespace
      --insiders            Use the insiders version of Visual Studio Code
  -R, --repo string         Filter codespace selection by repository name (user/repo)
      --repo-owner string   Filter codespace selection by repository owner (username or org)
  -w, --web                 Use the web version of Visual Studio Code
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-codespace-cp"></a>`gh codespace cp`

The `cp` command copies files between the local and remote file systems.

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

### Synopsis
```bash
gh codespace cp [-e] [-r] [-- [<scp flags>...]] <sources>... <dest>
```

### Flags
```text
-c, --codespace string    Name of the codespace
  -e, --expand              Expand remote file names on remote shell
  -p, --profile string      Name of the SSH profile to use
  -r, --recursive           Recursively copy directories
  -R, --repo string         Filter codespace selection by repository name (user/repo)
      --repo-owner string   Filter codespace selection by repository owner (username or org)
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
$ gh codespace cp -e README.md 'remote:/workspaces/$RepositoryName/'
  $ gh codespace cp -e 'remote:~/*.go' ./gofiles/
  $ gh codespace cp -e 'remote:/workspaces/myproj/go.{mod,sum}' ./gofiles/
  $ gh codespace cp -e -- -F ~/.ssh/codespaces_config 'remote:~/*.go' ./gofiles/
```

---

## <a id="cmd-codespace-create"></a>`gh codespace create`

Create a codespace

### Synopsis
```bash
gh codespace create [flags]
```

### Flags
```text
-b, --branch string               Repository branch
      --default-permissions         Do not prompt to accept additional permissions requested by the codespace
      --devcontainer-path string    Path to the devcontainer.json file to use when creating codespace
  -d, --display-name string         Display name for the codespace (48 characters or less)
      --idle-timeout duration       Allowed inactivity before codespace is stopped, e.g. "10m", "1h"
  -l, --location string             Location: {EastUs|SouthEastAsia|WestEurope|WestUs2} (determined automatically if not provided)
  -m, --machine string              Hardware specifications for the VM
  -R, --repo string                 Repository name with owner: user/repo
      --retention-period duration   Allowed time after shutting down before the codespace is automatically deleted (maximum 30 days), e.g. "1h", "72h"
  -s, --status                      Show status of post-create command and dotfiles
  -w, --web                         Create codespace from browser, cannot be used with --display-name, --idle-timeout, or --retention-period
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-codespace-delete"></a>`gh codespace delete`

Delete codespaces based on selection criteria.

All codespaces for the authenticated user can be deleted, as well as codespaces for a
specific repository. Alternatively, only codespaces older than N days can be deleted.

Organization administrators may delete any codespace billed to the organization.

### Synopsis
```bash
gh codespace delete [flags]
```

### Flags
```text
--all                 Delete all codespaces
  -c, --codespace string    Name of the codespace
      --days N              Delete codespaces older than N days
  -f, --force               Skip confirmation for codespaces that contain unsaved changes
  -o, --org login           The login handle of the organization (admin-only)
  -R, --repo string         Filter codespace selection by repository name (user/repo)
      --repo-owner string   Filter codespace selection by repository owner (username or org)
  -u, --user username       The username to delete codespaces for (used with --org)
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-codespace-edit"></a>`gh codespace edit`

Edit a codespace

### Synopsis
```bash
gh codespace edit [flags]
```

### Flags
```text
-c, --codespace string      Name of the codespace
  -d, --display-name string   Set the display name
  -m, --machine string        Set hardware specifications for the VM
  -R, --repo string           Filter codespace selection by repository name (user/repo)
      --repo-owner string     Filter codespace selection by repository owner (username or org)
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-codespace-jupyter"></a>`gh codespace jupyter`

Open a codespace in JupyterLab

### Synopsis
```bash
gh codespace jupyter [flags]
```

### Flags
```text
-c, --codespace string    Name of the codespace
  -R, --repo string         Filter codespace selection by repository name (user/repo)
      --repo-owner string   Filter codespace selection by repository owner (username or org)
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-codespace-list"></a>`gh codespace list`

List codespaces of the authenticated user.

Alternatively, organization administrators may list all codespaces billed to the organization.

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh codespace list [flags]
```

### Aliases
`gh codespace ls, gh cs ls`

### Flags
```text
-q, --jq expression     Filter JSON output using a jq expression
      --json fields       Output JSON with the specified fields
  -L, --limit int         Maximum number of codespaces to list (default 30)
  -o, --org login         The login handle of the organization to list codespaces for (admin-only)
  -R, --repo string       Repository name with owner: user/repo
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
  -u, --user username     The username to list codespaces for (used with --org)
  -w, --web               List codespaces in the web browser, cannot be used with --user or --org
```

### Inherited Flags
```text
--help   Show help for command

JSON FIELDS
  createdAt, displayName, gitStatus, lastUsedAt, machineName, name, owner,
  repository, state, vscsTarget
```

---

## <a id="cmd-codespace-logs"></a>`gh codespace logs`

Access codespace logs

### Synopsis
```bash
gh codespace logs [flags]
```

### Flags
```text
-c, --codespace string    Name of the codespace
  -f, --follow              Tail and follow the logs
  -R, --repo string         Filter codespace selection by repository name (user/repo)
      --repo-owner string   Filter codespace selection by repository owner (username or org)
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-codespace-ports"></a>`gh codespace ports`

List ports in a codespace

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh codespace ports [flags]

AVAILABLE COMMANDS
  forward:       Forward ports
  visibility:    Change the visibility of the forwarded port
```

### Flags
```text
-c, --codespace string    Name of the codespace
  -q, --jq expression       Filter JSON output using a jq expression
      --json fields         Output JSON with the specified fields
  -R, --repo string         Filter codespace selection by repository name (user/repo)
      --repo-owner string   Filter codespace selection by repository owner (username or org)
  -t, --template string     Format JSON output using a Go template; see "gh help formatting"
```

### Inherited Flags
```text
--help   Show help for command

JSON FIELDS
  browseUrl, label, sourcePort, visibility
```

---

## <a id="cmd-codespace-ports-forward"></a>`gh codespace ports forward`

Forward ports from a codespace to your local machine.

Ports bind to loopback (`127.0.0.1`) by default. Use `--all-interfaces`
to bind to all interfaces.

### Synopsis
```bash
gh codespace ports forward <remote-port>:<local-port>... [flags]
```

### Flags
```text
--all-interfaces   Listen on all network interfaces
```

### Inherited Flags
```text
-c, --codespace string    Name of the codespace
      --help                Show help for command
  -R, --repo string         Filter codespace selection by repository name (user/repo)
      --repo-owner string   Filter codespace selection by repository owner (username or org)
```

---

## <a id="cmd-codespace-ports-visibility"></a>`gh codespace ports visibility`

Change the visibility of the forwarded port

### Synopsis
```bash
gh codespace ports visibility <port>:{public|private|org}... [flags]
```

### Inherited Flags
```text
-c, --codespace string    Name of the codespace
      --help                Show help for command
  -R, --repo string         Filter codespace selection by repository name (user/repo)
      --repo-owner string   Filter codespace selection by repository owner (username or org)
```

### Examples
```bash
$ gh codespace ports visibility 80:org 3000:private 8000:public
```

---

## <a id="cmd-codespace-rebuild"></a>`gh codespace rebuild`

Rebuilding recreates your codespace.

Your code and any current changes will be preserved. Your codespace will be rebuilt using
your working directory's dev container. A full rebuild also removes cached Docker images.

### Synopsis
```bash
gh codespace rebuild [flags]
```

### Flags
```text
-c, --codespace string    Name of the codespace
      --full                Perform a full rebuild
  -R, --repo string         Filter codespace selection by repository name (user/repo)
      --repo-owner string   Filter codespace selection by repository owner (username or org)
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-codespace-ssh"></a>`gh codespace ssh`

The `ssh` command is used to SSH into a codespace. In its simplest form, you can
run `gh cs ssh`, select a codespace interactively, and connect.

The `ssh` command will automatically create a public/private ssh key pair in the
`~/.ssh` directory if you do not have an existing valid key pair. When selecting the
key pair to use, the preferred order is:

1. Key specified by `-i` in `<ssh-flags>`
2. Automatic key, if it already exists
3. First valid key pair in ssh config (according to `ssh -G`)
4. Automatic key, newly created

The `ssh` command also supports deeper integration with OpenSSH using a `--config`
option that generates per-codespace ssh configuration in OpenSSH format.
Including this configuration in your `~/.ssh/config` improves the user experience
of tools that integrate with OpenSSH, such as Bash/Zsh completion of ssh hostnames,
remote path completion for `scp/rsync/sshfs`, `git` ssh remotes, and so on.

Once that is set up (see the second example below), you can ssh to codespaces as
if they were ordinary remote hosts (using `ssh`, not `gh cs ssh`).

Note that the codespace you are connecting to must have an SSH server pre-installed.
If the docker image being used for the codespace does not have an SSH server,
install it in your `Dockerfile` or, for codespaces that use Debian-based images,
you can add the following to your `devcontainer.json`:

	"features": {
		"ghcr.io/devcontainers/features/sshd:1": {
			"version": "latest"
		}
	}

### Synopsis
```bash
gh codespace ssh [<flags>...] [-- <ssh-flags>...] [<command>]
```

### Flags
```text
-c, --codespace string    Name of the codespace
      --config              Write OpenSSH configuration to stdout
  -d, --debug               Log debug data to a file
      --debug-file string   Path of the file log to
      --profile string      Name of the SSH profile to use
  -R, --repo string         Filter codespace selection by repository name (user/repo)
      --repo-owner string   Filter codespace selection by repository owner (username or org)
      --server-port int     SSH server port number (0 => pick unused)
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
$ gh codespace ssh
  
  $ gh codespace ssh --config > ~/.ssh/codespaces
  $ printf 'Match all\nInclude ~/.ssh/codespaces\n' >> ~/.ssh/config
```

---

## <a id="cmd-codespace-stop"></a>`gh codespace stop`

Stop a running codespace

### Synopsis
```bash
gh codespace stop [flags]
```

### Flags
```text
-c, --codespace string    Name of the codespace
  -o, --org login           The login handle of the organization (admin-only)
  -R, --repo string         Filter codespace selection by repository name (user/repo)
      --repo-owner string   Filter codespace selection by repository owner (username or org)
  -u, --user username       The username to stop codespace for (used with --org)
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-codespace-view"></a>`gh codespace view`

View details about a codespace

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh codespace view [flags]
```

### Flags
```text
-c, --codespace string    Name of the codespace
  -q, --jq expression       Filter JSON output using a jq expression
      --json fields         Output JSON with the specified fields
  -R, --repo string         Filter codespace selection by repository name (user/repo)
      --repo-owner string   Filter codespace selection by repository owner (username or org)
  -t, --template string     Format JSON output using a Go template; see "gh help formatting"
```

### Inherited Flags
```text
--help   Show help for command

JSON FIELDS
  billableOwner, createdAt, devcontainerPath, displayName, environmentId,
  gitStatus, idleTimeoutMinutes, lastUsedAt, location, machineDisplayName,
  machineName, name, owner, prebuild, recentFolders, repository,
  retentionExpiresAt, retentionPeriodDays, state, vscsTarget
```

### Examples
```bash
# Select a codespace from a list of all codespaces you own
  $ gh cs view
  
  # View the details of a specific codespace
  $ gh cs view -c codespace-name-12345
  
  # View the list of all available fields for a codespace
  $ gh cs view --json
  
  # View specific fields for a codespace
  $ gh cs view --json displayName,machineDisplayName,state
```

---

## <a id="cmd-completion"></a>`gh completion`

Generate shell completion scripts for GitHub CLI commands.

When installing GitHub CLI through a package manager, it's possible that
no additional shell configuration is necessary to gain completion support. For
Homebrew, see <https://docs.brew.sh/Shell-Completion>

If you need to set up completions manually, follow the instructions below. The exact
config file locations might vary based on your system. Make sure to restart your
shell before testing whether completions are working.

### bash

First, ensure that you install `bash-completion` using your package manager.

After, add this to your `~/.bash_profile`:

	eval "$(gh completion -s bash)"

### zsh

Generate a `_gh` completion script and put it somewhere in your `$fpath`:

	gh completion -s zsh > /usr/local/share/zsh/site-functions/_gh

Ensure that the following is present in your `~/.zshrc`:

	autoload -U compinit
	compinit -i

Zsh version 5.7 or later is recommended.

### fish

Generate a `gh.fish` completion script:

	gh completion -s fish > ~/.config/fish/completions/gh.fish

### PowerShell

Open your profile script with:

	mkdir -Path (Split-Path -Parent $profile) -ErrorAction SilentlyContinue
	notepad $profile

Add the line and save the file:

	Invoke-Expression -Command $(gh completion -s powershell | Out-String)

### Synopsis
```bash
gh completion -s <shell>
```

### Flags
```text
-s, --shell string   Shell type: {bash|zsh|fish|powershell}
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-config"></a>`gh config`

Display or change configuration settings for gh.

Current respected settings:
- `api_host`: experimental: the hostname to use when making API requests for a GitHub host. Note: this is not a security boundary and requests to the canonical host will remain authenticated
- `git_protocol`: the protocol to use for git clone and push operations `{https | ssh}` (default `https`)
- `editor`: the text editor program to use for authoring text
- `prompt`: toggle interactive prompting in the terminal `{enabled | disabled}` (default `enabled`)
- `prefer_editor_prompt`: toggle preference for editor-based interactive prompting in the terminal `{enabled | disabled}` (default `disabled`)
- `expiring_credentials`: toggle preference for expiring credentials that gh refreshes automatically when logging in `{enabled | disabled}` (default `disabled`)
- `pager`: the terminal pager program to send standard output to
- `http_unix_socket`: the path to a Unix socket through which to make an HTTP connection
- `browser`: the web browser to use for opening URLs
- `clipboard`: whether to copy one-time OAuth device codes to the clipboard `{enabled | disabled}` (default `enabled`)
- `color_labels`: whether to display labels using their RGB hex color codes in terminals that support truecolor `{enabled | disabled}` (default `disabled`)
- `accessible_colors`: whether customizable, 4-bit accessible colors should be used `{enabled | disabled}` (default `disabled`)
- `accessible_prompter`: whether an accessible prompter should be used `{enabled | disabled}` (default `disabled`)
- `spinner`: whether to use an animated spinner as a progress indicator `{enabled | disabled}` (default `enabled`)
- `telemetry`: whether telemetry is enabled, disabled, or logging `{enabled | disabled | log}` (default `enabled`)

### Synopsis
```bash
gh config <command> [flags]

AVAILABLE COMMANDS
  clear-cache:   Clear the cli cache
  get:           Print the value of a given configuration key
  list:          Print a list of configuration keys and values
  set:           Update configuration with a value for the given key
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-config-clear-cache"></a>`gh config clear-cache`

Clear the cli cache

### Synopsis
```bash
gh config clear-cache [flags]
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Clear the cli cache
  $ gh config clear-cache
```

---

## <a id="cmd-config-get"></a>`gh config get`

Print the value of a given configuration key

### Synopsis
```bash
gh config get <key> [flags]
```

### Flags
```text
-h, --host string   Get per-host setting
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
$ gh config get git_protocol
```

---

## <a id="cmd-config-list"></a>`gh config list`

Print a list of configuration keys and values

### Synopsis
```bash
gh config list [flags]
```

### Aliases
`gh config ls`

### Flags
```text
-h, --host string   Get per-host configuration
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-config-set"></a>`gh config set`

Update configuration with a value for the given key

### Synopsis
```bash
gh config set <key> <value> [flags]
```

### Flags
```text
-h, --host string   Set per-host setting
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
$ gh config set editor vim
  $ gh config set editor "code --wait"
  $ gh config set git_protocol ssh --host github.com
  $ gh config set api_host api-gateway.example.com --host example.com
  $ gh config set prompt disabled
```

---

## <a id="cmd-copilot"></a>`gh copilot`

Runs the GitHub Copilot CLI.

Executing the Copilot CLI through `gh` is currently in preview and subject to change.

If already installed, `gh` will execute the Copilot CLI found in your `PATH`.
If the Copilot CLI is not installed, it will be downloaded to /Users/martinlarizzate/.local/share/gh/copilot.

Use `--remove` to remove the downloaded Copilot CLI.

This command is only supported on Windows, Linux, and Darwin, on amd64/x64
or arm64 architectures.

To prevent `gh` from interpreting flags intended for Copilot,
use `--` before Copilot flags and args.

Learn more at https://gh.io/copilot-cli

### Synopsis
```bash
gh copilot [flags] [args]
```

### Flags
```text
--remove   Remove the downloaded Copilot CLI
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Download and run the Copilot CLI
  $ gh copilot
  
  # Run the Copilot CLI
  $ gh copilot -p "Summarize this week's commits" --allow-tool 'shell(git)'
  
  # Remove the Copilot CLI (if installed through gh)
  $ gh copilot --remove
  
  # Run the Copilot CLI help command
  $ gh copilot -- --help
```

---

## <a id="cmd-discussion"></a>`gh discussion`

Working with discussions in the GitHub CLI is in preview and subject to change without notice.

### Synopsis
```bash
gh discussion <command> [flags]

GENERAL COMMANDS
  create:        Create a new discussion (preview)
  list:          List discussions in a repository (preview)

TARGETED COMMANDS
  comment:       Add, edit, or delete a comment or a reply on a discussion (preview)
  edit:          Edit a discussion (preview)
  view:          View a discussion (preview)
```

### Flags
```text
-R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
$ gh discussion list
  $ gh discussion create --category "General" --title "Hello" --body "Hello World!"
  $ gh discussion view 123
```

---

## <a id="cmd-discussion-comment"></a>`gh discussion comment`

Manage comments or replies on a GitHub discussion.

The positional argument can be a discussion number or URL (to add a new
top-level comment), or a comment node ID or comment URL (to reply, edit,
or delete that comment).

When the argument is a discussion number or URL, the default action is to
add a new top-level comment. Likewise, if the argument is a comment URL or ID
the default action is to add a reply.

Use `--edit` to update the comment/reply body, or `--delete` to remove it.

The body can be supplied via `--body`, `--body-file`, or interactively
through an editor.

### Synopsis
```bash
gh discussion comment {<number> | <discussion-url> | <comment-id> | <comment-url>} [flags]
```

### Flags
```text
-b, --body string              Comment body text
  -F, --body-file string         Read body text from file (use "-" to read from standard input)
      --delete                   Delete the specified comment
      --edit                     Edit the specified comment
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
      --yes                      Skip the delete confirmation prompt
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Add a top-level comment to discussion #123
  $ gh discussion comment 123 --body 'Thanks'
  
  # Reply to a comment using its URL
  $ gh discussion comment 'https://github.com/OWNER/REPO/discussions/123#discussioncomment-456' --body 'Thanks'
  
  # Reply to a comment using its node ID
  $ gh discussion comment DC_abc123 --body 'Thanks'
  
  # Edit a comment/reply
  $ gh discussion comment 'https://github.com/OWNER/REPO/discussions/123#discussioncomment-456' --edit --body 'Thanks'
  
  # Delete a comment/reply
  $ gh discussion comment 'https://github.com/OWNER/REPO/discussions/123#discussioncomment-456' --delete
  
  # Delete a comment/reply without confirmation prompt
  $ gh discussion comment 'https://github.com/OWNER/REPO/discussions/123#discussioncomment-456' --delete --yes
```

---

## <a id="cmd-discussion-create"></a>`gh discussion create`

Create a new GitHub Discussion in a repository.

With `--title`, `--body` (or `--body-file`), and `--category`, a discussion is created non-interactively.
Omitting any of these flags triggers interactive prompts when connected to a terminal.

### Synopsis
```bash
gh discussion create [flags]
```

### Flags
```text
-b, --body string              Body for the discussion
  -F, --body-file string         Read body text from file (use "-" to read from stdin)
  -c, --category string          Category name or slug for the discussion
  -l, --label strings            Labels to apply to the discussion
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
  -t, --title string             Title for the discussion
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Create interactively
  $ gh discussion create
  
  # Create non-interactively
  $ gh discussion create --title "My question" --category "Q&A" --body "Details here"
```

---

## <a id="cmd-discussion-edit"></a>`gh discussion edit`

Edit a GitHub Discussion.

Without flags, the command runs interactively when connected to a terminal.
Use flags to update specific fields non-interactively.

### Synopsis
```bash
gh discussion edit {<number> | <discussion-url>} [flags]
```

### Flags
```text
--add-label name           Add labels by name
  -b, --body string              New body for the discussion
  -F, --body-file string         Read body text from file (use "-" to read from standard input)
  -c, --category string          New category name or slug for the discussion
      --remove-label name        Remove labels by name
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
  -t, --title string             New title for the discussion
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Edit interactively
  $ gh discussion edit 123
  
  # Update title, body, and category
  $ gh discussion edit 123 --title "Updated title" --body "Updated body" --category "Ideas"
  
  # Update body from a file
  $ gh discussion edit 123 --body-file body.md
  
  # Add and remove labels
  $ gh discussion edit 123 --add-label "bug,help wanted" --remove-label "stale"
```

---

## <a id="cmd-discussion-list"></a>`gh discussion list`

List discussions in a GitHub repository. By default, only open discussions
are shown.

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh discussion list [flags]
```

### Aliases
`gh discussion ls`

### Flags
```text
--after string             Cursor for the next page of results
      --answered                 Filter by answered state
  -A, --author string            Filter by author
  -c, --category string          Filter by category name or slug
  -q, --jq expression            Filter JSON output using a jq expression
      --json fields              Output JSON with the specified fields
  -l, --label strings            Filter by label
  -L, --limit int                Maximum number of discussions to fetch (default 30)
      --order string             Order of results: {asc|desc} (default "desc")
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
  -S, --search query             Search discussions with query
      --sort string              Sort by field: {created|updated} (default "updated")
  -s, --state string             Filter by state: {open|closed|all} (default "open")
  -t, --template string          Format JSON output using a Go template; see "gh help formatting"
  -w, --web                      List discussions in the web browser
```

### Inherited Flags
```text
--help   Show help for command

JSON FIELDS
  answerChosenAt, answerChosenBy, answered, author, body, category, closed,
  closedAt, createdAt, id, labels, locked, number, stateReason, title, updatedAt,
  url
```

### Examples
```bash
# List open discussions
  $ gh discussion list
  
  # List discussions with a specific category
  $ gh discussion list --category General
  
  # List closed discussions by author
  $ gh discussion list --state closed --author monalisa
  
  # List all discussions (closed or open) by label
  $ gh discussion list --state all --label bug,enhancement
  
  # List answered Q&A discussions as JSON
  $ gh discussion list --answered --json number,title,url
  
  # List unanswered Q&A discussions as JSON
  $ gh discussion list --answered=false --json number,title,url
```

---

## <a id="cmd-discussion-view"></a>`gh discussion view`

Display the title, body, and other information about a discussion.

To see the comments on a discussion, pass `--comments`. A few latest replies
of each comment will also be retrieved regardless of the selected ordering.
When `--comments` is used, terminal output includes the discussion details and comments.
When output is piped or redirected, only the comments are printed.

To see the full reply thread of a single comment, pass a comment node ID or
comment URL as the argument instead of a discussion
(e.g., `https://github.com/OWNER/REPO/discussions/123#discussioncomment-456`).

Pagination and ordering can be controlled via `--order`, `--limit`, and `--after` flags.

Use `--web` to open the discussion or comment in a web browser instead.

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh discussion view {<number> | <discussion-url> | <comment-id> | <comment-url>} [flags]
```

### Flags
```text
--after string             Cursor for the next page
  -c, --comments                 View discussion comments
  -q, --jq expression            Filter JSON output using a jq expression
      --json fields              Output JSON with the specified fields
  -L, --limit int                Maximum number of comments or replies to fetch (default 30)
      --order string             Order of comments or replies: {oldest|newest} (default "newest")
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
  -t, --template string          Format JSON output using a Go template; see "gh help formatting"
  -w, --web                      Open a discussion in the browser
```

### Inherited Flags
```text
--help   Show help for command

JSON FIELDS
  answerChosenAt, answerChosenBy, answered, author, body, category, closed,
  closedAt, comments, createdAt, id, labels, locked, number, reactionGroups,
  state, stateReason, title, updatedAt, url
```

### Examples
```bash
# View a discussion by number
  $ gh discussion view 123
  
  # View a discussion by URL
  $ gh discussion view https://github.com/OWNER/REPO/discussions/123
  
  # View with comments
  $ gh discussion view 123 --comments
  
  # View with oldest comments first
  $ gh discussion view 123 --comments --order oldest
  
  # Limit to 10 comments
  $ gh discussion view 123 --comments --limit 10
  
  # Fetch the next page of comments
  $ gh discussion view 123 --comments --after CURSOR
  
  # View the reply thread of a comment by node ID
  $ gh discussion view DC_abc123
  
  # View the reply thread of a comment by URL
  $ gh discussion view 'https://github.com/OWNER/REPO/discussions/123#discussioncomment-456'
  
  # Paginate through replies
  $ gh discussion view DC_abc123 --limit 10 --after CURSOR
  
  # Open in browser
  $ gh discussion view 123 --web
```

---

## <a id="cmd-extension"></a>`gh extension`

GitHub CLI extensions are repositories that provide additional gh commands.

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

### Synopsis
```bash
gh extension [flags]
```

### Aliases
`gh extensions, gh ext`, ``, `AVAILABLE COMMANDS`, `  browse:        Enter a UI for browsing, adding, and removing extensions`, `  create:        Create a new extension`, `  exec:          Execute an installed extension`, `  install:       Install a gh extension from a repository`, `  list:          List installed extension commands`, `  remove:        Remove an installed extension`, `  search:        Search extensions to the GitHub CLI`, `  upgrade:       Upgrade installed extensions`

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-extension-browse"></a>`gh extension browse`

This command will take over your terminal and run a fully interactive
interface for browsing, adding, and removing gh extensions. A terminal
width greater than 100 columns is recommended. Narrow terminals
automatically use a single-column layout.

To learn how to control this interface, press `?` after running to see
the help text.

Press `q` to quit.

Running this command with `--single-column` should make this command
more intelligible for users who rely on assistive technology like screen
readers or high zoom.

For a more traditional way to discover extensions, see:

	gh ext search

along with `gh ext install`, `gh ext remove`, and `gh repo view`.

### Synopsis
```bash
gh extension browse [flags]
```

### Flags
```text
--debug           Log to /tmp/extBrowse-*
  -s, --single-column   Render TUI with only one column of text
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-extension-create"></a>`gh extension create`

Create a new extension

### Synopsis
```bash
gh extension create [<name>] [flags]
```

### Flags
```text
--precompiled string   Create a precompiled extension. Possible values: go, other
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Use interactively
  $ gh extension create
  
  # Create a script-based extension
  $ gh extension create foobar
  
  # Create a Go extension
  $ gh extension create --precompiled=go foobar
  
  # Create a non-Go precompiled extension
  $ gh extension create --precompiled=other foobar
```

---

## <a id="cmd-extension-exec"></a>`gh extension exec`

---

## <a id="cmd-extension-install"></a>`gh extension install`

Install a GitHub CLI extension from a GitHub or local repository.

For GitHub repositories, the repository argument can be specified in
`OWNER/REPO` format or as a full repository URL.
The URL format is useful when the repository is not hosted on `github.com`.

For remote repositories, the GitHub CLI first looks for the release artifacts assuming
that it's a binary extension i.e. prebuilt binaries provided as part of the release.
In the absence of a release, the repository itself is cloned assuming that it's a
script extension i.e. prebuilt executable or script exists on its root.

The `--pin` flag may be used to specify a tag or commit for binary and script
extensions respectively, the latest version is used otherwise.

For local repositories, often used while developing extensions, use `.` as the
value of the repository argument. Note the following:

- After installing an extension from a locally cloned repository, the GitHub CLI will
manage this extension as a symbolic link (or equivalent mechanism on Windows) pointing
to an executable file with the same name as the repository in the repository's root.
For example, if the repository is named `gh-foobar`, the symbolic link will point
to `gh-foobar` in the extension repository's root.
- When executing the extension, the GitHub CLI will run the executable file found
by following the symbolic link. If no executable file is found, the extension
will fail to execute.
- If the extension is precompiled, the executable file must be built manually and placed
in the repository's root.

For the list of available extensions, see <https://github.com/topics/gh-extension>.

### Synopsis
```bash
gh extension install <repository> [flags]
```

### Flags
```text
--force        Force upgrade extension, or ignore if latest already installed
  --pin string   Pin extension to a release tag or commit ref
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Install an extension from a remote repository hosted on GitHub
  $ gh extension install owner/gh-extension
  
  # Install an extension from a remote repository via full URL
  $ gh extension install https://my.ghes.com/owner/gh-extension
  
  # Install an extension from a local repository in the current working directory
  $ gh extension install .
```

---

## <a id="cmd-extension-list"></a>`gh extension list`

List installed extension commands

### Synopsis
```bash
gh extension list [flags]
```

### Aliases
`gh ext ls, gh extension ls, gh extensions ls`

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-extension-remove"></a>`gh extension remove`

Remove an installed extension

### Synopsis
```bash
gh extension remove <name> [flags]
```

### Aliases
`gh ext uninstall, gh extension uninstall, gh extensions uninstall`

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-extension-search"></a>`gh extension search`

Search for gh extensions.

With no arguments, this command prints out the first 30 extensions
available to install sorted by number of stars. More extensions can
be fetched by specifying a higher limit with the `--limit` flag.

When connected to a terminal, this command prints out three columns.
The first has a ✓ if the extension is already installed locally. The
second is the full name of the extension repository in `OWNER/REPO`
format. The third is the extension's description.

When not connected to a terminal, the ✓ character is rendered as the
word "installed" but otherwise the order and content of the columns
are the same.

This command behaves similarly to `gh search repos` but does not
support as many search qualifiers. For a finer grained search of
extensions, try using:

	gh search repos --topic "gh-extension"

and adding qualifiers as needed. See `gh help search repos` to learn
more about repository search.

For listing just the extensions that are already installed locally,
see:

	gh ext list

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh extension search [<query>] [flags]
```

### Flags
```text
-q, --jq expression     Filter JSON output using a jq expression
      --json fields       Output JSON with the specified fields
      --license strings   Filter based on license type
  -L, --limit int         Maximum number of extensions to fetch (default 30)
      --order string      Order of repositories returned, ignored unless '--sort' flag is specified: {asc|desc} (default "desc")
      --owner strings     Filter on owner
      --sort string       Sort fetched repositories: {forks|help-wanted-issues|stars|updated} (default "best-match")
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
  -w, --web               Open the search query in the web browser
```

### Inherited Flags
```text
--help   Show help for command

JSON FIELDS
  createdAt, defaultBranch, description, forksCount, fullName, hasDownloads,
  hasIssues, hasPages, hasProjects, hasWiki, homepage, id, isArchived, isDisabled,
  isFork, isPrivate, language, license, name, openIssuesCount, owner, pushedAt,
  size, stargazersCount, updatedAt, url, visibility, watchersCount
```

### Examples
```bash
# List the first 30 extensions sorted by star count, descending
  $ gh ext search
  
  # List more extensions
  $ gh ext search --limit 300
  
  # List extensions matching the term "branch"
  $ gh ext search branch
  
  # List extensions owned by organization "github"
  $ gh ext search --owner github
  
  # List extensions, sorting by recently updated, ascending
  $ gh ext search --sort updated --order asc
  
  # List extensions, filtering by license
  $ gh ext search --license MIT
  
  # Open search results in the browser
  $ gh ext search -w
```

---

## <a id="cmd-extension-upgrade"></a>`gh extension upgrade`

Upgrade installed extensions

### Synopsis
```bash
gh extension upgrade {<name> | --all} [flags]
```

### Flags
```text
--all       Upgrade all extensions
  --dry-run   Only display upgrades
  --force     Force upgrade extension
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-gist"></a>`gh gist`

Work with GitHub gists.

### Synopsis
```bash
gh gist <command> [flags]

AVAILABLE COMMANDS
  clone:         Clone a gist locally
  create:        Create a new gist
  delete:        Delete a gist
  edit:          Edit one of your gists
  list:          List your gists
  rename:        Rename a file in a gist
  view:          View a gist
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-gist-clone"></a>`gh gist clone`

Clone a GitHub gist locally.

A gist can be supplied as argument in either of the following formats:
- by ID, e.g. `5b0e0062eb8e9654adad7bb1d81cc75f`
- by URL, e.g. `https://gist.github.com/OWNER/5b0e0062eb8e9654adad7bb1d81cc75f`

Pass additional `git clone` flags by listing them after `--`.

### Synopsis
```bash
gh gist clone <gist> [<directory>] [-- <gitflags>...]
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-gist-create"></a>`gh gist create`

Create a new GitHub gist with given contents.

Gists can be created from one or multiple files. Alternatively, pass `-` as
filename to read from standard input.

By default, gists are secret; use `--public` to make publicly listed ones.

### Synopsis
```bash
gh gist create [<filename>... | <pattern>... | -] [flags]
```

### Aliases
`gh gist new`

### Flags
```text
-d, --desc string       A description for this gist
  -f, --filename string   Provide a filename to be used when reading from standard input
  -p, --public            List the gist publicly (default "secret")
  -w, --web               Open the web browser with created gist
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Publish file 'hello.py' as a public gist
  $ gh gist create --public hello.py
  
  # Create a gist with a description
  $ gh gist create hello.py -d "my Hello-World program in Python"
  
  # Create a gist containing several files
  $ gh gist create hello.py world.py cool.txt
  
  # Create a gist containing several files using patterns
  $ gh gist create *.md *.txt artifact.*
  
  # Read from standard input to create a gist
  $ gh gist create -
  
  # Create a gist from output piped from another command
  $ cat cool.txt | gh gist create
```

---

## <a id="cmd-gist-delete"></a>`gh gist delete`

Delete a GitHub gist.

To delete a gist interactively, use `gh gist delete` with no arguments.

To delete a gist non-interactively, supply the gist id or url.

### Synopsis
```bash
gh gist delete {<id> | <url>} [flags]
```

### Flags
```text
--yes   Confirm deletion without prompting
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Delete a gist interactively
  $ gh gist delete
  
  # Delete a gist non-interactively
  $ gh gist delete 1234
```

---

## <a id="cmd-gist-edit"></a>`gh gist edit`

Edit one of your gists

### Synopsis
```bash
gh gist edit {<id> | <url>} [<filename>] [flags]
```

### Flags
```text
-a, --add string        Add a new file to the gist
  -d, --desc string       New description for the gist
  -f, --filename string   Select a file to edit
  -r, --remove string     Remove a file from the gist
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Select a gist to edit interactively
  $ gh gist edit
  
  # Edit a gist file in the default editor
  $ gh gist edit 1234567890abcdef1234567890abcdef
  
  # Edit a specific file in the gist
  $ gh gist edit 1234567890abcdef1234567890abcdef --filename hello.py
  
  # Replace a gist file with content from a local file
  $ gh gist edit 1234567890abcdef1234567890abcdef --filename hello.py hello.py
  
  # Add a new file to the gist
  $ gh gist edit 1234567890abcdef1234567890abcdef --add newfile.py
  
  # Change the description of the gist
  $ gh gist edit 1234567890abcdef1234567890abcdef --desc "new description"
  
  # Remove a file from the gist
  $ gh gist edit 1234567890abcdef1234567890abcdef --remove hello.py
```

---

## <a id="cmd-gist-list"></a>`gh gist list`

List gists from your user account.

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

### Synopsis
```bash
gh gist list [flags]
```

### Aliases
`gh gist ls`

### Flags
```text
--filter expression   Filter gists using a regular expression
      --include-content     Include gists' file content when filtering
  -L, --limit int           Maximum number of gists to fetch (default 10)
      --public              Show only public gists
      --secret              Show only secret gists
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# List all secret gists from your user account
  $ gh gist list --secret
  
  # Find all gists from your user account mentioning "octo" anywhere
  $ gh gist list --filter octo --include-content
```

---

## <a id="cmd-gist-rename"></a>`gh gist rename`

Rename a file in the given gist ID / URL.

### Synopsis
```bash
gh gist rename {<id> | <url>} <old-filename> <new-filename> [flags]
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-gist-view"></a>`gh gist view`

View the given gist or select from recent gists.

### Synopsis
```bash
gh gist view [<id> | <url>] [flags]
```

### Flags
```text
--allow-escape-sequences   Allow printing terminal escape sequences
  -f, --filename string          Display a single file from the gist
      --files                    List file names from the gist
  -r, --raw                      Print raw instead of rendered gist contents
  -w, --web                      Open gist in the browser
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-gpg-key"></a>`gh gpg-key`

Manage GPG keys registered with your GitHub account.

### Synopsis
```bash
gh gpg-key <command> [flags]

AVAILABLE COMMANDS
  add:           Add a GPG key to your GitHub account
  delete:        Delete a GPG key from your GitHub account
  list:          Lists GPG keys in your GitHub account
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-gpg-key-add"></a>`gh gpg-key add`

Add a GPG key to your GitHub account

### Synopsis
```bash
gh gpg-key add [<key-file>] [flags]
```

### Flags
```text
-t, --title string   Title for the new key
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-gpg-key-delete"></a>`gh gpg-key delete`

Delete a GPG key from your GitHub account

### Synopsis
```bash
gh gpg-key delete <key-id> [flags]
```

### Flags
```text
-y, --yes   Skip the confirmation prompt
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-gpg-key-list"></a>`gh gpg-key list`

Lists GPG keys in your GitHub account

### Synopsis
```bash
gh gpg-key list [flags]
```

### Aliases
`gh gpg-key ls`

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-issue"></a>`gh issue`

Work with GitHub issues.

### Synopsis
```bash
gh issue <command> [flags]

GENERAL COMMANDS
  create:        Create a new issue
  list:          List issues in a repository
  status:        Show status of relevant issues

TARGETED COMMANDS
  artifact:      Work with issue artifacts (preview)
  close:         Close issue
  comment:       Add a comment to an issue
  delete:        Delete issue
  develop:       Manage linked branches for an issue
  edit:          Edit issues
  lock:          Lock issue conversation
  pin:           Pin an issue
  reopen:        Reopen issue
  transfer:      Transfer issue to another repository
  unlock:        Unlock issue conversation
  unpin:         Unpin an issue
  view:          View an issue
```

### Flags
```text
-R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
$ gh issue list
  $ gh issue create --label bug
  $ gh issue view 123 --web
```

---

## <a id="cmd-issue-artifact"></a>`gh issue artifact`

Working with issue artifacts in the GitHub CLI is in preview and subject to change without notice.

Issue artifacts are Markdown documents, HTML documents and links attached to an issue.
They are not GitHub Actions artifacts; to download those, use `gh run download`.

### Synopsis
```bash
gh issue artifact <command> [flags]

AVAILABLE COMMANDS
  create:        Create issue artifacts (preview)
  delete:        Delete issue artifacts (preview)
  download:      Download issue artifacts (preview)
  edit:          Edit an issue artifact (preview)
  list:          List artifacts on an issue (preview)
  view:          View an issue artifact (preview)
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

---

## <a id="cmd-issue-artifact-create"></a>`gh issue artifact create`

Create one artifact for each file or URL. A text file becomes a document
named after the file; add `#<name>` to choose a different name. A `.html` or
`.htm` file becomes an HTML document. A URL, or a `.url` Internet Shortcut
file, becomes a link; a URL is named after its host.

Artifact names can't contain some characters, such as parentheses. When a
file's name has them, they're removed: `plan (1).md` is named `plan 1.md`.

Use `--body` to create a single document from text, or `--body-file` to create
one artifact from a file (`-` reads standard input). `--name` sets its name.

Documents are saved as `generic`, and HTML documents as `embedded_html`. Use
`--type` to set the type of every document instead, whatever the file
extension. A plan currently behaves the same as a generic document.

### Synopsis
```bash
gh issue artifact create {<issue-number> | <issue-url>} [<file>[#<name>] | <url>]... [flags]
```

### Aliases
`gh issue artifact new`

### Flags
```text
--attach file      Attach an image or video file, in '<file>#<image alt text>' format
  -b, --body string      Content for a single document
  -F, --body-file file   Read content for a single artifact from file (use "-" to read from standard input)
      --name string      Name for a single artifact
      --type string      Type for documents: {generic|plan|embedded_html}
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Examples
```bash
# Create a document from a file
  $ gh issue artifact create 142 signin-plan.md
  
  # Create documents from two files, naming the first
  $ gh issue artifact create 142 'docs/signin-plan.md#Sign-in plan' oauth-research.md
  
  # Create an HTML document from a file
  $ gh issue artifact create 142 menu-prototype.html
  
  # Create a link with a name
  $ gh issue artifact create 142 https://github.com/monalisa/monas-cafe/wiki/OAuth-runbook --name 'Staging OAuth runbook'
  
  # Create a document from standard input
  $ cat order-sync.log | gh issue artifact create 142 --body-file - --name 'Order sync log'
  
  # Upload an image that the document references
  $ gh issue artifact create 142 signin-plan.md --attach ./signin-flow.png
```

---

## <a id="cmd-issue-artifact-delete"></a>`gh issue artifact delete`

Delete artifacts from an issue. A deleted artifact can't be restored.

Name artifacts by their issue and numbers, or by their URLs, which must all be
on one issue. `<issue>` is an issue number or URL.

In a terminal, deletion requires confirmation. `--yes` skips the prompt and is
required when prompting is unavailable.

### Synopsis
```bash
gh issue artifact delete {<issue> <artifact-number>... | <artifact-url>...} [flags]
```

### Flags
```text
--yes   Confirm deletion without prompting
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Examples
```bash
# Delete artifact 2 from issue 142
  $ gh issue artifact delete 142 2
  
  # Delete two artifacts without a prompt
  $ gh issue artifact delete 142 2 5 --yes
```

---

## <a id="cmd-issue-artifact-download"></a>`gh issue artifact download`

Download issue artifacts to files. Without artifact numbers, every artifact
on the issue is downloaded. Artifacts can also be named by their URLs, which
must all be on one issue. `<issue>` is an issue number or URL.

Each file is named `<number>-<name>`. Markdown documents end in `.md`, HTML
documents in `.html`, and links are saved as `.url` Internet Shortcut files.
If a file already exists, that artifact fails unless you use `--clobber` to
overwrite it or `--skip-existing` to skip it.

Use `--dir` to choose the directory to download files into, `--output` to
choose the path for a single artifact, or `--output -` to print its content.
Use `--version` with a single artifact to download an earlier version from
its edit history.

### Synopsis
```bash
gh issue artifact download {<issue> [<artifact-number>...] | <artifact-url>...} [flags]
```

### Flags
```text
--clobber          Overwrite existing files of the same name
  -D, --dir directory    The directory to download files into (default ".")
  -O, --output file      The file to write a single artifact to (use "-" to write to standard output)
      --skip-existing    Skip downloading when files of the same name exist
      --version number   Download the version with this number from the edit history
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Examples
```bash
# Download every artifact on issue 142
  $ gh issue artifact download 142
  
  # Download two artifacts into a folder
  $ gh issue artifact download 142 2 5 --dir notes
  
  # Print one artifact's content
  $ gh issue artifact download 142 2 --output -
  
  # Download an earlier version of one artifact
  $ gh issue artifact download 142 2 --version 5
```

---

## <a id="cmd-issue-artifact-edit"></a>`gh issue artifact edit`

Rename an issue artifact or replace its content. The type never changes, so a
link's new content must be an http(s) URL or a `.url` Internet Shortcut file.

Name the artifact by its issue and number, or by its URL. `<issue>` is an
issue number or URL.

With only `--attach`, the attachments are appended to the current content.

With `--restore-version`, an earlier version's name and content are saved as a
new version. `gh issue artifact view` shows the edit history.

### Synopsis
```bash
gh issue artifact edit {<issue> <artifact-number> | <artifact-url>} [flags]
```

### Flags
```text
--attach file              Attach an image or video file, in '<file>#<image alt text>' format
  -b, --body string              New content; for a link, a URL
  -F, --body-file file           Read new content from file (use "-" to read from standard input)
      --name string              New name
      --restore-version number   Restore the version with this number from the edit history
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Examples
```bash
# Rename an artifact
  $ gh issue artifact edit 142 2 --name 'OAuth callback plan v2'
  
  # Replace a document's content with a file
  $ gh issue artifact edit 142 2 --body-file 2-OAuth-callback-plan.md
  
  # Point a link at a new URL
  $ gh issue artifact edit 142 3 --body https://github.com/monalisa/monas-cafe/wiki/OAuth-runbook-v2
  
  # Append an image to a document
  $ gh issue artifact edit 142 2 --attach ./signin-flow.png
  
  # Restore an earlier version
  $ gh issue artifact edit 142 2 --restore-version 5
```

---

## <a id="cmd-issue-artifact-list"></a>`gh issue artifact list`

List the artifacts on an issue, in number order. Every artifact is listed
unless you set `--limit`.

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh issue artifact list {<issue-number> | <issue-url>} [flags]
```

### Aliases
`gh issue artifact ls`

### Flags
```text
-q, --jq expression     Filter JSON output using a jq expression
      --json fields       Output JSON with the specified fields
  -L, --limit int         Maximum number of artifacts to fetch
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
      --type string       Filter by type: {generic|plan|link|embedded_html}
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format

JSON FIELDS
  body, bodyHtml, createdAt, creator, description, id, name, number, type,
  updatedAt, updatedByActor, url
```

### Examples
```bash
# List the artifacts on issue 142
  $ gh issue artifact list 142
  
  # List only links
  $ gh issue artifact list 142 --type link
  
  # Print artifact numbers and names as JSON
  $ gh issue artifact list 142 --json number,name
```

---

## <a id="cmd-issue-artifact-view"></a>`gh issue artifact view`

Display an issue artifact's name, type, authors, content, and edit history. A
link shows its URL.

Name the artifact by its issue and number, or by its URL. `<issue>` is an
issue number or URL.

By default, the current version is shown. Use `--version` to show an earlier
version from the edit history.

With `--web`, open a document's page on GitHub, or a link's URL.

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh issue artifact view {<issue> <artifact-number> | <artifact-url>} [flags]
```

### Flags
```text
-q, --jq expression     Filter JSON output using a jq expression
      --json fields       Output JSON with the specified fields
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
      --version number    Show the version with this number from the edit history
  -w, --web               Open a document's page on GitHub, or a link's URL
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format

JSON FIELDS
  body, bodyHtml, createdAt, creator, description, id, name, number, type,
  updatedAt, updatedByActor, url, versions
```

### Examples
```bash
# View artifact 2 on issue 142
  $ gh issue artifact view 142 2
  
  # View an earlier version
  $ gh issue artifact view 142 2 --version 5
  
  # View an artifact by its URL
  $ gh issue artifact view https://github.com/monalisa/monas-cafe/issues/142/artifacts/3
  
  # Open a link artifact in the browser
  $ gh issue artifact view 142 3 --web
  
  # Print an artifact's body
  $ gh issue artifact view 142 2 --json body --jq .body
```

---

## <a id="cmd-issue-close"></a>`gh issue close`

Close issue

### Synopsis
```bash
gh issue close {<number> | <url>} [flags]
```

### Flags
```text
-c, --comment string        Leave a closing comment
      --duplicate-of string   Mark as duplicate of another issue by number or URL
  -r, --reason string         Reason for closing: {completed|not planned|duplicate}
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Examples
```bash
# Close issue
  $ gh issue close 123
  
  # Close issue and add a closing comment
  $ gh issue close 123 --comment "Closing this issue"
  
  # Close issue as a duplicate of issue #456
  $ gh issue close 123 --duplicate-of 456
  
  # Close issue as not planned
  $ gh issue close 123 --reason "not planned"
```

---

## <a id="cmd-issue-comment"></a>`gh issue comment`

Add a comment to a GitHub issue.

Without body text or attachments supplied through flags, the command will
interactively prompt for the comment text.

Use `--attach` to upload an image or video. If the body already references an
attached file, such as `![alt](./login.png)`, that reference is rewritten to point
at the uploaded asset. Paths in a `--body-file` are relative to its directory,
falling back to the working directory. Any attached file the body does not reference
is appended to the end of the comment.
You can attach up to 50 files per command.

Alt text for an image follows the path after `#`, as in
`--attach './login.png#The login error state'`. Without it the filename is used.
A reference already in the body keeps the alt text written there. Video renders
as a player and has no alt text, so it cannot be given any.

### Synopsis
```bash
gh issue comment {<number> | <url>} [flags]
```

### Flags
```text
--attach file      Attach an image or video file, in '<file>#<image alt text>' format
  -b, --body text        The comment body text
  -F, --body-file file   Read body text from file (use "-" to read from standard input)
      --create-if-none   Create a new comment if no comments are found. Can be used only with --edit-last
      --delete-last      Delete the last comment of the current user
      --edit-last        Edit the last comment of the current user
  -e, --editor           Skip prompts and open the text editor to write the body in
  -w, --web              Open the web browser to write the comment
      --yes              Skip the delete confirmation prompt when --delete-last is provided
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Examples
```bash
# Add a comment to an issue
  $ gh issue comment 12 --body "Hi from GitHub CLI"
  
  # Attach a screenshot, with alt text after "#"
  $ gh issue comment 12 --attach './login.png#The login error state'
  
  # Attach multiple files by repeating the flag
  $ gh issue comment 12 --attach ./before.png --attach ./after.png
```

---

## <a id="cmd-issue-create"></a>`gh issue create`

Create an issue on GitHub.

Use `--attach` to upload an image or video. The attachment is appended to the
body. If the body references an attached file, such as `![alt](./login.png)`, that
reference is rewritten to point at the uploaded asset instead. Paths in a
`--body-file` are relative to its directory, falling back to the working directory.
You can attach up to 50 files per command.

Alt text for an image follows the path after `#`, as in
`--attach './login.png#The login error state'`. Without it the filename is used.
A reference already in the body keeps the alt text written there. Video renders
as a player and has no alt text, so it cannot be given any.

If some attachments upload and others fail, the issue is still created with the
ones that succeeded. The command then exits with a non-zero status, but the new
issue's URL is still printed to stdout.

Adding an issue to projects requires authorization with the `project` scope.
To authorize, run `gh auth refresh -s project`.

The `--assignee` flag supports the following special values:
- `@me`: assign yourself
- `@copilot`: assign Copilot (not supported on GitHub Enterprise Server)

### Synopsis
```bash
gh issue create [flags]
```

### Aliases
`gh issue new`

### Flags
```text
-a, --assignee login       Assign people by their login. Use "@me" to self-assign.
      --attach file          Attach an image or video file, in '<file>#<image alt text>' format
      --blocked-by numbers   Mark the new issue as blocked by these issue numbers or URLs
      --blocking numbers     Mark the new issue as blocking these issue numbers or URLs
  -b, --body string          Supply a body. Will prompt for one otherwise.
  -F, --body-file file       Read body text from file (use "-" to read from standard input)
  -e, --editor               Skip prompts and open the text editor to write the title and body in. The first line is the title and the remaining text is the body.
  -l, --label name           Add labels by name
  -m, --milestone name       Add the issue to a milestone by name
      --parent number        Add the new issue as a sub-issue of the specified parent number or URL
  -p, --project title        Add the issue to projects by title
      --recover string       Recover input from a failed run of create
  -T, --template name        Template name to use as starting body text
  -t, --title string         Supply a title. Will prompt for one otherwise.
      --type name            Set the issue type by name
  -w, --web                  Open the browser to create an issue
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Examples
```bash
$ gh issue create --title "I found a bug" --body "Nothing works"
  $ gh issue create --attach './login.png#The login error state'
  $ gh issue create --attach ./before.png --attach ./after.png
  $ gh issue create --label "bug,help wanted"
  $ gh issue create --label bug --label "help wanted"
  $ gh issue create --assignee monalisa,hubot
  $ gh issue create --assignee "@me"
  $ gh issue create --assignee "@copilot"
  $ gh issue create --project "Roadmap"
  $ gh issue create --template "Bug Report"
  $ gh issue create --type Bug
  $ gh issue create --parent 100
  $ gh issue create --parent https://github.com/cli/go-gh/issues/42
  $ gh issue create --blocked-by 200,201 --blocking 300
```

---

## <a id="cmd-issue-delete"></a>`gh issue delete`

Delete issue

### Synopsis
```bash
gh issue delete {<number> | <url>} [flags]
```

### Flags
```text
--yes   Confirm deletion without prompting
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

---

## <a id="cmd-issue-develop"></a>`gh issue develop`

Manage linked branches for an issue.

When using the `--base` flag, the new development branch will be created from the specified
remote branch. The new branch will be configured as the base branch for pull requests created using
`gh pr create`.

### Synopsis
```bash
gh issue develop {<number> | <url>} [flags]
```

### Flags
```text
-b, --base string          Name of the remote branch you want to make your new branch from
      --branch-repo string   Name or URL of the repository where you want to create your new branch
  -c, --checkout             Checkout the branch after creating it
  -l, --list                 List linked branches for the issue
  -n, --name string          Name of the branch to create
      --worktree path        Check out the branch into a worktree at the given path
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Examples
```bash
# List branches for issue 123
  $ gh issue develop --list 123
  
  # List branches for issue 123 in repo cli/cli
  $ gh issue develop --list --repo cli/cli 123
  
  # Create a branch for issue 123 based on the my-feature branch
  $ gh issue develop 123 --base my-feature
  
  # Create a branch for issue 123 and check it out
  $ gh issue develop 123 --checkout
  
  # Create a branch for issue 123 and check it out in a worktree
  $ gh issue develop 123 --checkout --worktree /path/to/wt-feature
  
  # Create a branch in repo monalisa/cli for issue 123 in repo cli/cli
  $ gh issue develop 123 --repo cli/cli --branch-repo monalisa/cli
```

---

## <a id="cmd-issue-edit"></a>`gh issue edit`

Edit one or more issues within the same repository.

Editing issues' projects requires authorization with the `project` scope.
To authorize, run `gh auth refresh -s project`.

Use `--attach` to upload an image or video to a single issue. Without a body
flag the issue keeps the body it already has and the attachment is appended to it.
If the body references an attached file, such as `![alt](./login.png)`, that
reference is rewritten to point at the uploaded asset instead. Paths in a
`--body-file` are relative to its directory, falling back to the working directory.
You can attach up to 50 files per command.

Alt text for an image follows the path after `#`, as in
`--attach './login.png#The login error state'`. Without it the filename is used.
A reference already in the body keeps the alt text written there. Video renders
as a player and has no alt text, so it cannot be given any.

If some attachments upload and others fail, the issue is still updated with the
ones that succeeded. The command then exits with a non-zero status, but the edited
issue URLs are still printed to stdout.

The `--add-assignee` and `--remove-assignee` flags both support
the following special values:
- `@me`: assign or unassign yourself
- `@copilot`: assign or unassign Copilot (not supported on GitHub Enterprise Server)

### Synopsis
```bash
gh issue edit {<numbers> | <urls>} [flags]
```

### Flags
```text
--add-assignee login         Add assigned users by their login. Use "@me" to assign yourself, or "@copilot" to assign Copilot.
      --add-blocked-by number      Add 'blocked by' relationships by issue number or URL
      --add-blocking number        Add 'blocking' relationships by issue number or URL
      --add-label name             Add labels by name
      --add-project title          Add the issue to projects by title
      --add-sub-issue number       Add sub-issues by number or URL
      --attach file                Attach an image or video file, in '<file>#<image alt text>' format
  -b, --body string                Set the new body.
  -F, --body-file file             Read body text from file (use "-" to read from standard input)
  -m, --milestone name             Edit the milestone the issue belongs to by name
      --parent number              Set the parent issue by number or URL
      --remove-assignee login      Remove assigned users by their login. Use "@me" to unassign yourself, or "@copilot" to unassign Copilot.
      --remove-blocked-by number   Remove 'blocked by' relationships by issue number or URL
      --remove-blocking number     Remove 'blocking' relationships by issue number or URL
      --remove-label name          Remove labels by name
      --remove-milestone           Remove the milestone association from the issue
      --remove-parent              Remove the parent issue
      --remove-project title       Remove the issue from projects by title
      --remove-sub-issue number    Remove sub-issues by number or URL
      --remove-type                Remove the issue type from the issue
  -t, --title string               Set the new title.
      --type name                  Set the issue type by name
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Examples
```bash
$ gh issue edit 23 --title "I found a bug" --body "Nothing works"
  $ gh issue edit 23 --add-label "bug,help wanted" --remove-label "core"
  $ gh issue edit 23 --add-assignee "@me" --remove-assignee monalisa,hubot
  $ gh issue edit 23 --add-assignee "@copilot"
  $ gh issue edit 23 --add-project "Roadmap" --remove-project v1,v2
  $ gh issue edit 23 --milestone "Version 1"
  $ gh issue edit 23 --remove-milestone
  $ gh issue edit 23 --body-file body.txt
  $ gh issue edit 23 --attach './login.png#The login error state'
  $ gh issue edit 23 --attach ./before.png --attach ./after.png
  $ gh issue edit 23 34 --add-label "help wanted"
  $ gh issue edit 23 --type Bug
  $ gh issue edit 23 --remove-type
  $ gh issue edit 23 --parent 100
  $ gh issue edit 23 --remove-parent
  $ gh issue edit 100 --add-sub-issue 123,124
  $ gh issue edit 123 --add-blocked-by 200 --add-blocking 300,301
```

---

## <a id="cmd-issue-list"></a>`gh issue list`

List issues in a GitHub repository. By default, this only lists open issues.

The search query syntax is documented here:
<https://docs.github.com/en/search-github/searching-on-github/searching-issues-and-pull-requests>

On supported GitHub hosts, advanced issue search syntax can be used in the
`--search` query. For more information about advanced issue search, see:
<https://docs.github.com/en/issues/tracking-your-work-with-issues/using-issues/filtering-and-searching-issues-and-pull-requests#building-advanced-filters-for-issues>

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh issue list [flags]
```

### Aliases
`gh issue ls`

### Flags
```text
--app string         Filter by GitHub App author
  -a, --assignee string    Filter by assignee
  -A, --author string      Filter by author (use --app to filter by a GitHub App)
  -q, --jq expression      Filter JSON output using a jq expression
      --json fields        Output JSON with the specified fields
  -l, --label strings      Filter by label
  -L, --limit int          Maximum number of issues to fetch (default 30)
      --mention string     Filter by mention
  -m, --milestone string   Filter by milestone number or title
  -S, --search query       Search issues with query
  -s, --state string       Filter by state: {open|closed|all} (default "open")
  -t, --template string    Format JSON output using a Go template; see "gh help formatting"
      --type name          Filter by issue type name
  -w, --web                List issues in the web browser
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format

JSON FIELDS
  assignees, author, blockedBy, blocking, body, closed, closedAt,
  closedByPullRequestsReferences, comments, createdAt, id, isPinned, issueType,
  labels, milestone, number, parent, projectCards, projectItems, reactionGroups,
  state, stateReason, subIssues, subIssuesSummary, title, updatedAt, url
```

### Examples
```bash
$ gh issue list --label "bug" --label "help wanted"
  $ gh issue list --author monalisa
  $ gh issue list --app dependabot
  $ gh issue list --assignee "@me"
  $ gh issue list --milestone "The big 1.0"
  $ gh issue list --search "error no:assignee sort:created-asc"
  $ gh issue list --state all
  $ gh issue list --type Bug
```

---

## <a id="cmd-issue-lock"></a>`gh issue lock`

Lock issue conversation

### Synopsis
```bash
gh issue lock {<number> | <url>} [flags]
```

### Flags
```text
-r, --reason string   Optional reason for locking conversation (off_topic, resolved, spam, too_heated).
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

---

## <a id="cmd-issue-pin"></a>`gh issue pin`

Pin an issue to a repository.

The issue can be specified by issue number or URL.

### Synopsis
```bash
gh issue pin {<number> | <url>} [flags]
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Examples
```bash
# Pin an issue to the current repository
  $ gh issue pin 23
  
  # Pin an issue by URL
  $ gh issue pin https://github.com/owner/repo/issues/23
  
  # Pin an issue to specific repository
  $ gh issue pin 23 --repo owner/repo
```

---

## <a id="cmd-issue-reopen"></a>`gh issue reopen`

Reopen issue

### Synopsis
```bash
gh issue reopen {<number> | <url>} [flags]
```

### Flags
```text
-c, --comment string   Add a reopening comment
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

---

## <a id="cmd-issue-status"></a>`gh issue status`

Show status of relevant issues

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh issue status [flags]
```

### Flags
```text
-q, --jq expression     Filter JSON output using a jq expression
      --json fields       Output JSON with the specified fields
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format

JSON FIELDS
  assignees, author, blockedBy, blocking, body, closed, closedAt,
  closedByPullRequestsReferences, comments, createdAt, id, isPinned, issueType,
  labels, milestone, number, parent, projectCards, projectItems, reactionGroups,
  state, stateReason, subIssues, subIssuesSummary, title, updatedAt, url
```

---

## <a id="cmd-issue-transfer"></a>`gh issue transfer`

Transfer issue to another repository

### Synopsis
```bash
gh issue transfer {<number> | <url>} <destination-repo> [flags]
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

---

## <a id="cmd-issue-unlock"></a>`gh issue unlock`

Unlock issue conversation

### Synopsis
```bash
gh issue unlock {<number> | <url>} [flags]
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

---

## <a id="cmd-issue-unpin"></a>`gh issue unpin`

Unpin an issue from a repository.

The issue can be specified by issue number or URL.

### Synopsis
```bash
gh issue unpin {<number> | <url>} [flags]
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Examples
```bash
# Unpin issue from the current repository
  $ gh issue unpin 23
  
  # Unpin issue by URL
  $ gh issue unpin https://github.com/owner/repo/issues/23
  
  # Unpin an issue from specific repository
  $ gh issue unpin 23 --repo owner/repo
```

---

## <a id="cmd-issue-view"></a>`gh issue view`

Display the title, body, and other information about an issue.

When `--comments` is used, terminal output includes the issue details and comments.
When output is piped or redirected, only the comments are printed.

With `--web` flag, open the issue in a web browser instead.

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh issue view {<number> | <url>} [flags]
```

### Flags
```text
-c, --comments          View issue comments
  -q, --jq expression     Filter JSON output using a jq expression
      --json fields       Output JSON with the specified fields
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
  -w, --web               Open an issue in the browser
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format

JSON FIELDS
  assignees, author, blockedBy, blocking, body, closed, closedAt,
  closedByPullRequestsReferences, comments, createdAt, id, isPinned, issueType,
  labels, milestone, number, parent, projectCards, projectItems, reactionGroups,
  state, stateReason, subIssues, subIssuesSummary, title, updatedAt, url
```

---

## <a id="cmd-label"></a>`gh label`

Work with GitHub labels.

### Synopsis
```bash
gh label <command> [flags]

AVAILABLE COMMANDS
  clone:         Clones labels from one repository to another
  create:        Create a new label
  delete:        Delete a label from a repository
  edit:          Edit a label
  list:          List labels in a repository
```

### Flags
```text
-R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-label-clone"></a>`gh label clone`

Clones labels from a source repository to a destination repository on GitHub.
By default, the destination repository is the current repository.

All labels from the source repository will be copied to the destination
repository. Labels in the destination repository that are not in the source
repository will not be deleted or modified.

Labels from the source repository that already exist in the destination
repository will be skipped. You can overwrite existing labels in the
destination repository using the `--force` flag.

### Synopsis
```bash
gh label clone <source-repository> [flags]
```

### Flags
```text
-f, --force   Overwrite labels in the destination repository
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Examples
```bash
# Clone and overwrite labels from cli/cli repository into the current repository
  $ gh label clone cli/cli --force
  
  # Clone labels from cli/cli repository into octocat/cli repository
  $ gh label clone cli/cli --repo octocat/cli
```

---

## <a id="cmd-label-create"></a>`gh label create`

Create a new label on GitHub, or update an existing one with `--force`.

Must specify name for the label. The description and color are optional.
If a color isn't provided, a random one will be chosen.

The label color needs to be 6 character hex value.

### Synopsis
```bash
gh label create <name> [flags]
```

### Flags
```text
-c, --color string         Color of the label
  -d, --description string   Description of the label
  -f, --force                Update the label color and description if label already exists
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Examples
```bash
# Create new bug label
  $ gh label create bug --description "Something isn't working" --color E99695
```

---

## <a id="cmd-label-delete"></a>`gh label delete`

Delete a label from a repository

### Synopsis
```bash
gh label delete <name> [flags]
```

### Flags
```text
--yes   Confirm deletion without prompting
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

---

## <a id="cmd-label-edit"></a>`gh label edit`

Update a label on GitHub.

A label can be renamed using the `--name` flag.

The label color needs to be 6 character hex value.

### Synopsis
```bash
gh label edit <name> [flags]
```

### Flags
```text
-c, --color string         Color of the label
  -d, --description string   Description of the label
  -n, --name string          New name of the label
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Examples
```bash
# Update the color of the bug label
  $ gh label edit bug --color FF0000
  
  # Rename and edit the description of the bug label
  $ gh label edit bug --name big-bug --description "Bigger than normal bug"
```

---

## <a id="cmd-label-list"></a>`gh label list`

Display labels in a GitHub repository.

When using the `--search` flag results are sorted by best match of the query.
This behavior cannot be configured with the `--order` or `--sort` flags.

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh label list [flags]
```

### Aliases
`gh label ls`

### Flags
```text
-q, --jq expression     Filter JSON output using a jq expression
      --json fields       Output JSON with the specified fields
  -L, --limit int         Maximum number of labels to fetch (default 30)
      --order string      Order of labels returned: {asc|desc} (default "asc")
  -S, --search string     Search label names and descriptions
      --sort string       Sort fetched labels: {created|name} (default "created")
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
  -w, --web               List labels in the web browser
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format

JSON FIELDS
  color, createdAt, description, id, isDefault, name, updatedAt, url
```

### Examples
```bash
# Sort labels by name
  $ gh label list --sort name
  
  # Find labels with "bug" in the name or description
  $ gh label list --search bug
```

---

## <a id="cmd-licenses"></a>`gh licenses`

View license information for third-party libraries used in this build of the GitHub CLI.

### Synopsis
```bash
gh licenses [flags]
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-org"></a>`gh org`

Work with GitHub organizations.

### Synopsis
```bash
gh org <command> [flags]

GENERAL COMMANDS
  list:          List organizations for the authenticated user.
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
$ gh org list
```

---

## <a id="cmd-org-list"></a>`gh org list`

List organizations for the authenticated user.

### Synopsis
```bash
gh org list [flags]
```

### Aliases
`gh org ls`

### Flags
```text
-L, --limit int   Maximum number of organizations to list (default 30)
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# List the first 30 organizations
  $ gh org list
  
  # List more organizations
  $ gh org list --limit 100
```

---

## <a id="cmd-pr"></a>`gh pr`

Work with GitHub pull requests.

### Synopsis
```bash
gh pr <command> [flags]

GENERAL COMMANDS
  create:        Create a pull request
  list:          List pull requests in a repository
  status:        Show status of relevant pull requests

TARGETED COMMANDS
  checkout:      Check out a pull request in git
  checks:        Show CI status for a single pull request
  close:         Close a pull request
  comment:       Add a comment to a pull request
  diff:          View changes in a pull request
  edit:          Edit a pull request
  lock:          Lock pull request conversation
  merge:         Merge a pull request
  ready:         Mark a pull request as ready for review
  reopen:        Reopen a pull request
  revert:        Revert a pull request
  review:        Add a review to a pull request
  unlock:        Unlock pull request conversation
  update-branch: Update a pull request branch
  view:          View a pull request
```

### Flags
```text
-R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
$ gh pr checkout 353
  $ gh pr create --fill
  $ gh pr view --web
```

---

## <a id="cmd-pr-checkout"></a>`gh pr checkout`

Check out a pull request in git

### Synopsis
```bash
gh pr checkout [<number> | <url> | <branch>] [flags]
```

### Aliases
`gh pr co`

### Flags
```text
-b, --branch string        Local branch name to use (default [the name of the head branch])
      --detach               Checkout PR with a detached HEAD
  -f, --force                Reset the existing local branch to the latest state of the pull request
      --recurse-submodules   Update all submodules after checkout
      --worktree path        Check out the pull request into a worktree at the given path
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Examples
```bash
# Interactively select a PR from the 10 most recent to check out
  $ gh pr checkout
  
  # Checkout a specific PR
  $ gh pr checkout 32
  $ gh pr checkout https://github.com/OWNER/REPO/pull/32
  $ gh pr checkout feature
  $ gh pr checkout 32 --branch feature --worktree /path/to/wt-feature
```

---

## <a id="cmd-pr-checks"></a>`gh pr checks`

Show CI status for a single pull request.

Without an argument, the pull request that belongs to the current branch
is selected.

When the `--json` flag is used, it includes a `bucket` field, which categorizes
the `state` field into `pass`, `fail`, `pending`, `skipping`, or `cancel`.

Additional exit codes:
	8: Checks pending

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh pr checks [<number> | <url> | <branch>] [flags]
```

### Flags
```text
--fail-fast         Exit watch mode on first check failure
  -i, --interval int      Refresh interval in seconds in watch mode (default 10)
  -q, --jq expression     Filter JSON output using a jq expression
      --json fields       Output JSON with the specified fields
      --required          Only show checks that are required
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
      --watch             Watch checks until they finish
  -w, --web               Open the web browser to show details about checks
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format

JSON FIELDS
  bucket, completedAt, description, event, link, name, startedAt, state, workflow
```

---

## <a id="cmd-pr-close"></a>`gh pr close`

Close a pull request

### Synopsis
```bash
gh pr close {<number> | <url> | <branch>} [flags]
```

### Flags
```text
-c, --comment string   Leave a closing comment
  -d, --delete-branch    Delete the local and remote branch after close
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

---

## <a id="cmd-pr-comment"></a>`gh pr comment`

Add a comment to a GitHub pull request.

Without body text or attachments supplied through flags, the command will
interactively prompt for the comment text.

Use `--attach` to upload an image or video. If the body already references an
attached file, such as `![alt](./login.png)`, that reference is rewritten to point
at the uploaded asset. Paths in a `--body-file` are relative to its directory,
falling back to the working directory. Any attached file the body does not reference
is appended to the end of the comment.
You can attach up to 50 files per command.

Alt text for an image follows the path after `#`, as in
`--attach './login.png#The login error state'`. Without it the filename is used.
A reference already in the body keeps the alt text written there. Video renders
as a player and has no alt text, so it cannot be given any.

### Synopsis
```bash
gh pr comment [<number> | <url> | <branch>] [flags]
```

### Flags
```text
--attach file      Attach an image or video file, in '<file>#<image alt text>' format
  -b, --body text        The comment body text
  -F, --body-file file   Read body text from file (use "-" to read from standard input)
      --create-if-none   Create a new comment if no comments are found. Can be used only with --edit-last
      --delete-last      Delete the last comment of the current user
      --edit-last        Edit the last comment of the current user
  -e, --editor           Skip prompts and open the text editor to write the body in
  -w, --web              Open the web browser to write the comment
      --yes              Skip the delete confirmation prompt when --delete-last is provided
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Examples
```bash
# Add a comment to a pull request
  $ gh pr comment 13 --body "Hi from GitHub CLI"
  
  # Attach a screenshot, with alt text after "#"
  $ gh pr comment 13 --attach './login.png#The login error state'
  
  # Attach multiple files by repeating the flag
  $ gh pr comment 13 --attach ./before.png --attach ./after.png
```

---

## <a id="cmd-pr-create"></a>`gh pr create`

Create a pull request on GitHub.

Upon success, the URL of the created pull request will be printed.

When the current branch isn't fully pushed to a git remote, a prompt will ask where
to push the branch and offer an option to fork the base repository. Any fork created this
way will only have the default branch of the upstream repository. Use `--head` to
explicitly skip any forking or pushing behavior.

`--head` supports `<user>:<branch>` syntax to select a head repo owned by `<user>`.
Using an organization as the `<user>` is currently not supported.
For more information, see <https://github.com/cli/cli/issues/10093>

A prompt will also ask for the title and the body of the pull request. Use `--title` and
`--body` to skip this, or use `--fill` to autofill these values from git commits.
It's important to notice that if the `--title` and/or `--body` are also provided
alongside `--fill`, the values specified by `--title` and/or `--body` will
take precedence and overwrite any autofilled content.

The base branch for the created PR can be specified using the `--base` flag. If not provided,
the value of `gh-merge-base` git branch config will be used. If not configured, the repository's
default branch will be used. Run `git config branch.{current}.gh-merge-base {base}` to configure
the current branch to use the specified merge base.

Link an issue to the pull request by referencing the issue in the body of the pull
request. If the body text mentions `Fixes #123` or `Closes #123`, the referenced issue
will automatically get closed when the pull request gets merged.

Use `--attach` to upload an image or video. The attachment is appended to the
body. If the body references an attached file, such as `![alt](./login.png)`, that
reference is rewritten to point at the uploaded asset instead. Paths in a
`--body-file` are relative to its directory, falling back to the working directory.
You can attach up to 50 files per command.

Alt text for an image follows the path after `#`, as in
`--attach './login.png#The login error state'`. Without it the filename is used.
A reference already in the body keeps the alt text written there. Video renders
as a player and has no alt text, so it cannot be given any.

If some attachments upload and others fail, the pull request is still created with the
ones that succeeded. The command then exits with a non-zero status, but the new pull
request's URL is still printed to stdout.

By default, users with write access to the base repository can push new commits to the
head branch of the pull request. Disable this with `--no-maintainer-edit`.

Adding a pull request to projects requires authorization with the `project` scope.
To authorize, run `gh auth refresh -s project`.

### Synopsis
```bash
gh pr create [flags]
```

### Aliases
`gh pr new`

### Flags
```text
-a, --assignee login       Assign people by their login. Use "@me" to self-assign.
      --attach file          Attach an image or video file, in '<file>#<image alt text>' format
  -B, --base branch          The branch into which you want your code merged
  -b, --body string          Body for the pull request
  -F, --body-file file       Read body text from file (use "-" to read from standard input)
  -d, --draft                Mark pull request as a draft
      --dry-run              Print details instead of creating the PR. May still push git changes.
  -e, --editor               Skip prompts and open the text editor to write the title and body in. The first line is the title and the remaining text is the body.
  -f, --fill                 Use commit info for title and body
      --fill-first           Use first commit info for title and body
      --fill-verbose         Use commits msg+body for description
  -H, --head branch          The branch that contains commits for your pull request (default [current branch])
  -l, --label name           Add labels by name
  -m, --milestone name       Add the pull request to a milestone by name
      --no-maintainer-edit   Disable maintainer's ability to modify pull request
  -p, --project title        Add the pull request to projects by title
      --recover string       Recover input from a failed run of create
  -r, --reviewer handle      Request reviews from people or teams by their handle
  -T, --template file        Template file to use as starting body text
  -t, --title string         Title for the pull request
  -w, --web                  Open the web browser to create a pull request
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Examples
```bash
$ gh pr create --title "The bug is fixed" --body "Everything works again"
  $ gh pr create --reviewer monalisa,hubot  --reviewer myorg/team-name
  $ gh pr create --project "Roadmap"
  $ gh pr create --base develop --head monalisa:feature
  $ gh pr create --template "pull_request_template.md"
  $ gh pr create --attach './login.png#The login error state'
  $ gh pr create --attach ./before.png --attach ./after.png
```

---

## <a id="cmd-pr-diff"></a>`gh pr diff`

View changes in a pull request.

Without an argument, the pull request that belongs to the current branch
is selected.

With `--web` flag, open the pull request diff in a web browser instead.

Use `--exclude` to filter out files matching a glob pattern. The pattern
uses forward slashes as path separators on all platforms. You can repeat
the flag to exclude multiple patterns.

By default, terminal escape sequences in the diff are neutralized, since
they could manipulate your terminal. Pass `--allow-escape-sequences` to
print the diff verbatim, for example when piping a patch to another program.

### Synopsis
```bash
gh pr diff [<number> | <url> | <branch>] [flags]
```

### Flags
```text
--allow-escape-sequences   Allow printing terminal escape sequences
      --color string             Use color in diff output: {always|never|auto} (default "auto")
  -e, --exclude patterns         Exclude files matching glob patterns from the diff
      --name-only                Display only names of changed files
      --patch                    Display diff in patch format
  -w, --web                      Open the pull request diff in the browser
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Examples
```bash
# See diff for current branch
  $ gh pr diff
  
  # See diff for a specific PR
  $ gh pr diff 123
  
  # Exclude files from diff output
  $ gh pr diff --exclude '*.yml' --exclude 'generated/*'
  
  # Exclude matching files by name
  $ gh pr diff --name-only --exclude '*.generated.*'
```

---

## <a id="cmd-pr-edit"></a>`gh pr edit`

Edit a pull request.

Without an argument, the pull request that belongs to the current branch
is selected.

Editing a pull request's projects requires authorization with the `project` scope.
To authorize, run `gh auth refresh -s project`.

Use `--attach` to upload an image or video. Without a body flag the pull
request keeps the body it already has and the attachment is appended to it. If the
body references an attached file, such as `![alt](./login.png)`, that reference
is rewritten to point at the uploaded asset instead. Paths in a `--body-file` are
relative to its directory, falling back to the working directory.
You can attach up to 50 files per command.

Alt text for an image follows the path after `#`, as in
`--attach './login.png#The login error state'`. Without it the filename is used.
A reference already in the body keeps the alt text written there. Video renders
as a player and has no alt text, so it cannot be given any.

If some attachments upload and others fail, the pull request is still updated with the
ones that succeeded. The command then exits with a non-zero status, but the pull
request's URL is still printed to stdout.

The `--add-assignee` and `--remove-assignee` flags both support
the following special values:
- `@me`: assign or unassign yourself
- `@copilot`: assign or unassign Copilot (not supported on GitHub Enterprise Server)

The `--add-reviewer` and `--remove-reviewer` flags support
the following special value:
- `@copilot`: request or remove review from Copilot (not supported on GitHub Enterprise Server)

### Synopsis
```bash
gh pr edit [<number> | <url> | <branch>] [flags]
```

### Flags
```text
--add-assignee login      Add assigned users by their login. Use "@me" to assign yourself, or "@copilot" to assign Copilot.
      --add-label name          Add labels by name
      --add-project title       Add the pull request to projects by title
      --add-reviewer login      Add or re-request reviewers by their login. Use "@copilot" to request review from Copilot.
      --attach file             Attach an image or video file, in '<file>#<image alt text>' format
  -B, --base branch             Change the base branch for this pull request
  -b, --body string             Set the new body.
  -F, --body-file file          Read body text from file (use "-" to read from standard input)
  -m, --milestone name          Edit the milestone the pull request belongs to by name
      --remove-assignee login   Remove assigned users by their login. Use "@me" to unassign yourself, or "@copilot" to unassign Copilot.
      --remove-label name       Remove labels by name
      --remove-milestone        Remove the milestone association from the pull request
      --remove-project title    Remove the pull request from projects by title
      --remove-reviewer login   Remove reviewers by their login. Use "@copilot" to remove review request from Copilot.
  -t, --title string            Set the new title.
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Examples
```bash
# Edit the title and body of a pull request
  $ gh pr edit 23 --title "I found a bug" --body "Nothing works"
  
  # Use a file as the body
  $ gh pr edit 23 --body-file body.txt
  
  # Append a screenshot to the body, with alt text after "#"
  $ gh pr edit 23 --attach './login.png#The login error state'
  
  # Append multiple files by repeating the flag
  $ gh pr edit 23 --attach ./before.png --attach ./after.png
  
  # Manage labels
  $ gh pr edit 23 --add-label "bug,help wanted" --remove-label "core"
  
  # Manage reviewers
  $ gh pr edit 23 --add-reviewer monalisa,hubot --remove-reviewer myorg/team-name
  
  # Re-request review
  $ gh pr edit 23 --add-reviewer monalisa
  
  # Request a review from GitHub Copilot
  $ gh pr edit 23 --add-reviewer "@copilot"
  
  # Manage assignees
  $ gh pr edit 23 --add-assignee "@me" --remove-assignee monalisa,hubot
  
  # Assign GitHub Copilot
  $ gh pr edit 23 --add-assignee "@copilot"
  
  # Manage projects and milestones
  $ gh pr edit 23 --add-project "Roadmap" --remove-project v1,v2
  $ gh pr edit 23 --milestone "Version 1"
  $ gh pr edit 23 --remove-milestone
```

---

## <a id="cmd-pr-list"></a>`gh pr list`

List pull requests in a GitHub repository. By default, this only lists open PRs.

The search query syntax is documented here:
<https://docs.github.com/en/search-github/searching-on-github/searching-issues-and-pull-requests>

On supported GitHub hosts, advanced issue search syntax can be used in the
`--search` query. For more information about advanced issue search, see:
<https://docs.github.com/en/issues/tracking-your-work-with-issues/using-issues/filtering-and-searching-issues-and-pull-requests#building-advanced-filters-for-issues>

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh pr list [flags]
```

### Aliases
`gh pr ls`

### Flags
```text
--app string        Filter by GitHub App author
  -a, --assignee string   Filter by assignee
  -A, --author string     Filter by author (use --app to filter by a GitHub App)
  -B, --base string       Filter by base branch
  -d, --draft             Filter by draft state
  -H, --head string       Filter by head branch ("<owner>:<branch>" syntax not supported)
  -q, --jq expression     Filter JSON output using a jq expression
      --json fields       Output JSON with the specified fields
  -l, --label strings     Filter by label
  -L, --limit int         Maximum number of items to fetch (default 30)
  -S, --search query      Search pull requests with query
  -s, --state string      Filter by state: {open|closed|merged|all} (default "open")
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
  -w, --web               List pull requests in the web browser
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format

JSON FIELDS
  additions, assignees, author, autoMergeRequest, baseRefName, baseRefOid, body,
  changedFiles, closed, closedAt, closingIssuesReferences, comments, commits,
  createdAt, deletions, files, fullDatabaseId, headRefName, headRefOid,
  headRepository, headRepositoryOwner, id, isCrossRepository, isDraft, labels,
  latestReviews, maintainerCanModify, mergeCommit, mergeStateStatus, mergeable,
  mergedAt, mergedBy, milestone, number, potentialMergeCommit, projectCards,
  projectItems, reactionGroups, reviewDecision, reviewRequests, reviews, state,
  statusCheckRollup, title, updatedAt, url
```

### Examples
```bash
# List PRs authored by you
  $ gh pr list --author "@me"
  
  # List PRs opened by a GitHub App such as Dependabot
  $ gh pr list --app dependabot
  
  # List PRs with a specific head branch name
  $ gh pr list --head "typo"
  
  # List only PRs with all of the given labels
  $ gh pr list --label bug --label "priority 1"
  
  # Filter PRs using search syntax
  $ gh pr list --search "status:success review:required"
  
  # Find a PR that introduced a given commit
  $ gh pr list --search "<SHA>" --state merged
```

---

## <a id="cmd-pr-lock"></a>`gh pr lock`

Lock pull request conversation

### Synopsis
```bash
gh pr lock {<number> | <url>} [flags]
```

### Flags
```text
-r, --reason string   Optional reason for locking conversation (off_topic, resolved, spam, too_heated).
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

---

## <a id="cmd-pr-merge"></a>`gh pr merge`

Merge a pull request on GitHub.

Without an argument, the pull request that belongs to the current branch
is selected.

When targeting a branch that requires a merge queue, no merge strategy is required.
If required checks have not yet passed, auto-merge will be enabled.
If required checks have passed, the pull request will be added to the merge queue.
To bypass a merge queue and merge directly, pass the `--admin` flag.

### Synopsis
```bash
gh pr merge [<number> | <url> | <branch>] [flags]
```

### Flags
```text
--admin                   Use administrator privileges to merge a pull request that does not meet requirements
  -A, --author-email text       Email text for merge commit author
      --auto                    Automatically merge only after necessary requirements are met
  -b, --body text               Body text for the merge commit
  -F, --body-file file          Read body text from file (use "-" to read from standard input)
  -d, --delete-branch           Delete the local and remote branch after merge
      --disable-auto            Disable auto-merge for this pull request
      --match-head-commit SHA   Commit SHA that the pull request head must match to allow merge
  -m, --merge                   Merge the commits with the base branch
  -r, --rebase                  Rebase the commits onto the base branch
  -s, --squash                  Squash the commits into one commit and merge it into the base branch
  -t, --subject text            Subject text for the merge commit
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

---

## <a id="cmd-pr-ready"></a>`gh pr ready`

Mark a pull request as ready for review.

Without an argument, the pull request that belongs to the current branch
is marked as ready.

If supported by your plan, convert to draft with `--undo`

### Synopsis
```bash
gh pr ready [<number> | <url> | <branch>] [flags]
```

### Flags
```text
--undo   Convert a pull request to "draft"
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

---

## <a id="cmd-pr-reopen"></a>`gh pr reopen`

Reopen a pull request

### Synopsis
```bash
gh pr reopen {<number> | <url> | <branch>} [flags]
```

### Flags
```text
-c, --comment string   Add a reopening comment
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

---

## <a id="cmd-pr-revert"></a>`gh pr revert`

Revert a pull request

### Synopsis
```bash
gh pr revert {<number> | <url> | <branch>} [flags]
```

### Flags
```text
-b, --body string      Body for the revert pull request
  -F, --body-file file   Read body text from file (use "-" to read from standard input)
  -d, --draft            Mark revert pull request as a draft
  -t, --title string     Title for the revert pull request
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

---

## <a id="cmd-pr-review"></a>`gh pr review`

Add a review to a pull request.

Without an argument, the pull request that belongs to the current branch is reviewed.

### Synopsis
```bash
gh pr review [<number> | <url> | <branch>] [flags]
```

### Flags
```text
-a, --approve           Approve pull request
  -b, --body string       Specify the body of a review
  -F, --body-file file    Read body text from file (use "-" to read from standard input)
  -c, --comment           Comment on a pull request
  -r, --request-changes   Request changes on a pull request
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Examples
```bash
# Approve the pull request of the current branch
  $ gh pr review --approve
  
  # Leave a review comment for the current branch
  $ gh pr review --comment -b "interesting"
  
  # Add a review for a specific pull request
  $ gh pr review 123
  
  # Request changes on a specific pull request
  $ gh pr review 123 -r -b "needs more ASCII art"
```

---

## <a id="cmd-pr-status"></a>`gh pr status`

Show status of relevant pull requests.

The status shows a summary of pull requests that includes information such as
pull request number, title, CI checks, reviews, etc.

To see more details of CI checks, run `gh pr checks`.

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh pr status [flags]
```

### Flags
```text
-c, --conflict-status   Display the merge conflict status of each pull request
  -q, --jq expression     Filter JSON output using a jq expression
      --json fields       Output JSON with the specified fields
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format

JSON FIELDS
  additions, assignees, author, autoMergeRequest, baseRefName, baseRefOid, body,
  changedFiles, closed, closedAt, closingIssuesReferences, comments, commits,
  createdAt, deletions, files, fullDatabaseId, headRefName, headRefOid,
  headRepository, headRepositoryOwner, id, isCrossRepository, isDraft, labels,
  latestReviews, maintainerCanModify, mergeCommit, mergeStateStatus, mergeable,
  mergedAt, mergedBy, milestone, number, potentialMergeCommit, projectCards,
  projectItems, reactionGroups, reviewDecision, reviewRequests, reviews, state,
  statusCheckRollup, title, updatedAt, url
```

---

## <a id="cmd-pr-unlock"></a>`gh pr unlock`

Unlock pull request conversation

### Synopsis
```bash
gh pr unlock {<number> | <url>} [flags]
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

---

## <a id="cmd-pr-update-branch"></a>`gh pr update-branch`

Update a pull request branch with latest changes of the base branch.

Without an argument, the pull request that belongs to the current branch is selected.

The default behavior is to update with a merge commit (i.e., merging the base branch
into the PR's branch). To reconcile the changes with rebasing on top of the base
branch, the `--rebase` option should be provided.

### Synopsis
```bash
gh pr update-branch [<number> | <url> | <branch>] [flags]
```

### Flags
```text
--rebase   Update PR branch by rebasing on top of latest base branch
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Examples
```bash
$ gh pr update-branch 23
  $ gh pr update-branch 23 --rebase
  $ gh pr update-branch 23 --repo owner/repo
```

---

## <a id="cmd-pr-view"></a>`gh pr view`

Display the title, body, and other information about a pull request.

Without an argument, the pull request that belongs to the current branch
is displayed.

When `--comments` is used, terminal output includes the pull request details, comments,
and reviews. When output is piped or redirected, only comments and reviews are printed.

With `--web` flag, open the pull request in a web browser instead.

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh pr view [<number> | <url> | <branch>] [flags]
```

### Flags
```text
-c, --comments          View pull request comments
  -q, --jq expression     Filter JSON output using a jq expression
      --json fields       Output JSON with the specified fields
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
  -w, --web               Open a pull request in the browser
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format

JSON FIELDS
  additions, assignees, author, autoMergeRequest, baseRefName, baseRefOid, body,
  changedFiles, closed, closedAt, closingIssuesReferences, comments, commits,
  createdAt, deletions, files, fullDatabaseId, headRefName, headRefOid,
  headRepository, headRepositoryOwner, id, isCrossRepository, isDraft, labels,
  latestReviews, maintainerCanModify, mergeCommit, mergeStateStatus, mergeable,
  mergedAt, mergedBy, milestone, number, potentialMergeCommit, projectCards,
  projectItems, reactionGroups, reviewDecision, reviewRequests, reviews, state,
  statusCheckRollup, title, updatedAt, url
```

---

## <a id="cmd-preview"></a>`gh preview`

Preview commands are for testing, demonstrative, and development purposes only.
They should be considered unstable and can change at any time.

### Synopsis
```bash
gh preview <command> [flags]

AVAILABLE COMMANDS
  prompter:      Execute a test program to preview the prompter
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-preview-prompter"></a>`gh preview prompter`

Execute a test program to preview the prompter.
Without an argument, all prompts will be run.

Available prompt types:
- select
- multi-select
- multi-select-with-search
- input
- password
- confirm
- auth-token
- confirm-deletion
- input-hostname
- markdown-editor

### Synopsis
```bash
gh preview prompter [prompt type] [flags]
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-project"></a>`gh project`

Work with GitHub Projects.

The minimum required scope for the token is: `project`.
You can verify your token scope by running `gh auth status` and
add the `project` scope by running `gh auth refresh -s project`.

### Synopsis
```bash
gh project <command> [flags]

AVAILABLE COMMANDS
  close:         Close a project
  copy:          Copy a project
  create:        Create a project
  delete:        Delete a project
  edit:          Edit a project
  field-create:  Create a field in a project
  field-delete:  Delete a field in a project
  field-list:    List the fields in a project
  item-add:      Add a pull request or an issue to a project
  item-archive:  Archive an item in a project
  item-create:   Create a draft issue item in a project
  item-delete:   Delete an item from a project by ID
  item-edit:     Edit an item in a project
  item-list:     List the items in a project
  link:          Link a project to a repository or a team
  list:          List the projects for an owner
  mark-template: Mark a project as a template
  unlink:        Unlink a project from a repository or a team
  view:          View a project
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
$ gh project create --owner monalisa --title "Roadmap"
  $ gh project view 1 --owner cli --web
  $ gh project field-list 1 --owner cli
  $ gh project item-list 1 --owner cli
```

---

## <a id="cmd-project-close"></a>`gh project close`

Close a project

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh project close [<number>] [flags]
```

### Flags
```text
--format string     Output format: {json}
  -q, --jq expression     Filter JSON output using a jq expression
      --owner string      Login of the owner. Use "@me" for the current user.
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
      --undo              Reopen a closed project
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Close project "1" owned by monalisa
  $ gh project close 1 --owner monalisa
  
  # Reopen closed project "1" owned by github
  $ gh project close 1 --owner github --undo
```

---

## <a id="cmd-project-copy"></a>`gh project copy`

Copy a project

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh project copy [<number>] [flags]
```

### Flags
```text
--drafts                Include draft issues when copying
      --format string         Output format: {json}
  -q, --jq expression         Filter JSON output using a jq expression
      --source-owner string   Login of the source owner. Use "@me" for the current user.
      --target-owner string   Login of the target owner. Use "@me" for the current user.
  -t, --template string       Format JSON output using a Go template; see "gh help formatting"
      --title string          Title for the new project
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Copy project "1" owned by monalisa to github
  $ gh project copy 1 --source-owner monalisa --target-owner github --title "a new project"
```

---

## <a id="cmd-project-create"></a>`gh project create`

Create a project

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh project create [flags]
```

### Flags
```text
--format string     Output format: {json}
  -q, --jq expression     Filter JSON output using a jq expression
      --owner string      Login of the owner. Use "@me" for the current user.
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
      --title string      Title for the project
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Create a new project owned by login monalisa
  $ gh project create --owner monalisa --title "a new project"
```

---

## <a id="cmd-project-delete"></a>`gh project delete`

Delete a project

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh project delete [<number>] [flags]
```

### Flags
```text
--format string     Output format: {json}
  -q, --jq expression     Filter JSON output using a jq expression
      --owner string      Login of the owner. Use "@me" for the current user.
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Delete the current user's project "1"
  $ gh project delete 1 --owner "@me"
```

---

## <a id="cmd-project-edit"></a>`gh project edit`

Edit a project

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh project edit [<number>] [flags]
```

### Flags
```text
-d, --description string   New description of the project
      --format string        Output format: {json}
  -q, --jq expression        Filter JSON output using a jq expression
      --owner string         Login of the owner. Use "@me" for the current user.
      --readme string        New readme for the project
  -t, --template string      Format JSON output using a Go template; see "gh help formatting"
      --title string         New title for the project
      --visibility string    Change project visibility: {PUBLIC|PRIVATE}
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Edit the title of monalisa's project "1"
  $ gh project edit 1 --owner monalisa --title "New title"
```

---

## <a id="cmd-project-field-create"></a>`gh project field-create`

Create a field in a project

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh project field-create [<number>] [flags]
```

### Flags
```text
--data-type string                DataType of the new field.: {TEXT|SINGLE_SELECT|DATE|NUMBER}
      --format string                   Output format: {json}
  -q, --jq expression                   Filter JSON output using a jq expression
      --name string                     Name of the new field
      --owner string                    Login of the owner. Use "@me" for the current user.
      --single-select-options strings   Options for SINGLE_SELECT data type
  -t, --template string                 Format JSON output using a Go template; see "gh help formatting"
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Create a field in the current user's project "1"
  $ gh project field-create 1 --owner "@me" --name "new field" --data-type "text"
  
  # Create a field with three options to select from for owner monalisa
  $ gh project field-create 1 --owner monalisa --name "new field" --data-type "SINGLE_SELECT" --single-select-options "one,two,three"
```

---

## <a id="cmd-project-field-delete"></a>`gh project field-delete`

Delete a field in a project

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh project field-delete [flags]
```

### Flags
```text
--format string     Output format: {json}
      --id string         ID of the field to delete
  -q, --jq expression     Filter JSON output using a jq expression
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-project-field-list"></a>`gh project field-list`

List the fields in a project

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh project field-list [<number>] [flags]
```

### Flags
```text
--format string     Output format: {json}
  -q, --jq expression     Filter JSON output using a jq expression
  -L, --limit int         Maximum number of fields to fetch (default 30)
      --owner string      Login of the owner. Use "@me" for the current user.
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# List fields in the current user's project "1"
  $ gh project field-list 1 --owner "@me"
```

---

## <a id="cmd-project-item-add"></a>`gh project item-add`

Add a pull request or an issue to a project

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh project item-add [<number>] [flags]
```

### Flags
```text
--format string     Output format: {json}
  -q, --jq expression     Filter JSON output using a jq expression
      --owner string      Login of the owner. Use "@me" for the current user.
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
      --url string        URL of the issue or pull request to add to the project
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Add an item to monalisa's project "1"
  $ gh project item-add 1 --owner monalisa --url https://github.com/monalisa/myproject/issues/23
```

---

## <a id="cmd-project-item-archive"></a>`gh project item-archive`

Archive an item in a project

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh project item-archive [<number>] [flags]
```

### Flags
```text
--format string     Output format: {json}
      --id string         ID of the item to archive
  -q, --jq expression     Filter JSON output using a jq expression
      --owner string      Login of the owner. Use "@me" for the current user.
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
      --undo              Unarchive an item
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Archive an item in the current user's project "1"
  $ gh project item-archive 1 --owner "@me" --id <item-ID>
```

---

## <a id="cmd-project-item-create"></a>`gh project item-create`

Create a draft issue item in a project

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh project item-create [<number>] [flags]
```

### Flags
```text
--body string       Body for the draft issue
      --format string     Output format: {json}
  -q, --jq expression     Filter JSON output using a jq expression
      --owner string      Login of the owner. Use "@me" for the current user.
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
      --title string      Title for the draft issue
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Create a draft issue in the current user's project "1"
  $ gh project item-create 1 --owner "@me" --title "new item" --body "new item body"
```

---

## <a id="cmd-project-item-delete"></a>`gh project item-delete`

Delete an item from a project by ID

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh project item-delete [<number>] [flags]
```

### Flags
```text
--format string     Output format: {json}
      --id string         ID of the item to delete
  -q, --jq expression     Filter JSON output using a jq expression
      --owner string      Login of the owner. Use "@me" for the current user.
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Delete an item in the current user's project "1"
  $ gh project item-delete 1 --owner "@me" --id <item-id>
```

---

## <a id="cmd-project-item-edit"></a>`gh project item-edit`

Edit a draft issue or a project item.

The usual way to select the item and field is by name: pass the project
`number` plus `--owner`, point at the item with its issue or pull
request `--url`, and name the field with `--field`. For single-select
fields, `--value` is the option name.

For scripts and machine use, you can also pass GraphQL node IDs directly with
`--id`, `--field-id` and `--project-id` (and, for single-select
fields, `--single-select-option-id`).

Note that `--url` is the issue or pull request URL, not a project URL, so its
owner may differ from the project's; `--owner` selects the project.

For non-draft issues, only a single field value can be updated per invocation.

Remove a project item field value with `--clear`.

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh project item-edit [<number>] [flags]
```

### Flags
```text
--body string                      Body of the draft issue item
      --clear                            Remove field value
      --date string                      Date value for the field (YYYY-MM-DD)
      --field string                     Name of the field to update
      --field-id string                  ID of the field to update
      --format string                    Output format: {json}
      --id string                        ID of the item to edit
      --iteration-id string              ID of the iteration value to set on the field
  -q, --jq expression                    Filter JSON output using a jq expression
      --number float                     Number value for the field
      --owner string                     Login of the owner. Use "@me" for the current user.
      --project-id string                ID of the project to which the field belongs to
      --single-select-option-id string   ID of the single select option value to set on the field
  -t, --template string                  Format JSON output using a Go template; see "gh help formatting"
      --text string                      Text value for the field
      --title string                     Title of the draft issue item
      --url string                       URL of the issue or pull request whose project item to edit
      --value --field                    Value to set on the field named by --field
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Set the "Status" field to "In Progress" for an issue on monalisa's project 1
  $ gh project item-edit 1 --owner monalisa --url https://github.com/monalisa/myproject/issues/23 --field "Status" --value "In Progress"
  
  # Edit an item's text field value by node ID (machine / scripted use)
  $ gh project item-edit --id <item-id> --field-id <field-id> --project-id <project-id> --text "new text"
  
  # Clear an item's field value by node ID
  $ gh project item-edit --id <item-id> --field-id <field-id> --project-id <project-id> --clear
```

---

## <a id="cmd-project-item-list"></a>`gh project item-list`

List the items in a project.

If supported by the API host, the --query option can be used to perform
advanced search. For the full syntax, see:
https://docs.github.com/en/issues/planning-and-tracking-with-projects/customizing-views-in-your-project/filtering-projects

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh project item-list [<number>] [flags]
```

### Flags
```text
--field stringArray      Name of a field to show as an extra column
      --field-id stringArray   ID of a field to show as an extra column
      --format string          Output format: {json}
  -q, --jq expression          Filter JSON output using a jq expression
  -L, --limit int              Maximum number of items to fetch (default 30)
      --owner string           Login of the owner. Use "@me" for the current user
      --query string           Filter items using the Projects filter syntax, e.g. "assignee:octocat -status:Done"
  -t, --template string        Format JSON output using a Go template; see "gh help formatting"
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# List the items in the current users's project "1"
  $ gh project item-list 1 --owner "@me"
  
  # List items assigned to a specific user
  $ gh project item-list 1 --owner "@me" --query "assignee:monalisa"
  
  # List open issues assigned to yourself
  $ gh project item-list 1 --owner "@me" --query "assignee:@me is:issue is:open"
  
  # List items with the "bug" label that are not done
  $ gh project item-list 1 --owner "@me" --query "label:bug -status:Done"
  
  # Show the "Status" and "Priority" field values as extra columns
  $ gh project item-list 1 --owner "@me" --field "Status" --field "Priority"
```

---

## <a id="cmd-project-link"></a>`gh project link`

Link a project to a repository or a team

### Synopsis
```bash
gh project link [<number>] [flags]
```

### Flags
```text
--owner string   Login of the owner. Use "@me" for the current user.
  -R, --repo string    The repository to be linked to this project
  -T, --team string    The team to be linked to this project
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Link monalisa's project 1 to her repository "my_repo"
  $ gh project link 1 --owner monalisa --repo my_repo
  
  # Link monalisa's organization's project 1 to her team "my_team"
  $ gh project link 1 --owner my_organization --team my_team
  
  # Link monalisa's project 1 to the repository of current directory if neither --repo nor --team is specified
  $ gh project link 1
```

---

## <a id="cmd-project-list"></a>`gh project list`

List the projects for an owner

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh project list [flags]
```

### Aliases
`gh project ls`

### Flags
```text
--closed            Include closed projects
      --format string     Output format: {json}
  -q, --jq expression     Filter JSON output using a jq expression
  -L, --limit int         Maximum number of projects to fetch (default 30)
      --owner string      Login of the owner
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
  -w, --web               Open projects list in the browser
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# List the current user's projects
  $ gh project list
  
  # List the projects for org github including closed projects
  $ gh project list --owner github --closed
```

---

## <a id="cmd-project-mark-template"></a>`gh project mark-template`

Mark a project as a template

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh project mark-template [<number>] [flags]
```

### Flags
```text
--format string     Output format: {json}
  -q, --jq expression     Filter JSON output using a jq expression
      --owner string      Login of the org owner.
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
      --undo              Unmark the project as a template.
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Mark the github org's project "1" as a template
  $ gh project mark-template 1 --owner "github"
  
  # Unmark the github org's project "1" as a template
  $ gh project mark-template 1 --owner "github" --undo
```

---

## <a id="cmd-project-unlink"></a>`gh project unlink`

Unlink a project from a repository or a team

### Synopsis
```bash
gh project unlink [<number>] [flags]
```

### Flags
```text
--owner string   Login of the owner. Use "@me" for the current user.
  -R, --repo string    The repository to be unlinked from this project
  -T, --team string    The team to be unlinked from this project
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Unlink monalisa's project 1 from her repository "my_repo"
  $ gh project unlink 1 --owner monalisa --repo my_repo
  
  # Unlink monalisa's organization's project 1 from her team "my_team"
  $ gh project unlink 1 --owner my_organization --team my_team
  
  # Unlink monalisa's project 1 from the repository of current directory if neither --repo nor --team is specified
  $ gh project unlink 1
```

---

## <a id="cmd-project-view"></a>`gh project view`

View a project

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh project view [<number>] [flags]
```

### Flags
```text
--format string     Output format: {json}
  -q, --jq expression     Filter JSON output using a jq expression
      --owner string      Login of the owner. Use "@me" for the current user.
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
  -w, --web               Open a project in the browser
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# View the current user's project "1"
  $ gh project view 1
  
  # Open user monalisa's project "1" in the browser
  $ gh project view 1 --owner monalisa --web
```

---

## <a id="cmd-release"></a>`gh release`

Manage releases

### Synopsis
```bash
gh release <command> [flags]

GENERAL COMMANDS
  create:        Create a new release
  list:          List releases in a repository

TARGETED COMMANDS
  delete:        Delete a release
  delete-asset:  Delete an asset from a release
  download:      Download release assets
  edit:          Edit a release
  upload:        Upload assets to a release
  verify:        Verify the attestation for a release
  verify-asset:  Verify that a given asset originated from a release
  view:          View information about a release
```

### Flags
```text
-R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-release-create"></a>`gh release create`

Create a new GitHub Release for a repository.

A list of asset files may be given to upload to the new release. To define a
display label for an asset, append text starting with `#` after the file name.

If a matching git tag does not yet exist, one will automatically get created
from the latest state of the default branch.
Use `--target` to point to a different branch or commit for the automatic tag creation.
Use `--verify-tag` to abort the release if the tag doesn't already exist.
To fetch the new tag locally after the release, do `git fetch --tags origin`.

To create a release from an annotated git tag, first create one locally with
git, push the tag to GitHub, then run this command.
Use `--notes-from-tag` to get the release notes from the annotated git tag.
If the tag is not annotated, the commit message will be used instead.

Use `--generate-notes` to automatically generate notes using GitHub Release Notes API.
When using automatically generated release notes, a release title will also be automatically
generated unless a title was explicitly passed. Additional release notes can be prepended to
automatically generated notes by using the `--notes` flag.

By default, the release is created even if there are no new commits since the last release.
This may result in the same or duplicate release which may not be desirable in some cases.
Use `--fail-on-no-commits` to fail if no new commits are available. This flag has no
effect if there are no existing releases or this is the very first release.

## Immutable Releases

When release immutability is enabled for a repository, the following protections are enforced:
- Git tags associated with a release cannot be modified or deleted.
- Release assets cannot be modified or deleted.

When you attach assets, `gh release create` creates a draft release, uploads
each asset, and then publishes the release. These steps use separate API requests
and do not form a single atomic operation. If you specify `--draft`, the command
leaves the release unpublished.

When release immutability is enabled for the repository, its protections take effect
only when the release is published. While the release remains a draft, users and
workflows with the required permissions can modify it and its assets, including while
this command is running.

### Synopsis
```bash
gh release create [<tag>] [<filename>... | <pattern>...]
```

### Aliases
`gh release new`

### Flags
```text
--discussion-category string   Start a discussion in the specified category
  -d, --draft                        Save the release as a draft instead of publishing it
      --fail-on-no-commits           Fail if there are no commits since the last release (no impact on the first release)
      --generate-notes               Automatically generate title and notes for the release via GitHub Release Notes API
      --latest                       Mark this release as "Latest" (default [automatic based on date and version]). --latest=false to explicitly NOT set as latest
  -n, --notes string                 Release notes
  -F, --notes-file file              Read release notes from file (use "-" to read from standard input)
      --notes-from-tag               Fetch notes from the tag annotation or message of commit associated with tag
      --notes-start-tag string       Tag to use as the starting point for generating release notes
  -p, --prerelease                   Mark the release as a prerelease
      --target branch                Target branch or full commit SHA (default [main branch])
  -t, --title string                 Release title
      --verify-tag                   Abort in case the git tag doesn't already exist in the remote repository
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Examples
```bash
# Interactively create a release
  $ gh release create
  
  # Interactively create a release from specific tag
  $ gh release create v1.2.3
  
  # Non-interactively create a release
  $ gh release create v1.2.3 --notes "bugfix release"
  
  # Use automatically generated via GitHub Release Notes API release notes
  $ gh release create v1.2.3 --generate-notes
  
  # Use release notes from a file
  $ gh release create v1.2.3 -F release-notes.md
  
  # Use tag annotation or associated commit message as notes
  $ gh release create v1.2.3 --notes-from-tag
  
  # Don't mark the release as latest
  $ gh release create v1.2.3 --latest=false
  
  # Upload all tarballs in a directory as release assets
  $ gh release create v1.2.3 ./dist/*.tgz
  
  # Upload a release asset with a display label
  $ gh release create v1.2.3 '/path/to/asset.zip#My display label'
  
  # Create a release and start a discussion
  $ gh release create v1.2.3 --discussion-category "General"
  
  # Create a release only if there are new commits available since the last release
  $ gh release create v1.2.3 --fail-on-no-commits
```

---

## <a id="cmd-release-delete"></a>`gh release delete`

Delete a release

### Synopsis
```bash
gh release delete <tag> [flags]
```

### Flags
```text
--cleanup-tag   Delete the specified tag in addition to its release
  -y, --yes           Skip the confirmation prompt
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

---

## <a id="cmd-release-delete-asset"></a>`gh release delete-asset`

Delete an asset from a release

### Synopsis
```bash
gh release delete-asset <tag> <asset-name> [flags]
```

### Flags
```text
-y, --yes   Skip the confirmation prompt
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

---

## <a id="cmd-release-download"></a>`gh release download`

Download assets from a GitHub release.

Without an explicit tag name argument, assets are downloaded from the
latest release in the project. In this case, `--pattern` or `--archive`
is required.

### Synopsis
```bash
gh release download [<tag>] [flags]
```

### Flags
```text
--allow-escape-sequences   Allow printing terminal escape sequences when writing an asset to standard output
  -A, --archive format           Download the source code archive in the specified format (zip or tar.gz)
      --clobber                  Overwrite existing files of the same name
  -D, --dir directory            The directory to download files into (default ".")
  -O, --output file              The file to write a single asset to (use "-" to write to standard output)
  -p, --pattern stringArray      Download only assets that match a glob pattern
      --skip-existing            Skip downloading when files of the same name exist
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Examples
```bash
# Download all assets from a specific release
  $ gh release download v1.2.3
  
  # Download only Debian packages for the latest release
  $ gh release download --pattern '*.deb'
  
  # Specify multiple file patterns
  $ gh release download -p '*.deb' -p '*.rpm'
  
  # Download the archive of the source code for a release
  $ gh release download v1.2.3 --archive=zip
```

---

## <a id="cmd-release-edit"></a>`gh release edit`

Edit a release

### Synopsis
```bash
gh release edit <tag>
```

### Flags
```text
--discussion-category string   Start a discussion in the specified category when publishing a draft
      --draft                        Save the release as a draft instead of publishing it
      --latest                       Explicitly mark the release as "Latest"
  -n, --notes string                 Release notes
  -F, --notes-file file              Read release notes from file (use "-" to read from standard input)
      --prerelease                   Mark the release as a prerelease
      --tag string                   The name of the tag
      --target branch                Target branch or full commit SHA (default [main branch])
  -t, --title string                 Release title
      --verify-tag                   Abort in case the git tag doesn't already exist in the remote repository
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Examples
```bash
# Publish a release that was previously a draft
  $ gh release edit v1.0 --draft=false
  
  # Update the release notes from the content of a file
  $ gh release edit v1.0 --notes-file /path/to/release_notes.md
```

---

## <a id="cmd-release-list"></a>`gh release list`

List releases in a repository

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh release list [flags]
```

### Aliases
`gh release ls`

### Flags
```text
--exclude-drafts         Exclude draft releases
      --exclude-pre-releases   Exclude pre-releases
  -q, --jq expression          Filter JSON output using a jq expression
      --json fields            Output JSON with the specified fields
  -L, --limit int              Maximum number of items to fetch (default 30)
  -O, --order string           Order of releases returned: {asc|desc} (default "desc")
  -t, --template string        Format JSON output using a Go template; see "gh help formatting"
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format

JSON FIELDS
  createdAt, isDraft, isImmutable, isLatest, isPrerelease, name, publishedAt,
  tagName
```

---

## <a id="cmd-release-upload"></a>`gh release upload`

Upload asset files to a GitHub Release.

To define a display label for an asset, append text starting with `#` after the
file name.

When using `--clobber`, existing assets are deleted before new assets are uploaded.
If the upload fails, the original assets will be lost.

### Synopsis
```bash
gh release upload <tag> <files>... [flags]
```

### Flags
```text
--clobber   Delete and re-upload existing assets of the same name
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

---

## <a id="cmd-release-verify"></a>`gh release verify`

Verify that a GitHub Release is accompanied by a valid cryptographically signed attestation.

An attestation is a claim made by GitHub regarding a release and its assets.

This command checks that the specified release (or the latest release, if no tag is given) has a valid attestation. 
It fetches the attestation for the release and prints metadata about all assets referenced in the attestation, including their digests.

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh release verify [<tag>] [flags]
```

### Flags
```text
--format string     Output format: {json}
  -q, --jq expression     Filter JSON output using a jq expression
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Examples
```bash
# Verify the latest release
  gh release verify
  
  # Verify a specific release by tag
  gh release verify v1.2.3
  
  # Verify a specific release by tag and output the attestation in JSON format
  gh release verify v1.2.3 --format json
```

---

## <a id="cmd-release-verify-asset"></a>`gh release verify-asset`

Verify that a given asset file originated from a specific GitHub Release using cryptographically signed attestations.

An attestation is a claim made by GitHub regarding a release and its assets.

		This command checks that the asset you provide matches a valid attestation for the specified release (or the latest release, if no tag is given).
It ensures the asset's integrity by validating that the asset's digest matches the subject in the attestation and that the attestation is associated with the release.

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh release verify-asset [<tag>] <file-path> [flags]
```

### Flags
```text
--format string     Output format: {json}
  -q, --jq expression     Filter JSON output using a jq expression
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Examples
```bash
# Verify an asset from the latest release
  $ gh release verify-asset ./dist/my-asset.zip
  
  # Verify an asset from a specific release tag
  $ gh release verify-asset v1.2.3 ./dist/my-asset.zip
  
  # Verify an asset from a specific release tag and output the attestation in JSON format
  $ gh release verify-asset v1.2.3 ./dist/my-asset.zip --format json
```

---

## <a id="cmd-release-view"></a>`gh release view`

View information about a GitHub Release.

Without an explicit tag name argument, the latest release in the project
is shown.

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh release view [<tag>] [flags]
```

### Flags
```text
-q, --jq expression     Filter JSON output using a jq expression
      --json fields       Output JSON with the specified fields
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
  -w, --web               Open the release in the browser
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format

JSON FIELDS
  apiUrl, assets, author, body, createdAt, databaseId, id, isDraft, isImmutable,
  isPrerelease, name, publishedAt, tagName, tarballUrl, targetCommitish,
  uploadUrl, url, zipballUrl
```

---

## <a id="cmd-repo"></a>`gh repo`

Work with GitHub repositories.

### Synopsis
```bash
gh repo <command> [flags]

GENERAL COMMANDS
  create:        Create a new repository
  list:          List repositories owned by user or organization

TARGETED COMMANDS
  archive:       Archive a repository
  autolink:      Manage autolink references
  clone:         Clone a repository locally
  delete:        Delete a repository
  deploy-key:    Manage deploy keys in a repository
  edit:          Edit repository settings
  fork:          Create a fork of a repository
  gitignore:     List and view available repository gitignore templates
  license:       Explore repository licenses
  read-dir:      List a directory in a repository (preview)
  read-file:     Read a file from a repository (preview)
  rename:        Rename a repository
  set-default:   Configure default repository for this directory
  sync:          Sync a repository
  unarchive:     Unarchive a repository
  view:          View a repository
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
$ gh repo create
  $ gh repo clone cli/cli
  $ gh repo view --web
```

---

## <a id="cmd-repo-archive"></a>`gh repo archive`

Archive a GitHub repository.

With no argument, archives the current repository.

### Synopsis
```bash
gh repo archive [<repository>] [flags]
```

### Flags
```text
-y, --yes   Skip the confirmation prompt
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-repo-autolink"></a>`gh repo autolink`

Autolinks link issues, pull requests, commit messages, and release descriptions to external third-party services.

Autolinks require `admin` role to view or manage.

For more information, see <https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/managing-repository-settings/configuring-autolinks-to-reference-external-resources>

### Synopsis
```bash
gh repo autolink <command> [flags]

AVAILABLE COMMANDS
  create:        Create a new autolink reference
  delete:        Delete an autolink reference
  list:          List autolink references for a GitHub repository
  view:          View an autolink reference
```

### Flags
```text
-R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-repo-autolink-create"></a>`gh repo autolink create`

Create a new autolink reference for a repository.

The `keyPrefix` argument specifies the prefix that will generate a link when it is appended by certain characters.

The `urlTemplate` argument specifies the target URL that will be generated when the keyPrefix is found, which
must contain `<num>` variable for the reference number.

By default, autolinks are alphanumeric with `--numeric` flag used to create a numeric autolink.

The `<num>` variable behavior differs depending on whether the autolink is alphanumeric or numeric:

- alphanumeric: matches `A-Z` (case insensitive), `0-9`, and `-`
- numeric: matches `0-9`

If the template contains multiple instances of `<num>`, only the first will be replaced.

### Synopsis
```bash
gh repo autolink create <keyPrefix> <urlTemplate> [flags]
```

### Aliases
`gh repo autolink new`

### Flags
```text
-n, --numeric   Mark autolink as numeric
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Examples
```bash
# Create an alphanumeric autolink to example.com for the key prefix "TICKET-".
  # Generates https://example.com/TICKET?query=123abc from "TICKET-123abc".
  $ gh repo autolink create TICKET- "https://example.com/TICKET?query=<num>"
  
  # Create a numeric autolink to example.com for the key prefix "STORY-".
  # Generates https://example.com/STORY?id=123 from "STORY-123".
  $ gh repo autolink create STORY- "https://example.com/STORY?id=<num>" --numeric
```

---

## <a id="cmd-repo-autolink-delete"></a>`gh repo autolink delete`

Delete an autolink reference for a repository.

### Synopsis
```bash
gh repo autolink delete <id> [flags]
```

### Flags
```text
--yes   Confirm deletion without prompting
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

---

## <a id="cmd-repo-autolink-list"></a>`gh repo autolink list`

Gets all autolink references that are configured for a repository.

Information about autolinks is only available to repository administrators.

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh repo autolink list [flags]
```

### Aliases
`gh repo autolink ls`

### Flags
```text
-q, --jq expression     Filter JSON output using a jq expression
      --json fields       Output JSON with the specified fields
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
  -w, --web               List autolink references in the web browser
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format

JSON FIELDS
  id, isAlphanumeric, keyPrefix, urlTemplate
```

---

## <a id="cmd-repo-autolink-view"></a>`gh repo autolink view`

View an autolink reference for a repository.

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh repo autolink view <id> [flags]
```

### Flags
```text
-q, --jq expression     Filter JSON output using a jq expression
      --json fields       Output JSON with the specified fields
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format

JSON FIELDS
  id, isAlphanumeric, keyPrefix, urlTemplate
```

---

## <a id="cmd-repo-clone"></a>`gh repo clone`

Clone a GitHub repository locally. Pass additional `git clone` flags by listing
them after `--`.

If the `OWNER/` portion of the `OWNER/REPO` repository argument is omitted, it
defaults to the name of the authenticating user.

When a protocol scheme is not provided in the repository argument, the `git_protocol` will be
chosen from your configuration, which can be checked via `gh config get git_protocol`. If the protocol
scheme is provided, the repository will be cloned using the specified protocol.

If the repository is a fork, its parent repository will be added as an additional
git remote called `upstream`. The remote name can be configured using `--upstream-remote-name`.
The `--upstream-remote-name` option supports an `@owner` value which will name
the remote after the owner of the parent repository.

If the repository is a fork, its parent repository will be set as the default remote repository.
To skip this behavior, use `--no-upstream`.

### Synopsis
```bash
gh repo clone <repository> [<directory>] [-- <gitflags>...]
```

### Flags
```text
--no-upstream                   Do not add an upstream remote when cloning a fork
  -u, --upstream-remote-name string   Upstream remote name when cloning a fork (default "upstream")
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Clone a repository from a specific org
  $ gh repo clone cli/cli
  
  # Clone a repository from your own account
  $ gh repo clone myrepo
  
  # Clone a repo, overriding git protocol configuration
  $ gh repo clone https://github.com/cli/cli
  $ gh repo clone git@github.com:cli/cli.git
  
  # Clone a repository to a custom directory
  $ gh repo clone cli/cli workspace/cli
  
  # Clone a repository with additional git clone flags
  $ gh repo clone cli/cli -- --depth=1
  
  # Clone a fork without adding an upstream remote
  $ gh repo clone myfork --no-upstream
```

---

## <a id="cmd-repo-create"></a>`gh repo create`

Create a new GitHub repository.

To create a repository interactively, use `gh repo create` with no arguments.

To create a remote repository non-interactively, supply the repository name and one of `--public`, `--private`, or `--internal`.
Pass `--clone` to clone the new repository locally.

If the `OWNER/` portion of the `OWNER/REPO` name argument is omitted, it
defaults to the name of the authenticating user.

To create a remote repository from an existing local repository, specify the source directory with `--source`.
By default, the remote repository name will be the name of the source directory.

Pass `--push` to push any local commits to the new repository. If the repo is bare, this will mirror all refs.

For language or platform .gitignore templates to use with `--gitignore`, <https://github.com/github/gitignore>.

For license keywords to use with `--license`, run `gh repo license list` or visit <https://choosealicense.com>.

The repo is created with the configured repository default branch, see <https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-personal-account-on-github/managing-user-account-settings/managing-the-default-branch-name-for-your-repositories>.

### Synopsis
```bash
gh repo create [<name>] [flags]
```

### Aliases
`gh repo new`

### Flags
```text
--add-readme             Add a README file to the new repository
  -c, --clone                  Clone the new repository to the current directory
  -d, --description string     Description of the repository
      --disable-issues         Disable issues in the new repository
      --disable-wiki           Disable wiki in the new repository
  -g, --gitignore string       Specify a gitignore template for the repository
  -h, --homepage URL           Repository home page URL
      --include-all-branches   Include all branches from template repository
      --internal               Make the new repository internal
  -l, --license string         Specify an Open Source License for the repository
      --private                Make the new repository private
      --public                 Make the new repository public
      --push                   Push local commits to the new repository
  -r, --remote string          Specify remote name for the new repository
  -s, --source string          Specify path to local repository to use as source
  -t, --team name              The name of the organization team to be granted access
  -p, --template repository    Make the new repository based on a template repository
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Create a repository interactively
  $ gh repo create
  
  # Create a new remote repository and clone it locally
  $ gh repo create my-project --public --clone
  
  # Create a new remote repository in a different organization
  $ gh repo create my-org/my-project --public
  
  # Create a remote repository from the current directory
  $ gh repo create my-project --private --source=. --remote=upstream
```

---

## <a id="cmd-repo-delete"></a>`gh repo delete`

Delete a GitHub repository.

With no argument, deletes the current repository. Otherwise, deletes the specified repository.

For safety, when no repository argument is provided, the `--yes` flag is ignored 
and you will be prompted for confirmation. To delete the current repository non-interactively, 
specify it explicitly (e.g., `gh repo delete owner/repo --yes`).

Deletion requires authorization with the `delete_repo` scope.
To authorize, run `gh auth refresh -s delete_repo`

### Synopsis
```bash
gh repo delete [<repository>] [flags]
```

### Flags
```text
--yes   Confirm deletion without prompting
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-repo-deploy-key"></a>`gh repo deploy-key`

Manage deploy keys in a repository

### Synopsis
```bash
gh repo deploy-key <command> [flags]

AVAILABLE COMMANDS
  add:           Add a deploy key to a GitHub repository
  delete:        Delete a deploy key from a GitHub repository
  list:          List deploy keys in a GitHub repository
```

### Flags
```text
-R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-repo-deploy-key-add"></a>`gh repo deploy-key add`

Add a deploy key to a GitHub repository.

Note that any key added by gh will be associated with the current authentication token.
If you de-authorize the GitHub CLI app or authentication token from your account, any
deploy keys added by GitHub CLI will be removed as well.

### Synopsis
```bash
gh repo deploy-key add <key-file> [flags]
```

### Flags
```text
-w, --allow-write    Allow write access for the key
  -t, --title string   Title of the new key
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Examples
```bash
# Generate a passwordless SSH key and add it as a deploy key to a repository
  $ ssh-keygen -t ed25519 -C "my description" -N "" -f ~/.ssh/gh-test
  $ gh repo deploy-key add ~/.ssh/gh-test.pub
```

---

## <a id="cmd-repo-deploy-key-delete"></a>`gh repo deploy-key delete`

Delete a deploy key from a GitHub repository

### Synopsis
```bash
gh repo deploy-key delete <key-id> [flags]
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

---

## <a id="cmd-repo-deploy-key-list"></a>`gh repo deploy-key list`

List deploy keys in a GitHub repository

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh repo deploy-key list [flags]
```

### Aliases
`gh repo deploy-key ls`

### Flags
```text
-q, --jq expression     Filter JSON output using a jq expression
      --json fields       Output JSON with the specified fields
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format

JSON FIELDS
  createdAt, id, key, readOnly, title
```

---

## <a id="cmd-repo-edit"></a>`gh repo edit`

Edit repository settings.

To toggle a setting off, use the `--<flag>=false` syntax.

Changing repository visibility can have unexpected consequences including but not limited to:

- Losing stars and watchers, affecting repository ranking
- Detaching public forks from the network
- Disabling push rulesets
- Allowing access to GitHub Actions history and logs

When the `--visibility` flag is used, `--accept-visibility-change-consequences` flag is required.

For information on all the potential consequences, see <https://gh.io/setting-repository-visibility>.

When the `--enable-squash-merge` flag is used, `--squash-merge-commit-message`
can be used to change the default squash merge commit message behavior:

- `default`: uses commit title and message for 1 commit, or pull request title and list of commits for 2 or more
- `pr-title`: uses pull request title
- `pr-title-commits`: uses pull request title and list of commits
- `pr-title-description`: uses pull request title and description

### Synopsis
```bash
gh repo edit [<repository>] [flags]
```

### Flags
```text
--accept-visibility-change-consequences    Accept the consequences of changing the repository visibility
      --add-topic strings                        Add repository topic
      --allow-forking                            Allow forking of an organization repository
      --allow-update-branch                      Allow a pull request head branch that is behind its base branch to be updated
      --default-branch name                      Set the default branch name for the repository
      --delete-branch-on-merge                   Delete head branch when pull requests are merged
  -d, --description string                       Description of the repository
      --enable-advanced-security                 Enable advanced security in the repository
      --enable-auto-merge                        Enable auto-merge functionality
      --enable-discussions                       Enable discussions in the repository
      --enable-issues                            Enable issues in the repository
      --enable-merge-commit                      Enable merging pull requests via merge commit
      --enable-projects                          Enable projects in the repository
      --enable-rebase-merge                      Enable merging pull requests via rebase
      --enable-secret-scanning                   Enable secret scanning in the repository
      --enable-secret-scanning-push-protection   Enable secret scanning push protection in the repository. Secret scanning must be enabled first
      --enable-squash-merge                      Enable merging pull requests via squashed commit
      --enable-wiki                              Enable wiki in the repository
  -h, --homepage URL                             Repository home page URL
      --remove-topic strings                     Remove repository topic
      --squash-merge-commit-message string       The default value for a squash merge commit message: {default|pr-title|pr-title-commits|pr-title-description}
      --template                                 Make the repository available as a template repository
      --visibility string                        Change the visibility of the repository to {public,private,internal}
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Enable issues and wiki
  $ gh repo edit --enable-issues --enable-wiki
  
  # Disable projects
  $ gh repo edit --enable-projects=false
```

---

## <a id="cmd-repo-fork"></a>`gh repo fork`

Create a fork of a repository.

With no argument, creates a fork of the current repository. Otherwise, forks
the specified repository.

By default, the new fork is set to be your `origin` remote and any existing
origin remote is renamed to `upstream`. To alter this behavior, you can set
a name for the new fork's remote with `--remote-name`.

The `upstream` remote will be set as the default remote repository.

Additional `git clone` flags can be passed after `--`.

### Synopsis
```bash
gh repo fork [<repository>] [-- <gitflags>...] [flags]
```

### Flags
```text
--clone                 Clone the fork
  --default-branch-only   Only include the default branch in the fork
  --fork-name string      Rename the forked repository
  --org string            Create the fork in an organization
  --remote                Add a git remote for the fork
  --remote-name string    Specify the name for the new remote (default "origin")
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Fork a repository
  $ gh repo fork owner/repo
  
  # Fork a repository and clone it locally
  $ gh repo fork owner/repo --clone
  
  # Fork a repository without cloning it, skip the prompt
  $ gh repo fork owner/repo --clone=false
```

---

## <a id="cmd-repo-gitignore"></a>`gh repo gitignore`

List and view available repository gitignore templates

### Synopsis
```bash
gh repo gitignore <command> [flags]

AVAILABLE COMMANDS
  list:          List available repository gitignore templates
  view:          View an available repository gitignore template
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-repo-gitignore-list"></a>`gh repo gitignore list`

List available repository gitignore templates

### Synopsis
```bash
gh repo gitignore list [flags]
```

### Aliases
`gh repo gitignore ls`

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-repo-gitignore-view"></a>`gh repo gitignore view`

View an available repository `.gitignore` template.

`<template>` is a case-sensitive `.gitignore` template name.

For a list of available templates, run `gh repo gitignore list`.

### Synopsis
```bash
gh repo gitignore view <template> [flags]
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# View the Go gitignore template
  $ gh repo gitignore view Go
  
  # View the Python gitignore template
  $ gh repo gitignore view Python
  
  # Create a new .gitignore file using the Go template
  $ gh repo gitignore view Go > .gitignore
  
  # Create a new .gitignore file using the Python template
  $ gh repo gitignore view Python > .gitignore
```

---

## <a id="cmd-repo-license"></a>`gh repo license`

Explore repository licenses

### Synopsis
```bash
gh repo license <command> [flags]

AVAILABLE COMMANDS
  list:          List common repository licenses
  view:          View a specific repository license
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-repo-license-list"></a>`gh repo license list`

List common repository licenses.

For even more licenses, visit <https://choosealicense.com/appendix>

### Synopsis
```bash
gh repo license list [flags]
```

### Aliases
`gh repo license ls`

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-repo-license-view"></a>`gh repo license view`

View a specific repository license by license key or SPDX ID.

Run `gh repo license list` to see available commonly used licenses. For even more licenses, visit <https://choosealicense.com/appendix>.

### Synopsis
```bash
gh repo license view {<license-key> | <spdx-id>} [flags]
```

### Flags
```text
-w, --web   Open https://choosealicense.com/ in the browser
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
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

---

## <a id="cmd-repo-list"></a>`gh repo list`

List repositories owned by a user or organization.

Note that the list will only include repositories owned by the provided argument,
and the `--fork` or `--source` flags will not traverse ownership boundaries. For example,
when listing the forks in an organization, the output would not include those owned by individual users.

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh repo list [<owner>] [flags]
```

### Aliases
`gh repo ls`

### Flags
```text
--archived            Show only archived repositories
      --fork                Show only forks
  -q, --jq expression       Filter JSON output using a jq expression
      --json fields         Output JSON with the specified fields
  -l, --language string     Filter by primary coding language
  -L, --limit int           Maximum number of repositories to list (default 30)
      --no-archived         Omit archived repositories
      --source              Show only non-forks
  -t, --template string     Format JSON output using a Go template; see "gh help formatting"
      --topic strings       Filter by topic
      --visibility string   Filter by repository visibility: {public|private|internal}
```

### Inherited Flags
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

---

## <a id="cmd-repo-read-dir"></a>`gh repo read-dir`

List the contents of a directory in a GitHub repository without cloning it.

This command is in preview and subject to change without notice.

By default, the directory is listed from the default branch. Use the `--ref` flag to
list from a specific branch, tag, or commit. When no path is given, the repository root
is listed.

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh repo read-dir [<path>] [flags]
```

### Flags
```text
-q, --jq expression            Filter JSON output using a jq expression
      --json fields              Output JSON with the specified fields
      --ref string               The branch, tag, or commit to list from
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
  -t, --template string          Format JSON output using a Go template; see "gh help formatting"
```

### Inherited Flags
```text
--help   Show help for command

JSON FIELDS
  gitSHA, gitType, mode, modeOctal, name, nameRaw, path, pathRaw, size, submodule,
  type
```

### Examples
```bash
# List the root of the default branch
  $ gh repo read-dir --repo cli/cli
  
  # List a subdirectory
  $ gh repo read-dir docs --repo cli/cli
  
  # List a directory at a specific ref
  $ gh repo read-dir docs --repo cli/cli --ref v2.50.0
  
  # Print selected fields as JSON
  $ gh repo read-dir docs --repo cli/cli --json name,path,type,size
```

---

## <a id="cmd-repo-read-file"></a>`gh repo read-file`

Read the contents of a file in a GitHub repository without cloning it.

This command is in preview and subject to change without notice.

By default, the file is read from the default branch. Use the `--ref` flag to
read from a specific branch, tag, or commit.

When run in TTY mode, the content is shown through your pager. When stdout is piped or
redirected, the raw content is written directly. To save the file to disk instead, use
the `--output` flag.

By default, the command refuses to output a file that contains terminal escape sequences,
since they could manipulate your terminal. Pass `--allow-escape-sequences` to read the file anyway.
This check applies only to terminal and piped output; writing to disk with `--output` always
includes the raw bytes, as if `--allow-escape-sequences` were given.

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh repo read-file <path> [flags]
```

### Flags
```text
--allow-escape-sequences   Allow printing terminal escape sequences
      --clobber                  Overwrite the output path if it already exists
  -q, --jq expression            Filter JSON output using a jq expression
      --json fields              Output JSON with the specified fields
  -o, --output path              Write the file to a path instead of stdout
      --ref string               The branch, tag, or commit to read from
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
  -t, --template string          Format JSON output using a Go template; see "gh help formatting"
```

### Inherited Flags
```text
--help   Show help for command

JSON FIELDS
  content, downloadUrl, encoding, gitSHA, gitUrl, htmlUrl, name, path, size, type,
  url
```

### Examples
```bash
# Read a file from the default branch
  $ gh repo read-file README.md --repo cli/cli
  
  # Read a file at a specific ref
  $ gh repo read-file README.md --repo cli/cli --ref v2.50.0
  
  # Save a file to disk
  $ gh repo read-file README.md --repo cli/cli --output download/README.md
  
  # Print selected fields as JSON
  $ gh repo read-file README.md --repo cli/cli --json name,path,size,type
  
  # Read a file that contains terminal escape sequences
  $ gh repo read-file path/to/file --repo OWNER/REPO --allow-escape-sequences
```

---

## <a id="cmd-repo-rename"></a>`gh repo rename`

Rename a GitHub repository.

`<new-name>` is the desired repository name without the owner.

By default, the current repository is renamed. Otherwise, the repository specified
with `--repo` is renamed.

To transfer repository ownership to another user account or organization,
you must follow additional steps on `github.com`.

For more information on transferring repository ownership, see:
<https://docs.github.com/en/repositories/creating-and-managing-repositories/transferring-a-repository>

### Synopsis
```bash
gh repo rename [<new-name>] [flags]
```

### Flags
```text
-R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
  -y, --yes                      Skip the confirmation prompt
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Rename the current repository (foo/bar -> foo/baz)
  $ gh repo rename baz
  
  # Rename the specified repository (qux/quux -> qux/baz)
  $ gh repo rename -R qux/quux baz
```

---

## <a id="cmd-repo-set-default"></a>`gh repo set-default`

This command sets the default remote repository to use when querying the
GitHub API for the locally cloned repository.

gh uses the default repository for things like:

 - viewing and creating pull requests
 - viewing and creating issues
 - viewing and creating releases
 - working with GitHub Actions

### NOTE: gh does not use the default repository for managing repository and environment secrets.

### Synopsis
```bash
gh repo set-default [<repository>] [flags]
```

### Flags
```text
-u, --unset   Unset the current default repository
  -v, --view    View the current default repository
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Interactively select a default repository
  $ gh repo set-default
  
  # Set a repository explicitly
  $ gh repo set-default owner/repo
  
  # Set a repository using a git remote name
  $ gh repo set-default origin
  
  # View the current default repository
  $ gh repo set-default --view
  
  # Show more repository options in the interactive picker
  $ git remote add newrepo https://github.com/owner/repo
  $ gh repo set-default
```

---

## <a id="cmd-repo-sync"></a>`gh repo sync`

Sync destination repository from source repository. Syncing uses the default branch
of the source repository to update the matching branch on the destination
repository so they are equal. A fast forward update will be used except when the
`--force` flag is specified, then the two branches will
be synced using a hard reset.

Without an argument, the local repository is selected as the destination repository.

The source repository is the parent of the destination repository by default.
This can be overridden with the `--source` flag.

### Synopsis
```bash
gh repo sync [<destination-repository>] [flags]
```

### Flags
```text
-b, --branch string   Branch to sync (default [default branch])
      --force           Hard reset the branch of the destination repository to match the source repository
  -s, --source string   Source repository
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Sync local repository from remote parent
  $ gh repo sync
  
  # Sync local repository from remote parent on specific branch
  $ gh repo sync --branch v1
  
  # Sync remote fork from its parent
  $ gh repo sync owner/cli-fork
  
  # Sync remote repository from another remote repository
  $ gh repo sync owner/repo --source owner2/repo2
```

---

## <a id="cmd-repo-unarchive"></a>`gh repo unarchive`

Unarchive a GitHub repository.

With no argument, unarchives the current repository.

### Synopsis
```bash
gh repo unarchive [<repository>] [flags]
```

### Flags
```text
-y, --yes   Skip the confirmation prompt
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-repo-view"></a>`gh repo view`

Display the description and the README of a GitHub repository.

With no argument, the repository for the current directory is displayed.

With `--web`, open the repository in a web browser instead.

With `--branch`, view a specific branch of the repository.

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh repo view [<repository>] [flags]
```

### Flags
```text
-b, --branch string     View a specific branch of the repository
  -q, --jq expression     Filter JSON output using a jq expression
      --json fields       Output JSON with the specified fields
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
  -w, --web               Open a repository in the browser
```

### Inherited Flags
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

---

## <a id="cmd-ruleset"></a>`gh ruleset`

Repository rulesets are a way to define a set of rules that apply to a repository.
These commands allow you to view information about them.

### Synopsis
```bash
gh ruleset <command> [flags]
```

### Aliases
`gh rs`, ``, `AVAILABLE COMMANDS`, `  check:         View rules that would apply to a given branch`, `  list:          List rulesets for a repository or organization`, `  view:          View information about a ruleset`

### Flags
```text
-R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
$ gh ruleset list
  $ gh ruleset view --repo OWNER/REPO --web
  $ gh ruleset check branch-name
```

---

## <a id="cmd-ruleset-check"></a>`gh ruleset check`

View information about GitHub rules that apply to a given branch.

The provided branch name does not need to exist; rules will be displayed that would apply
to a branch with that name. All rules are returned regardless of where they are configured.

If no branch name is provided, then the current branch will be used.

The `--default` flag can be used to view rules that apply to the default branch of the
repository.

### Synopsis
```bash
gh ruleset check [<branch>] [flags]
```

### Flags
```text
--default   Check rules on default branch
  -w, --web       Open the branch rules page in a web browser
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Examples
```bash
# View all rules that apply to the current branch
  $ gh ruleset check
  
  # View all rules that apply to a branch named "my-branch" in a different repository
  $ gh ruleset check my-branch --repo owner/repo
  
  # View all rules that apply to the default branch in a different repository
  $ gh ruleset check --default --repo owner/repo
  
  # View a ruleset configured in a different repository or any of its parents
  $ gh ruleset view 23 --repo owner/repo
  
  # View an organization-level ruleset
  $ gh ruleset view 23 --org my-org
```

---

## <a id="cmd-ruleset-list"></a>`gh ruleset list`

List GitHub rulesets for a repository or organization.

If no options are provided, the current repository's rulesets are listed. You can query a different
repository's rulesets by using the `--repo` flag. You can also use the `--org` flag to list rulesets
configured for the provided organization.

Use the `--parents` flag to control whether rulesets configured at higher levels that also apply to the provided
repository or organization should be returned. The default is `true`.

Your access token must have the `admin:org` scope to use the `--org` flag, which can be granted by running `gh auth refresh -s admin:org`.

### Synopsis
```bash
gh ruleset list [flags]
```

### Aliases
`gh rs ls, gh ruleset ls`

### Flags
```text
-L, --limit int    Maximum number of rulesets to list (default 30)
  -o, --org string   List organization-wide rulesets for the provided organization
  -p, --parents      Whether to include rulesets configured at higher levels that also apply (default true)
  -w, --web          Open the list of rulesets in the web browser
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Examples
```bash
# List rulesets in the current repository
  $ gh ruleset list
  
  # List rulesets in a different repository, including those configured at higher levels
  $ gh ruleset list --repo owner/repo --parents
  
  # List rulesets in an organization
  $ gh ruleset list --org org-name
```

---

## <a id="cmd-ruleset-view"></a>`gh ruleset view`

View information about a GitHub ruleset.

If no ID is provided, an interactive prompt will be used to choose
the ruleset to view.

Use the `--parents` flag to control whether rulesets configured at higher
levels that also apply to the provided repository or organization should
be returned. The default is `true`.

### Synopsis
```bash
gh ruleset view [<ruleset-id>] [flags]
```

### Flags
```text
-o, --org string   Organization name if the provided ID is an organization-level ruleset
  -p, --parents      Whether to include rulesets configured at higher levels that also apply (default true)
  -w, --web          Open the ruleset in the browser
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Examples
```bash
# Interactively choose a ruleset to view from all rulesets that apply to the current repository
  $ gh ruleset view
  
  # Interactively choose a ruleset to view from only rulesets configured in the current repository
  $ gh ruleset view --parents=false
  
  # View a ruleset configured in the current repository or any of its parents
  $ gh ruleset view 43
  
  # View a ruleset configured in a different repository or any of its parents
  $ gh ruleset view 23 --repo owner/repo
  
  # View an organization-level ruleset
  $ gh ruleset view 23 --org my-org
```

---

## <a id="cmd-run"></a>`gh run`

List, view, and watch recent workflow runs from GitHub Actions.

### Synopsis
```bash
gh run <command> [flags]

AVAILABLE COMMANDS
  cancel:        Cancel a workflow run
  delete:        Delete a workflow run
  download:      Download artifacts generated by a workflow run
  list:          List recent workflow runs
  rerun:         Rerun a run
  view:          View a summary of a workflow run
  watch:         Watch a run until it completes, showing its progress
```

### Flags
```text
-R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-run-cancel"></a>`gh run cancel`

Cancel a workflow run

### Synopsis
```bash
gh run cancel [<run-id>] [flags]
```

### Flags
```text
--force   Force cancel a workflow run
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

---

## <a id="cmd-run-delete"></a>`gh run delete`

Delete a workflow run

### Synopsis
```bash
gh run delete [<run-id>] [flags]
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Examples
```bash
# Interactively select a run to delete
  $ gh run delete
  
  # Delete a specific run
  $ gh run delete 12345
```

---

## <a id="cmd-run-download"></a>`gh run download`

Download artifacts generated by a GitHub Actions workflow run.

The contents of each artifact will be extracted under separate directories based on
the artifact name. If only a single artifact is specified, it will be extracted into
the current directory.

By default, this command downloads the latest artifact created and uploaded through
GitHub Actions. Because workflows can delete or overwrite artifacts, `<run-id>`
must be used to select an artifact from a specific workflow run.

### Synopsis
```bash
gh run download [<run-id>] [flags]
```

### Flags
```text
-D, --dir string            The directory to download artifacts into (default ".")
  -n, --name stringArray      Download artifacts that match any of the given names
  -p, --pattern stringArray   Download artifacts that match a glob pattern
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Examples
```bash
# Download all artifacts generated by a workflow run
  $ gh run download <run-id>
  
  # Download a specific artifact within a run
  $ gh run download <run-id> -n <name>
  
  # Download specific artifacts across all runs in a repository
  $ gh run download -n <name1> -n <name2>
  
  # Select artifacts to download interactively
  $ gh run download
```

---

## <a id="cmd-run-list"></a>`gh run list`

List recent workflow runs.

Note that providing the `workflow_name` to the `-w` flag will not fetch disabled workflows.
Also pass the `-a` flag to fetch disabled workflow runs using the `workflow_name` and the `-w` flag.

Runs created by organization and enterprise ruleset workflows will not display a workflow name due to GitHub API limitations.

To see runs associated with a pull request, users should run `gh pr checks`.

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh run list [flags]
```

### Aliases
`gh run ls`

### Flags
```text
-a, --all               Include disabled workflows
  -b, --branch string     Filter runs by branch
  -c, --commit SHA        Filter runs by the SHA of the commit
      --created date      Filter runs by the date it was created
  -e, --event event       Filter runs by which event triggered the run
  -q, --jq expression     Filter JSON output using a jq expression
      --json fields       Output JSON with the specified fields
  -L, --limit int         Maximum number of runs to fetch (default 20)
  -s, --status string     Filter runs by status: {queued|completed|in_progress|requested|waiting|pending|action_required|cancelled|failure|neutral|skipped|stale|startup_failure|success|timed_out}
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
  -u, --user string       Filter runs by user who triggered the run
  -w, --workflow string   Filter runs by workflow
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format

JSON FIELDS
  attempt, conclusion, createdAt, databaseId, displayTitle, event, headBranch,
  headSha, name, number, startedAt, status, updatedAt, url, workflowDatabaseId,
  workflowName
```

---

## <a id="cmd-run-rerun"></a>`gh run rerun`

Rerun an entire run, only failed jobs, or a specific job from a run.

Note that due to historical reasons, the `--job` flag may not take what you expect.
Specifically, when navigating to a job in the browser, the URL looks like this:
`https://github.com/<owner>/<repo>/actions/runs/<run-id>/jobs/<number>`.

However, this `<number>` should not be used with the `--job` flag and will result in the
API returning `404 NOT FOUND`. Instead, you can get the correct job IDs using the following command:

	gh run view <run-id> --json jobs --jq '.jobs[] | {name, databaseId}'

You will need to use databaseId field for triggering job re-runs.

### Synopsis
```bash
gh run rerun [<run-id>] [flags]
```

### Flags
```text
-d, --debug        Rerun with debug logging
      --failed       Rerun only failed jobs, including dependencies
  -j, --job string   Rerun a specific job ID from a run, including dependencies
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

---

## <a id="cmd-run-view"></a>`gh run view`

View a summary of a workflow run.

Due to platform limitations, `gh` may not always be able to associate jobs with their
corresponding logs when using the primary method of fetching logs in zip format.

In such cases, `gh` will attempt to fetch logs for each job individually via the API.
This fallback is slower and more resource-intensive. If more than 25 job logs are missing,
the operation will fail with an error.

Additionally, due to similar platform constraints, some log lines may not be
associated with a specific step within a job. In these cases, the step name will
appear as `UNKNOWN STEP` in the log output.

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh run view [<run-id>] [flags]
```

### Flags
```text
-a, --attempt uint      The attempt number of the workflow run
      --exit-status       Exit with non-zero status if run failed
  -j, --job string        View a specific job ID from a run
  -q, --jq expression     Filter JSON output using a jq expression
      --json fields       Output JSON with the specified fields
      --log               View full log for either a run or specific job
      --log-failed        View the log for any failed steps in a run or specific job
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
  -v, --verbose           Show job steps
  -w, --web               Open run in the browser
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format

JSON FIELDS
  attempt, conclusion, createdAt, databaseId, displayTitle, event, headBranch,
  headSha, jobs, name, number, startedAt, status, updatedAt, url,
  workflowDatabaseId, workflowName
```

### Examples
```bash
# Interactively select a run to view, optionally selecting a single job
  $ gh run view
  
  # View a specific run
  $ gh run view 12345
  
  # View a specific run with specific attempt number
  $ gh run view 12345 --attempt 3
  
  # View a specific job within a run
  $ gh run view --job 456789
  
  # View the full log for a specific job
  $ gh run view --log --job 456789
  
  # Exit non-zero if a run failed
  $ gh run view 0451 --exit-status && echo "run pending or passed"
```

---

## <a id="cmd-run-watch"></a>`gh run watch`

Watch a run until it completes, showing its progress.

By default, all steps are displayed. The `--compact` option can be used to only
show the relevant/failed steps.

This command does not support authenticating via fine grained PATs
as it is not currently possible to create a PAT with the `checks:read` permission.

### Synopsis
```bash
gh run watch <run-id> [flags]
```

### Flags
```text
--compact        Show only relevant/failed steps
      --exit-status    Exit with non-zero status if run fails
  -i, --interval int   Refresh interval in seconds (default 3)
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Examples
```bash
# Watch a run until it's done
  $ gh run watch
  
  # Watch a run in compact mode
  $ gh run watch --compact
  
  # Run some other command when the run is finished
  $ gh run watch && notify-send 'run is done!'
```

---

## <a id="cmd-search"></a>`gh search`

Search across all of GitHub.

Excluding search results that match a qualifier

In a browser, the GitHub search syntax supports excluding results that match a search qualifier
by prefixing the qualifier with a hyphen. For example, to search for issues that
do not have the label "bug", you would use `-label:bug` as a search qualifier.

`gh` supports this syntax in `gh search` as well, but it requires extra
command line arguments to avoid the hyphen being interpreted as a command line flag because it begins with a hyphen.

On Unix-like systems, you can use the `--` argument to indicate that
the arguments that follow are not a flag, but rather a query string. For example:

$ gh search issues -- "my-search-query -label:bug"

On PowerShell, you must use both the `--%` argument and the `--` argument to
produce the same effect. For example:

$ gh --% search issues -- "my search query -label:bug"

See the following for more information:
- GitHub search syntax: <https://docs.github.com/en/search-github/getting-started-with-searching-on-github/understanding-the-search-syntax#exclude-results-that-match-a-qualifier>
- The PowerShell stop parse flag `--%`: <https://learn.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_parsing?view=powershell-7.5#the-stop-parsing-token>
- The Unix-like `--` argument: <https://www.gnu.org/software/bash/manual/bash.html#Shell-Builtin-Commands-1>

### Synopsis
```bash
gh search <command> [flags]

AVAILABLE COMMANDS
  code:          Search within code
  commits:       Search for commits
  issues:        Search for issues
  prs:           Search for pull requests
  repos:         Search for repositories
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-search-code"></a>`gh search code`

Search within code in GitHub repositories.

The search syntax is documented at:
<https://docs.github.com/search-github/searching-on-github/searching-code>

Note that these search results are powered by what is now a legacy GitHub code search engine.
The results might not match what is seen on `github.com`, and new features like regex search
are not yet available via the GitHub API.

For more information on handling search queries containing a hyphen, run `gh search --help`.

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh search code <query> [flags]
```

### Flags
```text
--extension string   Filter on file extension
      --filename string    Filter on filename
  -q, --jq expression      Filter JSON output using a jq expression
      --json fields        Output JSON with the specified fields
      --language string    Filter results by language
  -L, --limit int          Maximum number of code results to fetch (default 30)
      --match strings      Restrict search to file contents or file path: {file|path}
      --owner strings      Filter on owner
  -R, --repo OWNER/REPO    Filter on repository, in OWNER/REPO format
      --size string        Filter on size range, in kilobytes
  -t, --template string    Format JSON output using a Go template; see "gh help formatting"
  -w, --web                Open the search query in the web browser
```

### Inherited Flags
```text
--help   Show help for command

JSON FIELDS
  path, repository, sha, textMatches, url
```

### Examples
```bash
# Search code matching "react" and "lifecycle"
  $ gh search code react lifecycle
  
  # Search code matching "error handling"
  $ gh search code "error handling"
  
  # Search code using raw search qualifiers as separate arguments
  $ gh search code panic path:pkg language:go
  
  # Search code matching "deque" in Python files
  $ gh search code deque --language=python
  
  # Search code matching "cli" in repositories owned by microsoft organization
  $ gh search code cli --owner=microsoft
  
  # Search code matching "panic" in the GitHub CLI repository
  $ gh search code panic --repo cli/cli
  
  # Search code matching keyword "lint" in package.json files
  $ gh search code lint --filename package.json
```

---

## <a id="cmd-search-commits"></a>`gh search commits`

Search for commits on GitHub.

The command supports constructing queries using the GitHub search syntax,
using the parameter and qualifier flags, or a combination of the two.

GitHub search syntax is documented at:
<https://docs.github.com/search-github/searching-on-github/searching-commits>

For more information on handling search queries containing a hyphen, run `gh search --help`.

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh search commits [<query>] [flags]
```

### Flags
```text
--author string            Filter by author
      --author-date date         Filter based on authored date
      --author-email string      Filter on author email
      --author-name string       Filter on author name
      --committer string         Filter by committer
      --committer-date date      Filter based on committed date
      --committer-email string   Filter on committer email
      --committer-name string    Filter on committer name
      --hash string              Filter by commit hash
  -q, --jq expression            Filter JSON output using a jq expression
      --json fields              Output JSON with the specified fields
  -L, --limit int                Maximum number of commits to fetch (default 30)
      --merge                    Filter on merge commits
      --order string             Order of commits returned, ignored unless '--sort' flag is specified: {asc|desc} (default "desc")
      --owner strings            Filter on repository owner
      --parent string            Filter by parent hash
  -R, --repo OWNER/REPO          Filter on repository, in OWNER/REPO format
      --sort string              Sort fetched commits: {author-date|committer-date} (default "best-match")
  -t, --template string          Format JSON output using a Go template; see "gh help formatting"
      --tree string              Filter by tree hash
      --visibility strings       Filter based on repository visibility: {public|private|internal}
  -w, --web                      Open the search query in the web browser
```

### Inherited Flags
```text
--help   Show help for command

JSON FIELDS
  author, commit, committer, id, parents, repository, sha, url
```

### Examples
```bash
# Search commits matching set of keywords "readme" and "typo"
  $ gh search commits readme typo
  
  # Search commits matching phrase "bug fix"
  $ gh search commits "bug fix"
  
  # Search commits using raw search qualifiers as separate arguments
  $ gh search commits fix author:monalisa merge:false
  
  # Search commits committed by user "monalisa"
  $ gh search commits --committer=monalisa
  
  # Search commits authored by users with name "Jane Doe"
  $ gh search commits --author-name="Jane Doe"
  
  # Search commits matching hash "8dd03144ffdc6c0d486d6b705f9c7fba871ee7c3"
  $ gh search commits --hash=8dd03144ffdc6c0d486d6b705f9c7fba871ee7c3
  
  # Search commits authored before February 1st, 2022
  $ gh search commits --author-date="<2022-02-01"
```

---

## <a id="cmd-search-issues"></a>`gh search issues`

Search for issues on GitHub.

The command supports constructing queries using the GitHub search syntax,
using the parameter and qualifier flags, or a combination of the two.

GitHub search syntax is documented at:
<https://docs.github.com/search-github/searching-on-github/searching-issues-and-pull-requests>

On supported GitHub hosts, advanced issue search syntax can be used in the
search query. Advanced search syntax, like boolean operators `OR`/`AND`,
and parentheses for nesting, must be passed as separate arguments, rather
than within a quoted multi-word string. This syntax is not supported with
`--web`. For more information about advanced issue search, see:
<https://docs.github.com/en/issues/tracking-your-work-with-issues/using-issues/filtering-and-searching-issues-and-pull-requests#building-advanced-filters-for-issues>

Use `--search-type` to select semantic or hybrid (keyword + semantic)
ranking instead of the default lexical search. Semantic and hybrid search are
scoped to issues, are relevance-ranked (so `--sort` and `--order`
cannot be used), return a single page of results, and are not available on
GitHub Enterprise Server.

For more information on handling search queries containing a hyphen, run `gh search --help`.

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh search issues [<query>] [flags]
```

### Flags
```text
--app string             Filter by GitHub App author
      --archived               Filter based on the repository archived state {true|false}
      --assignee string        Filter by assignee
      --author string          Filter by author (use --app to filter by a GitHub App)
      --closed date            Filter on closed at date
      --commenter user         Filter based on comments by user
      --comments number        Filter on number of comments
      --created date           Filter based on created at date
      --include-prs            Include pull requests in results
      --interactions number    Filter on number of reactions and comments
      --involves user          Filter based on involvement of user
  -q, --jq expression          Filter JSON output using a jq expression
      --json fields            Output JSON with the specified fields
      --label strings          Filter on label
      --language string        Filter based on the coding language
  -L, --limit int              Maximum number of results to fetch (default 30)
      --locked                 Filter on locked conversation status
      --match strings          Restrict search to specific field of issue: {title|body|comments}
      --mentions user          Filter based on user mentions
      --milestone title        Filter by milestone title
      --no-assignee            Filter on missing assignee
      --no-label               Filter on missing label
      --no-milestone           Filter on missing milestone
      --no-project             Filter on missing project
      --order string           Order of results returned, ignored unless '--sort' flag is specified: {asc|desc} (default "desc")
      --owner strings          Filter on repository owner
      --project owner/number   Filter on project board owner/number
      --reactions number       Filter on number of reactions
  -R, --repo OWNER/REPO        Filter on repository, in OWNER/REPO format
      --search-type string     Type of issue search to perform: {lexical|semantic|hybrid} (default "lexical")
      --sort string            Sort fetched results: {comments|created|interactions|reactions|reactions-+1|reactions--1|reactions-heart|reactions-smile|reactions-tada|reactions-thinking_face|updated} (default "best-match")
      --state string           Filter based on state: {open|closed}
      --team-mentions string   Filter based on team mentions
  -t, --template string        Format JSON output using a Go template; see "gh help formatting"
      --updated date           Filter on last updated at date
      --visibility strings     Filter based on repository visibility: {public|private|internal}
  -w, --web                    Open the search query in the web browser
```

### Inherited Flags
```text
--help   Show help for command

JSON FIELDS
  assignees, author, authorAssociation, body, closedAt, commentsCount, createdAt,
  id, isLocked, isPullRequest, labels, number, repository, state, title,
  updatedAt, url
```

### Examples
```bash
# Search issues matching set of keywords "readme" and "typo"
  $ gh search issues readme typo
  
  # Search issues matching phrase "broken feature"
  $ gh search issues "broken feature"
  
  # Search issues using raw search qualifiers as separate arguments
  $ gh search issues label:bug author:monalisa state:open
  
  # Search issues and pull requests in cli organization
  $ gh search issues --include-prs --owner=cli
  
  # Search open issues assigned to yourself
  $ gh search issues --assignee=@me --state=open
  
  # Search issues with numerous comments
  $ gh search issues --comments=">100"
  
  # Search issues without label "bug"
  $ gh search issues -- -label:bug
  
  # Search issues only from un-archived repositories (default is all repositories)
  $ gh search issues --owner github --archived=false
  
  # Search issues using semantic (natural-language) ranking
  $ gh search issues "feature broken on web" --search-type semantic
  
  # Search issues using hybrid (keyword + semantic) ranking
  $ gh search issues "feature broken" --search-type hybrid
```

---

## <a id="cmd-search-prs"></a>`gh search prs`

Search for pull requests on GitHub.

The command supports constructing queries using the GitHub search syntax,
using the parameter and qualifier flags, or a combination of the two.

GitHub search syntax is documented at:
<https://docs.github.com/search-github/searching-on-github/searching-issues-and-pull-requests>

On supported GitHub hosts, advanced issue search syntax can be used in the
search query. Advanced search syntax, like boolean operators `OR`/`AND`,
and parentheses for nesting, must be passed as separate arguments, rather
than within a quoted multi-word string. This syntax is not supported with
`--web`. For more information about advanced issue search, see:
<https://docs.github.com/en/issues/tracking-your-work-with-issues/using-issues/filtering-and-searching-issues-and-pull-requests#building-advanced-filters-for-issues>

For more information on handling search queries containing a hyphen, run `gh search --help`.

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh search prs [<query>] [flags]
```

### Flags
```text
--app string              Filter by GitHub App author
      --archived                Filter based on the repository archived state {true|false}
      --assignee string         Filter by assignee
      --author string           Filter by author (use --app to filter by a GitHub App)
  -B, --base string             Filter on base branch name
      --checks string           Filter based on status of the checks: {pending|success|failure}
      --closed date             Filter on closed at date
      --commenter user          Filter based on comments by user
      --comments number         Filter on number of comments
      --created date            Filter based on created at date
      --draft                   Filter based on draft state
  -H, --head string             Filter on head branch name
      --interactions number     Filter on number of reactions and comments
      --involves user           Filter based on involvement of user
  -q, --jq expression           Filter JSON output using a jq expression
      --json fields             Output JSON with the specified fields
      --label strings           Filter on label
      --language string         Filter based on the coding language
  -L, --limit int               Maximum number of results to fetch (default 30)
      --locked                  Filter on locked conversation status
      --match strings           Restrict search to specific field of issue: {title|body|comments}
      --mentions user           Filter based on user mentions
      --merged                  Filter based on merged state
      --merged-at date          Filter on merged at date
      --milestone title         Filter by milestone title
      --no-assignee             Filter on missing assignee
      --no-label                Filter on missing label
      --no-milestone            Filter on missing milestone
      --no-project              Filter on missing project
      --order string            Order of results returned, ignored unless '--sort' flag is specified: {asc|desc} (default "desc")
      --owner strings           Filter on repository owner
      --project owner/number    Filter on project board owner/number
      --reactions number        Filter on number of reactions
  -R, --repo OWNER/REPO         Filter on repository, in OWNER/REPO format
      --review string           Filter based on review status: {none|required|approved|changes_requested}
      --review-requested user   Filter on user or team requested to review
      --reviewed-by user        Filter on user who reviewed
      --sort string             Sort fetched results: {comments|reactions|reactions-+1|reactions--1|reactions-smile|reactions-thinking_face|reactions-heart|reactions-tada|interactions|created|updated} (default "best-match")
      --state string            Filter based on state: {open|closed}
      --team-mentions string    Filter based on team mentions
  -t, --template string         Format JSON output using a Go template; see "gh help formatting"
      --updated date            Filter on last updated at date
      --visibility strings      Filter based on repository visibility: {public|private|internal}
  -w, --web                     Open the search query in the web browser
```

### Inherited Flags
```text
--help   Show help for command

JSON FIELDS
  assignees, author, authorAssociation, body, closedAt, commentsCount, createdAt,
  id, isDraft, isLocked, isPullRequest, labels, number, repository, state, title,
  updatedAt, url
```

### Examples
```bash
# Search pull requests matching set of keywords "fix" and "bug"
  $ gh search prs fix bug
  
  # Search draft pull requests in cli repository
  $ gh search prs --repo=cli/cli --draft
  
  # Search pull requests using raw search qualifiers as separate arguments
  $ gh search prs is:merged author:monalisa
  
  # Search open pull requests requesting your review
  $ gh search prs --review-requested=@me --state=open
  
  # Search merged pull requests assigned to yourself
  $ gh search prs --assignee=@me --merged
  
  # Search pull requests with numerous reactions
  $ gh search prs --reactions=">100"
  
  # Search pull requests without label "bug"
  $ gh search prs -- -label:bug
  
  # Search pull requests only from un-archived repositories (default is all repositories)
  $ gh search prs --owner github --archived=false
```

---

## <a id="cmd-search-repos"></a>`gh search repos`

Search for repositories on GitHub.

The command supports constructing queries using the GitHub search syntax,
using the parameter and qualifier flags, or a combination of the two.

GitHub search syntax is documented at:
<https://docs.github.com/search-github/searching-on-github/searching-for-repositories>

For more information on handling search queries containing a hyphen, run `gh search --help`.

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh search repos [<query>] [flags]
```

### Flags
```text
--archived                    Filter based on the repository archived state {true|false}
      --created date                Filter based on created at date
      --followers number            Filter based on number of followers
      --forks number                Filter on number of forks
      --good-first-issues number    Filter on number of issues with the 'good first issue' label
      --help-wanted-issues number   Filter on number of issues with the 'help wanted' label
      --include-forks string        Include forks in fetched repositories: {false|true|only}
  -q, --jq expression               Filter JSON output using a jq expression
      --json fields                 Output JSON with the specified fields
      --language string             Filter based on the coding language
      --license strings             Filter based on license type
  -L, --limit int                   Maximum number of repositories to fetch (default 30)
      --match strings               Restrict search to specific field of repository: {name|description|readme}
      --number-topics number        Filter on number of topics
      --order string                Order of repositories returned, ignored unless '--sort' flag is specified: {asc|desc} (default "desc")
      --owner strings               Filter on owner
      --size string                 Filter on a size range, in kilobytes
      --sort string                 Sort fetched repositories: {forks|help-wanted-issues|stars|updated} (default "best-match")
      --stars number                Filter on number of stars
  -t, --template string             Format JSON output using a Go template; see "gh help formatting"
      --topic strings               Filter on topic
      --updated date                Filter on last updated at date
      --visibility strings          Filter based on visibility: {public|private|internal}
  -w, --web                         Open the search query in the web browser
```

### Inherited Flags
```text
--help   Show help for command

JSON FIELDS
  createdAt, defaultBranch, description, forksCount, fullName, hasDownloads,
  hasIssues, hasPages, hasProjects, hasWiki, homepage, id, isArchived, isDisabled,
  isFork, isPrivate, language, license, name, openIssuesCount, owner, pushedAt,
  size, stargazersCount, updatedAt, url, visibility, watchersCount
```

### Examples
```bash
# Search repositories matching set of keywords "cli" and "shell"
  $ gh search repos cli shell
  
  # Search repositories matching phrase "vim plugin"
  $ gh search repos "vim plugin"
  
  # Search repositories using raw search qualifiers as separate arguments
  $ gh search repos topic:github 'stars:>5000'
  
  # Search repositories public repos in the microsoft organization
  $ gh search repos --owner=microsoft --visibility=public
  
  # Search repositories with a set of topics
  $ gh search repos --topic=unix,terminal
  
  # Search repositories by coding language and number of good first issues
  $ gh search repos --language=go --good-first-issues=">=10"
  
  # Search repositories without topic "linux"
  $ gh search repos -- -topic:linux
  
  # Search repositories excluding archived repositories
  $ gh search repos --archived=false
```

---

## <a id="cmd-secret"></a>`gh secret`

Secrets can be set at the repository, or organization level for use in
GitHub Actions, Agents, or Dependabot. User, organization, and repository secrets can be set for
use in GitHub Codespaces. Environment secrets can be set for use in
GitHub Actions. Run `gh help secret set` to learn how to get started.

### Synopsis
```bash
gh secret <command> [flags]

AVAILABLE COMMANDS
  delete:        Delete secrets
  list:          List secrets
  set:           Create or update secrets
```

### Flags
```text
-R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-secret-delete"></a>`gh secret delete`

Delete a secret on one of the following levels:
- repository (default): available to GitHub Actions runs, Agents sessions, or Dependabot in a repository
- environment: available to GitHub Actions runs for a deployment environment in a repository
- organization: available to GitHub Actions runs, Agents sessions, Dependabot, or Codespaces within an organization
- user: available to Codespaces for your user

### Synopsis
```bash
gh secret delete <secret-name> [flags]
```

### Aliases
`gh secret remove`

### Flags
```text
-a, --app string   Delete a secret for a specific application: {actions|agents|codespaces|dependabot}
  -e, --env string   Delete a secret for an environment
  -o, --org string   Delete a secret for an organization
  -u, --user         Delete a secret for your user
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

---

## <a id="cmd-secret-list"></a>`gh secret list`

List secrets on one of the following levels:
- repository (default): available to GitHub Actions runs, Agents sessions, or Dependabot in a repository
- environment: available to GitHub Actions runs for a deployment environment in a repository
- organization: available to GitHub Actions runs, Agents sessions, Dependabot, or Codespaces within an organization
- user: available to Codespaces for your user

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh secret list [flags]
```

### Aliases
`gh secret ls`

### Flags
```text
-a, --app string        List secrets for a specific application: {actions|agents|codespaces|dependabot}
  -e, --env string        List secrets for an environment
  -q, --jq expression     Filter JSON output using a jq expression
      --json fields       Output JSON with the specified fields
  -o, --org string        List secrets for an organization
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
  -u, --user              List a secret for your user
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format

JSON FIELDS
  name, numSelectedRepos, selectedReposURL, updatedAt, visibility
```

---

## <a id="cmd-secret-set"></a>`gh secret set`

Set a value for a secret on one of the following levels:
- repository (default): available to GitHub Actions runs, Agents sessions, or Dependabot in a repository
- environment: available to GitHub Actions runs for a deployment environment in a repository
- organization: available to GitHub Actions runs, Agents sessions, Dependabot, or Codespaces within an organization
- user: available to Codespaces for your user

Organization and user secrets can optionally be restricted to only be available to
specific repositories.

Secret values are locally encrypted before being sent to GitHub.

### Synopsis
```bash
gh secret set <secret-name> [flags]
```

### Flags
```text
-a, --app string           Set the application for a secret: {actions|agents|codespaces|dependabot}
  -b, --body string          The value for the secret (reads from standard input if not specified)
  -e, --env environment      Set deployment environment secret
  -f, --env-file file        Load secret names and values from a dotenv-formatted file
      --no-repos-selected    No repositories can access the organization secret
      --no-store             Print the encrypted, base64-encoded value instead of storing it on GitHub
  -o, --org organization     Set organization secret
  -r, --repos repositories   List of repositories that can access an organization or user secret
  -u, --user                 Set a secret for your user
  -v, --visibility string    Set visibility for an organization secret: {all|private|selected} (default "private")
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Examples
```bash
# Paste secret value for the current repository in an interactive prompt
  $ gh secret set MYSECRET
  
  # Read secret value from an environment variable
  $ gh secret set MYSECRET --body "$ENV_VALUE"
  
  # Set secret for a specific remote repository
  $ gh secret set MYSECRET --repo origin/repo --body "$ENV_VALUE"
  
  # Read secret value from a file
  $ gh secret set MYSECRET < myfile.txt
  
  # Set secret for a deployment environment in the current repository
  $ gh secret set MYSECRET --env myenvironment
  
  # Set organization-level secret visible to both public and private repositories
  $ gh secret set MYSECRET --org myOrg --visibility all
  
  # Set organization-level secret visible to specific repositories
  $ gh secret set MYSECRET --org myOrg --repos repo1,repo2,repo3
  
  # Set organization-level secret visible to no repositories
  $ gh secret set MYSECRET --org myOrg --no-repos-selected
  
  # Set user-level secret for Codespaces
  $ gh secret set MYSECRET --user
  
  # Set repository-level secret for Dependabot
  $ gh secret set MYSECRET --app dependabot
  
  # Set multiple secrets imported from the ".env" file
  $ gh secret set -f .env
  
  # Set multiple secrets from stdin
  $ gh secret set -f - < myfile.txt
```

---

## <a id="cmd-skill"></a>`gh skill`

Install and manage agent skills from GitHub repositories.

Working with agent skills in the GitHub CLI is in preview and
subject to change without notice.

### Synopsis
```bash
gh skill <command> [flags]
```

### Aliases
`gh skills`, ``, `AVAILABLE COMMANDS`, `  install:       Install agent skills from a GitHub repository (preview)`, `  list:          List installed skills (preview)`, `  preview:       Preview a skill from a GitHub repository (preview)`, `  publish:       Validate and publish skills to a GitHub repository (preview)`, `  search:        Search for skills across GitHub (preview)`, `  update:        Update installed skills to their latest versions (preview)`

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Search for skills
  $ gh skill search terraform
  
  # Install a skill
  $ gh skill install github/awesome-copilot documentation-writer
  
  # List installed skills
  $ gh skill list
  
  # Preview a skill before installing
  $ gh skill preview github/awesome-copilot documentation-writer
  
  # Update all installed skills
  $ gh skill update --all
  
  # Validate skills for publishing
  $ gh skill publish --dry-run
```

---

## <a id="cmd-skill-install"></a>`gh skill install`

Install agent skills from a GitHub repository or local directory into
your local environment. Skills are placed in a host-specific directory
at either project scope (inside the current git repository) or user
scope (in your home directory, available everywhere).

A wide range of AI coding agents are supported, including GitHub
Copilot, Claude Code, Cursor, Codex, Gemini CLI, Antigravity, Amp,
Devin, Goose, Grok, Junie, OpenCode, and many more.

Supported `--agent` values:

  - GitHub Copilot (github-copilot)
  - Claude Code (claude-code)
  - Cursor (cursor)
  - Codex (codex)
  - Gemini CLI (gemini-cli)
  - Antigravity (antigravity)
  - Antigravity CLI (antigravity-cli)
  - Antigravity 2.0 (antigravity2.0)
  - AdaL (adal)
  - Amp (amp)
  - Augment (augment)
  - IBM Bob (bob)
  - Cline (cline)
  - CodeBuddy (codebuddy)
  - Command Code (command-code)
  - Continue (continue)
  - Cortex Code (cortex)
  - Crush (crush)
  - Deep Agents (deepagents)
  - Devin (devin)
  - Droid (droid)
  - Firebender (firebender)
  - Goose (goose)
  - Grok (grok)
  - iFlow CLI (iflow-cli)
  - Junie (junie)
  - Kilo Code (kilo)
  - Kimi Code CLI (kimi-cli)
  - Kiro CLI (kiro-cli)
  - Kode (kode)
  - MCPJam (mcpjam)
  - Mistral Vibe (mistral-vibe)
  - Mux (mux)
  - Neovate (neovate)
  - OpenClaw (openclaw)
  - OpenCode (opencode)
  - OpenHands (openhands)
  - Pi (pi)
  - Pochi (pochi)
  - Qoder (qoder)
  - Qwen Code (qwen-code)
  - Replit (replit)
  - Roo Code (roo)
  - Trae (trae)
  - Trae CN (trae-cn)
  - Universal (universal)
  - Warp (warp)
  - Zencoder (zencoder)

Use `--agent` and `--scope` to control placement, or `--dir` for a
custom directory. The default scope is `project`, and the default
agent is `github-copilot` (when running non-interactively).

At project scope, several agents (including GitHub Copilot, Cursor,
Codex, Gemini CLI, Antigravity, Amp, Cline, OpenCode, and Warp) share
the `.agents/skills` directory. If you select multiple hosts that
resolve to the same destination, each skill is installed there only once.

The first argument is a GitHub repository in `OWNER/REPO` format.
Use `--from-local` to install from a local directory instead.
Local skills are auto-discovered using the same conventions as remote
repositories, and files are copied (not symlinked) with local-path
tracking metadata injected into frontmatter.

Skills are discovered automatically using the `skills/*/SKILL.md` convention
defined by the Agent Skills specification, including when the `skills/`
directory is nested under a prefix (e.g. `terraform/code-generation/skills/...`).
For more information on the specification,
see: https://agentskills.io/specification

The skill argument can be a name, a namespaced name (`author/skill`),
or an exact path within the repository (`skills/author/skill`,
`packages/agent-skills/code-review`, or any `.../SKILL.md` path).
Namespaced names with one slash are matched by name. Use a `SKILL.md`
suffix to force a one-directory path outside the standard conventions.

Performance tip: when installing from a large repository with many
skills, providing an exact path instead of a skill name avoids a
full tree traversal of the repository, making the install significantly faster.

When a skill name is provided without a version, the CLI resolves the
version in this order:

  1. Latest tagged release in the repository
  2. Default branch HEAD

To pin to a specific version, either append `@VERSION` to the skill
name or use the `--pin` flag. The version is resolved as a git tag or commit SHA.

Installed skills have source tracking metadata injected into their
frontmatter. This metadata identifies the source repository and
enables `gh skill update` to detect changes.

When run interactively, the command prompts for any missing arguments.

Use `--all` to install every discovered skill from the repository
without prompting for skill selection. When run non-interactively,
`repository` is required; without a skill name or `--all` the
matching skills are listed (as tab-separated values when piped) so you can
browse or filter them with tools like `grep` before re-running with
a specific skill.

### Synopsis
```bash
gh skill install <repository> [<skill[@version]>] [flags]
```

### Aliases
`gh skill add, gh skills add`

### Flags
```text
--agent string        Target agent (see supported values above)
      --all                 Install all skills without prompting for skill selection
      --allow-hidden-dirs   Include skills in hidden directories (e.g. .claude/skills/, .agents/skills/)
      --dir string          Install to a custom directory (overrides --agent and --scope)
  -f, --force               Overwrite existing skills without prompting
      --from-local          Treat the argument as a local directory path instead of a repository
      --pin string          Pin to a specific git tag or commit SHA
      --scope string        Installation scope: {project|user} (default "project")
      --upstream            Install from the upstream source when a re-published skill is detected
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Interactive: choose repo, skill, and agent
  $ gh skill install
  
  # Choose a skill from the repo interactively
  $ gh skill install github/awesome-copilot
  
  # List available skills non-interactively (e.g. to pipe into grep)
  $ gh skill install github/awesome-copilot | grep review
  
  # Install a specific skill
  $ gh skill install github/awesome-copilot git-commit
  
  # Install all skills from a repository
  $ gh skill install github/awesome-copilot --all
  
  # Install a specific version
  $ gh skill install github/awesome-copilot git-commit@v1.2.0
  
  # Install from a large namespaced repo by path (efficient, skips full discovery)
  $ gh skill install github/awesome-copilot skills/monalisa/code-review
  
  # Install from a non-standard nested path (efficient, skips full discovery)
  $ gh skill install monalisa/skills-repo packages/agent-skills/code-review
  
  # Install from a local directory
  $ gh skill install ./my-skills-repo --from-local
  
  # Install a specific local skill
  $ gh skill install ./my-skills-repo git-commit --from-local
  
  # Install for Claude Code at user scope
  $ gh skill install github/awesome-copilot git-commit --agent claude-code --scope user
  
  # Pin to a specific git ref
  $ gh skill install github/awesome-copilot git-commit --pin v2.0.0
  
  # Install skills from hidden directories (e.g. .claude/skills/)
  $ gh skill install owner/repo --allow-hidden-dirs
```

---

## <a id="cmd-skill-list"></a>`gh skill list`

List installed agent skills across known agent host directories.

By default, scans all supported agent hosts in both project and user scope.
Use `--agent` to scan one host, `--scope` to scan only project or user
scope, or `--dir` to scan a custom skills directory.

Project-scope skills are discovered relative to the current git repository
root. User-scope skills are discovered relative to your home directory.

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh skill list [flags]
```

### Aliases
`gh skill ls, gh skills ls`

### Flags
```text
--agent string      Filter by target agent: {github-copilot|claude-code|cursor|codex|gemini-cli|antigravity|antigravity-cli|antigravity2.0|adal|amp|augment|bob|cline|codebuddy|command-code|continue|cortex|crush|deepagents|devin|droid|firebender|goose|grok|iflow-cli|junie|kilo|kimi-cli|kiro-cli|kode|mcpjam|mistral-vibe|mux|neovate|openclaw|opencode|openhands|pi|pochi|qoder|qwen-code|replit|roo|trae|trae-cn|universal|warp|zencoder}
      --dir string        Scan a custom directory for installed skills
  -q, --jq expression     Filter JSON output using a jq expression
      --json fields       Output JSON with the specified fields
      --scope string      Filter by installation scope: {project|user}
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
```

### Inherited Flags
```text
--help   Show help for command

JSON FIELDS
  agentHosts, path, pinned, scope, skillName, sourceURL, version
```

### Examples
```bash
# List all installed skills
  $ gh skill list
  
  # List skills installed for GitHub Copilot
  $ gh skill list --agent github-copilot
  
  # List user-scope skills
  $ gh skill list --scope user
  
  # List skills as JSON
  $ gh skill list --json skillName,sourceURL,scope,version,pinned,path
```

---

## <a id="cmd-skill-preview"></a>`gh skill preview`

Render a skill's `SKILL.md` content in the terminal. This fetches the
skill file from the repository and displays it using the configured
pager, without installing anything.

A file tree is shown first, followed by the rendered `SKILL.md` content.
When running interactively and the skill contains additional files
(scripts, references, etc.), a file picker lets you browse them
individually.

When run with only a repository argument, lists available skills and
prompts for selection.

The skill argument can be a name, a namespaced name (`author/skill`),
or an exact path within the repository (`skills/author/skill`,
`packages/agent-skills/code-review`, or any `.../SKILL.md` path).
Namespaced names with one slash are matched by name. Use a `SKILL.md`
suffix to force a one-directory path outside the standard conventions.

To preview a specific version of the skill, append `@VERSION` to the
skill name. The version is resolved as a git tag, branch, or commit SHA.

### Synopsis
```bash
gh skill preview <repository> [<skill>] [flags]
```

### Aliases
`gh skill show, gh skills show`

### Flags
```text
--allow-hidden-dirs   Include skills in hidden directories (e.g. .claude/skills/, .agents/skills/)
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Preview a specific skill
  $ gh skill preview github/awesome-copilot documentation-writer
  
  # Preview a skill at a specific version
  $ gh skill preview github/awesome-copilot documentation-writer@v1.2.0
  
  # Preview a skill at a specific commit SHA
  $ gh skill preview github/awesome-copilot documentation-writer@abc123def456
  
  # Preview from a non-standard nested path (efficient, skips full discovery)
  $ gh skill preview monalisa/skills-repo packages/agent-skills/code-review
  
  # Browse and preview interactively
  $ gh skill preview github/awesome-copilot
```

---

## <a id="cmd-skill-publish"></a>`gh skill publish`

Validate a local repository's skills against the Agent Skills specification
and publish them by creating a GitHub release.

Skills are discovered using the same conventions as install:

  - `skills/*/SKILL.md`
  - `skills/{scope}/*/SKILL.md`
  - `*/SKILL.md` (root-level)
  - `plugins/{scope}/skills/*/SKILL.md`

Validation checks include:

  - Skill names match the strict agentskills.io naming rules
  - Each skill name matches its directory name
  - Required frontmatter fields (name, description) are present
  - allowed-tools is a string, not an array
  - Install metadata (`metadata.github-*`) is stripped if present

After validation passes, publish will interactively guide you through:

  - Adding the `agent-skills` topic to the repository
  - Choosing a version tag (semver recommended)
  - Creating a GitHub release with auto-generated notes

Use `--dry-run` to validate without publishing.
Use `--tag` to publish non-interactively with a specific tag.
Use `--fix` to automatically strip install metadata from committed files
without publishing. Review and commit the changes, then run publish again.

### Synopsis
```bash
gh skill publish [<directory>] [flags]
```

### Flags
```text
--dry-run      Validate without publishing
  --fix          Auto-fix issues where possible without publishing (e.g. strip install metadata)
  --tag string   Version tag for the release (e.g. v1.0.0)
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Validate and publish interactively
  $ gh skill publish
  
  # Publish with a specific tag (non-interactive)
  $ gh skill publish --tag v1.0.0
  
  # Validate only (no publish)
  $ gh skill publish --dry-run
  
  # Strip install metadata without publishing
  $ gh skill publish --fix
```

---

## <a id="cmd-skill-search"></a>`gh skill search`

Search across all public GitHub repositories for skills matching a keyword.

Uses the GitHub Code Search API to find `SKILL.md` files whose name or
description matches the query term.

Results are ranked by relevance: skills whose name contains the query
term appear first.

Use `--owner` to scope results to a specific GitHub user or organization.

In interactive mode, you can select skills from the results to install directly.

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh skill search <query> [flags]
```

### Flags
```text
-q, --jq expression     Filter JSON output using a jq expression
      --json fields       Output JSON with the specified fields
  -L, --limit int         Maximum number of results per page (default 15)
      --owner string      Filter results to a specific GitHub user or organization
      --page int          Page number of results to fetch (default 1)
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
```

### Inherited Flags
```text
--help   Show help for command

JSON FIELDS
  description, namespace, path, repo, skillName, stars
```

### Examples
```bash
# Search for skills related to terraform
  $ gh skill search terraform
  
  # Search for skills from a specific owner
  $ gh skill search terraform --owner hashicorp
  
  # View the second page of results
  $ gh skill search terraform --page 2
  
  # Limit results to 5
  $ gh skill search terraform --limit 5
```

---

## <a id="cmd-skill-update"></a>`gh skill update`

Checks installed skills for available updates by comparing the local
tree SHA (from `SKILL.md` frontmatter) against the remote repository.

Scans all known agent host directories (including Copilot, Claude, Cursor,
Gemini, Antigravity, Grok, and others) in both project and user scope automatically.

Without arguments, checks all installed skills. With skill names,
checks only those specific skills.

Pinned skills (installed with `--pin`) are skipped with a notice.
Use `--unpin` to clear the pinned version and include those skills
in the update.

Skills without GitHub metadata (e.g. installed manually or by another
tool) are prompted for their source repository in interactive mode.
With `--all` or in non-interactive mode, they are skipped with a notice.
The update re-downloads the skill with metadata injected, so future
updates work automatically.

With `--force`, re-downloads skills even when the remote version matches
the local tree SHA. This overwrites locally modified skill files with
their original content, but does not remove extra files added locally.

In interactive mode, shows which skills have updates and asks for
confirmation before proceeding. With `--all`, updates without prompting.
With `--dry-run`, reports available updates without modifying any files.

### Synopsis
```bash
gh skill update [<skill>...] [flags]
```

### Flags
```text
--all          Update all skills without prompting
  --dir string   Scan a custom directory for installed skills
  --dry-run      Report available updates without modifying files
  --force        Re-download even if already up to date
  --unpin        Clear pinned version and include pinned skills in update
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
# Check and update all skills interactively
  $ gh skill update
  
  # Update specific skills
  $ gh skill update mcp-cli git-commit
  
  # Update all without prompting
  $ gh skill update --all
  
  # Re-download all skills (restore locally modified files)
  $ gh skill update --force --all
  
  # Check for updates without applying (read-only)
  $ gh skill update --dry-run
  
  # Unpin skills and update them to latest
  $ gh skill update --unpin
```

---

## <a id="cmd-ssh-key"></a>`gh ssh-key`

Manage SSH keys registered with your GitHub account.

### Synopsis
```bash
gh ssh-key <command> [flags]

AVAILABLE COMMANDS
  add:           Add an SSH key to your GitHub account
  delete:        Delete an SSH key from your GitHub account
  list:          Lists SSH keys in your GitHub account
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-ssh-key-add"></a>`gh ssh-key add`

Add an SSH key to your GitHub account

### Synopsis
```bash
gh ssh-key add [<key-file>] [flags]
```

### Flags
```text
-t, --title string   Title for the new key
      --type string    Type of the ssh key: {authentication|signing} (default "authentication")
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-ssh-key-delete"></a>`gh ssh-key delete`

Delete an SSH key from your GitHub account

### Synopsis
```bash
gh ssh-key delete <id> [flags]
```

### Flags
```text
-y, --yes   Skip the confirmation prompt
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-ssh-key-list"></a>`gh ssh-key list`

Lists SSH keys in your GitHub account

### Synopsis
```bash
gh ssh-key list [flags]
```

### Aliases
`gh ssh-key ls`

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-status"></a>`gh status`

The status command prints information about your work on GitHub across all the repositories you're subscribed to, including:

- Assigned Issues
- Assigned Pull Requests
- Review Requests
- Mentions
- Repository Activity (new issues/pull requests, comments)

### Synopsis
```bash
gh status [flags]
```

### Flags
```text
-e, --exclude strings   Comma separated list of repos to exclude in owner/name format
  -o, --org string        Report status within an organization
```

### Inherited Flags
```text
--help   Show help for command
```

### Examples
```bash
$ gh status -e cli/cli -e cli/go-gh # Exclude multiple repositories
  $ gh status -o cli # Limit results to a single organization
```

---

## <a id="cmd-variable"></a>`gh variable`

Variables can be set at the repository, environment or organization level for use in
GitHub Actions or Dependabot. Run `gh help variable set` to learn how to get started.

### Synopsis
```bash
gh variable <command> [flags]

AVAILABLE COMMANDS
  delete:        Delete variables
  get:           Get variables
  list:          List variables
  set:           Create or update variables
```

### Flags
```text
-R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-variable-delete"></a>`gh variable delete`

Delete a variable on one of the following levels:
- repository (default): available to GitHub Actions runs or Dependabot in a repository
- environment: available to GitHub Actions runs for a deployment environment in a repository
- organization: available to GitHub Actions runs or Dependabot within an organization

### Synopsis
```bash
gh variable delete <variable-name> [flags]
```

### Aliases
`gh variable remove`

### Flags
```text
-e, --env string   Delete a variable for an environment
  -o, --org string   Delete a variable for an organization
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

---

## <a id="cmd-variable-get"></a>`gh variable get`

Get a variable on one of the following levels:
- repository (default): available to GitHub Actions runs or Dependabot in a repository
- environment: available to GitHub Actions runs for a deployment environment in a repository
- organization: available to GitHub Actions runs or Dependabot within an organization

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh variable get <variable-name> [flags]
```

### Flags
```text
-e, --env string        Get a variable for an environment
  -q, --jq expression     Filter JSON output using a jq expression
      --json fields       Output JSON with the specified fields
  -o, --org string        Get a variable for an organization
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format

JSON FIELDS
  createdAt, name, numSelectedRepos, selectedReposURL, updatedAt, value,
  visibility
```

---

## <a id="cmd-variable-list"></a>`gh variable list`

List variables on one of the following levels:
- repository (default): available to GitHub Actions runs or Dependabot in a repository
- environment: available to GitHub Actions runs for a deployment environment in a repository
- organization: available to GitHub Actions runs or Dependabot within an organization

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh variable list [flags]
```

### Aliases
`gh variable ls`

### Flags
```text
-e, --env string        List variables for an environment
  -q, --jq expression     Filter JSON output using a jq expression
      --json fields       Output JSON with the specified fields
  -o, --org string        List variables for an organization
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format

JSON FIELDS
  createdAt, name, numSelectedRepos, selectedReposURL, updatedAt, value,
  visibility
```

---

## <a id="cmd-variable-set"></a>`gh variable set`

Set a value for a variable on one of the following levels:
- repository (default): available to GitHub Actions runs or Dependabot in a repository
- environment: available to GitHub Actions runs for a deployment environment in a repository
- organization: available to GitHub Actions runs or Dependabot within an organization

Organization variable can optionally be restricted to only be available to
specific repositories.

### Synopsis
```bash
gh variable set <variable-name> [flags]
```

### Flags
```text
-b, --body string          The value for the variable (reads from standard input if not specified)
  -e, --env environment      Set deployment environment variable
  -f, --env-file file        Load variable names and values from a dotenv-formatted file
  -o, --org organization     Set organization variable
  -r, --repos repositories   List of repositories that can access an organization variable
  -v, --visibility string    Set visibility for an organization variable: {all|private|selected} (default "private")
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Examples
```bash
# Add variable value for the current repository in an interactive prompt
  $ gh variable set MYVARIABLE
  
  # Read variable value from an environment variable
  $ gh variable set MYVARIABLE --body "$ENV_VALUE"
  
  # Read variable value from a file
  $ gh variable set MYVARIABLE < myfile.txt
  
  # Set variable for a deployment environment in the current repository
  $ gh variable set MYVARIABLE --env myenvironment
  
  # Set organization-level variable visible to both public and private repositories
  $ gh variable set MYVARIABLE --org myOrg --visibility all
  
  # Set organization-level variable visible to specific repositories
  $ gh variable set MYVARIABLE --org myOrg --repos repo1,repo2,repo3
  
  # Set multiple variables imported from the ".env" file
  $ gh variable set -f .env
```

---

## <a id="cmd-workflow"></a>`gh workflow`

List, view, and run workflows in GitHub Actions.

### Synopsis
```bash
gh workflow <command> [flags]

AVAILABLE COMMANDS
  disable:       Disable a workflow
  enable:        Enable a workflow
  list:          List workflows
  run:           Run a workflow by creating a workflow_dispatch event
  view:          View the summary of a workflow
```

### Flags
```text
-R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Inherited Flags
```text
--help   Show help for command
```

---

## <a id="cmd-workflow-disable"></a>`gh workflow disable`

Disable a workflow, preventing it from running or showing up when listing workflows.

### Synopsis
```bash
gh workflow disable [<workflow-id> | <workflow-name>] [flags]
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

---

## <a id="cmd-workflow-enable"></a>`gh workflow enable`

Enable a workflow, allowing it to be run and show up when listing workflows.

### Synopsis
```bash
gh workflow enable [<workflow-id> | <workflow-name>] [flags]
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

---

## <a id="cmd-workflow-list"></a>`gh workflow list`

List workflow files, hiding disabled workflows by default.

For more information about output formatting flags, see `gh help formatting`.

### Synopsis
```bash
gh workflow list [flags]
```

### Aliases
`gh workflow ls`

### Flags
```text
-a, --all               Include disabled workflows
  -q, --jq expression     Filter JSON output using a jq expression
      --json fields       Output JSON with the specified fields
  -L, --limit int         Maximum number of workflows to fetch (default 50)
  -t, --template string   Format JSON output using a Go template; see "gh help formatting"
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format

JSON FIELDS
  id, name, path, state
```

---

## <a id="cmd-workflow-run"></a>`gh workflow run`

Create a `workflow_dispatch` event for a given workflow.

This command will trigger GitHub Actions to run a given workflow file. The given workflow file must
support an `on.workflow_dispatch` trigger in order to be run in this way.

If the workflow file supports inputs, they can be specified in a few ways:

- Interactively
- Via `-f/--raw-field` or `-F/--field` flags
- As JSON, via standard input

The created workflow run URL will be returned if available.

### Synopsis
```bash
gh workflow run [<workflow-id> | <workflow-name>] [flags]
```

### Flags
```text
-F, --field key=value       Add a string parameter in key=value format, respecting @ syntax (see "gh help api").
      --json                  Read workflow inputs as JSON via STDIN
  -f, --raw-field key=value   Add a string parameter in key=value format
  -r, --ref string            Branch or tag name which contains the version of the workflow file you'd like to run
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Examples
```bash
# Have gh prompt you for what workflow you'd like to run and interactively collect inputs
  $ gh workflow run
  
  # Run the workflow file 'triage.yml' at the remote's default branch
  $ gh workflow run triage.yml
  
  # Run the workflow file 'triage.yml' at a specified ref
  $ gh workflow run triage.yml --ref my-branch
  
  # Run the workflow file 'triage.yml' with command line inputs
  $ gh workflow run triage.yml -f name=scully -f greeting=hello
  
  # Run the workflow file 'triage.yml' with JSON via standard input
  $ echo '{"name":"scully", "greeting":"hello"}' | gh workflow run triage.yml --json
```

---

## <a id="cmd-workflow-view"></a>`gh workflow view`

View the summary of a workflow

### Synopsis
```bash
gh workflow view [<workflow-id> | <workflow-name> | <filename>] [flags]
```

### Flags
```text
-r, --ref string   The branch or tag name which contains the version of the workflow file you'd like to view
  -w, --web          Open workflow in the browser
  -y, --yaml         View the workflow yaml file
```

### Inherited Flags
```text
--help                     Show help for command
  -R, --repo [HOST/]OWNER/REPO   Select another repository using the [HOST/]OWNER/REPO format
```

### Examples
```bash
# Interactively select a workflow to view
  $ gh workflow view
  
  # View a specific workflow
  $ gh workflow view 0451
```

---
