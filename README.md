# Awesome Maki [![Awesome](https://awesome.re/badge-flat.svg)](https://awesome.re)

<a href="https://maki.sh"><img src="https://raw.githubusercontent.com/tontinton/maki/main/site/android-chrome-512x512.png" alt="Maki logo" align="right" width="144"></a>

> [Maki](https://github.com/tontinton/maki) is an AI coding agent with a Lua extension API, built for efficient use of context tokens.

> [!IMPORTANT]
> **Installation reminder:** Maki maintainer [Tony](https://github.com/tontinton) [recommends documenting plugin installation with `maki.pack.add`](https://github.com/tontinton/maki/pull/1268#pullrequestreview-5548304143). Some projects still use manual installation or repository subdirectories. Follow each project's instructions; not every repository is an installable package. Authors: please provide a working `maki.pack.add` example when your project supports it.

A curation of useful Maki extensions, selected for a clear benefit, understandable setup, and supporting maintenance or test evidence. The forum and the maki.sh plugin catalog are discovery sources; inclusion here requires a separate review.

## Contents

- [Selection Criteria](#selection-criteria)
- [Agent Workflows](#agent-workflows)
- [Providers](#providers)
- [Web Search](#web-search)
- [Permissions](#permissions)
- [Observability](#observability)
- [Plugin Development](#plugin-development)
- [Resources](#resources)

## Selection Criteria

**Useful:** Adds a clear capability and explains how the reader benefits.

**Usable:** Has setup instructions and known dependencies, with any small correction stated here. Unresolved installation or API blockers keep an entry out.

**Supported:** Has evidence of compatibility work, meaningful tests, or continued author support. A recent commit or high star count alone is insufficient.

**Selective:** Incomplete examples, uncertain compatibility, and projects with little use evidence stay in the separate review notes, with reasons and a path to reconsideration.

The same criteria apply to the maintainer's own projects. We prefer a short, useful list to a complete forum index.

## Agent Workflows

- [laudney/maki-essential-plugins](https://github.com/laudney/maki-essential-plugins) - Keep an agent working toward a persistent goal, monitor background commands, and switch between saved provider logins with `/provider`. Uses `maki.pack.add`; requires Maki 0.6.0+. Optional RunInfra and Fireworks AI discovery uses the providers' own model APIs; requires Maki 0.6.3+, an API key, and explicit provider selection.
- [aidalgol/maki-specialist-subagents](https://github.com/aidalgol/maki-specialist-subagents) - Define review and implementation specialists, delegate to them in parallel or in the background, and skip reviews already recorded in a ledger. Uses `maki.pack.add`; requires Maki 0.7.0+ and requests `agent`, `run`, file, and `net` permissions. New in November 2026; unit tests cover the logic, and the author tests live delegation manually.

## Providers

- [sdroege/maki-plugins](https://github.com/sdroege/maki-plugins) - Add GreenPT, Inference Cooperative, or a local Strata server as a provider, each in its own package directory. Manual installation: symlink or copy the provider's directory into Maki's package path, because `maki.pack.add` cannot load this monorepo. Requires Maki 0.6.0+ and the provider's API key or local endpoint. The provider plugins have no automated tests.

## Web Search

- [bzzimmy/maki-parallel](https://github.com/bzzimmy/maki-parallel) - Retrieve focused search excerpts and page content through Parallel, with login and diagnostic commands. Uses `maki.pack.add`; requires a Parallel API key. Includes real Maki host integration tests. Disable the built-in web tools as documented.
- [g4bwy/maki-plugins/websearch](https://github.com/g4bwy/maki-plugins/tree/master/websearch) - Use your own SearXNG instance for web search instead of a hosted search API. Manual installation; requires JSON search support and a network allowlist for private hosts. Grant both `net` and `env` permissions; the upstream installation example omits `env`.

## Permissions

- [sdroege/maki-plugins/bash-filter](https://github.com/sdroege/maki-plugins/tree/main/bash-filter) - Reject `git diff` calls that would print an external-diff patch, and auto-allow `sed` commands whose script only prints. Manual installation from the monorepo, as for the providers; requires Maki 0.5.0+. Tests parse real shell commands with the tree-sitter bash grammar.

## Observability

- [g4bwy/maki-plugins/token-metrics](https://github.com/g4bwy/maki-plugins/tree/master/token-metrics) - Inspect vLLM throughput, prefix caching, speculative decoding, and queue state in a live panel. Manual installation; requires access to the server's Prometheus `/metrics` endpoint and the documented permissions. Values describe the whole server, including other clients.

## Plugin Development

- [lu-zero/maki-lua-plugin-template](https://github.com/lu-zero/maki-lua-plugin-template) - Start a Lua extension with a permissions manifest, real Maki host integration tests, and CI through `cargo-generate`. A development template, not a package to install in Maki.

## Resources

- [Maki Documentation](https://maki.sh/docs) - Setup, configuration, permissions, and usage.
- [Plugin Guide](https://maki.sh/docs/plugins) - Lua modules, permissions, and development.
- [Lua API Reference](https://maki.sh/docs/lua-api) - Package management, tools, commands, events, providers, and UI.
- [Provider Guide](https://maki.sh/docs/providers) - Custom providers, package selection, and migration from executable scripts.
- [Plugin Catalog](https://maki.sh/plugins) - Every public GitHub repository tagged `maki` and `plugin`, listed automatically and not reviewed.
- [Plugin Showcase](https://github.com/tontinton/maki/discussions/452) - Author announcements and demos, including experiments outside this curation.

## Contributing

Suggest a project or correct an entry through a pull request. Read [CONTRIBUTING.md](CONTRIBUTING.md) for the selection criteria and evidence to include. Authors are welcome to submit their own work.

## Footnotes

Maintained by [laudney](https://github.com/laudney). This is an independent community curation. The category and entry format follows [awesome-neovim](https://github.com/rockerBOO/awesome-neovim).

The first review covered all 14 public Maki forum discussions and replies on **2026-10-16**, examining 15 repositories and two gists against Maki **v0.6.3** and a recorded `main` revision. This was source and documentation review, not a runtime test of every project. A follow-up on **2026-11-08** reviewed the 10 repositories in the maki.sh plugin catalog against Maki **v0.7.1**. [Review notes](docs/curation.md) record the evidence, known limits, and projects held back.
