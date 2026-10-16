# Curation review

## Scope and method

Reviewed on **2026-10-16**. The initial pass read all **14 discussions** in [Maki's public forum](https://github.com/tontinton/maki/discussions), including all comments and replies returned by GitHub. Pagination was checked; no further pages remained. The main sources of project announcements were the [plugin showcase](https://github.com/tontinton/maki/discussions/452) and [custom providers](https://github.com/tontinton/maki/discussions/862). The [formatter discussion](https://github.com/tontinton/maki/discussions/1082) provided extra context for the formatter gist.

The pass examined **15 repositories and two gists**. It checked public source, README instructions, directory layouts, commit history, declared dependencies, licenses where present, and available tests or CI. Related projects mentioned only as inspiration, such as Pi extensions, were not treated as Maki plugins. No public Web UI project was linked in the Web UI discussions.

API references were [Maki v0.6.3](https://github.com/tontinton/maki/tree/v0.6.3) and [main at 8bc8e4c](https://github.com/tontinton/maki/tree/8bc8e4ccf9ccae5c3149f01f6474621096a46834). The projects were not installed or run as part of this curation review. Existing tests and CI indicate author practice; they do not prove compatibility with every current Maki build. Dates below refer to the default branch's latest commit, not GitHub's general repository update timestamp.

The README follows awesome-neovim's contents and category structure, with `author/project` entries and short descriptions. The reference was [awesome-neovim at 65a00c2](https://github.com/rockerBOO/awesome-neovim/tree/65a00c2853a74c3196f797050c3252d4089e5da4). Descriptions and contribution guidance were written for this curation. The standard CC0 license text was taken from that revision's `LICENSE`.

## Repository evidence

“Included” means selected for discovery with the stated limits. It does not mean the project passed a runtime compatibility test. Small, new projects are identified as new; stable templates do not need frequent commits to be useful.

| Repository | Reviewed commit | Commit date | Selection and evidence |
| --- | --- | --- | --- |
| [laudney/maki-essential-plugins](https://github.com/laudney/maki-essential-plugins) | [`59d9b79`](https://github.com/laudney/maki-essential-plugins/commit/59d9b79c0a891da55d5a950599c895ef5e48bc57) | 2026-10-16 | **Included.** Goals, monitor, and provider switching; repeated development and real-host tests. |
| [bzzimmy/maki-parallel](https://github.com/bzzimmy/maki-parallel) | [`cb11d39`](https://github.com/bzzimmy/maki-parallel/commit/cb11d3998ccee2012c2fea3f92ae6490144f970e) | 2026-09-27 | **Included.** Package layout, documented install, real-host tests, and CI; September API fixes. |
| [basvk/maki-browser-plugin](https://github.com/basvk/maki-browser-plugin) | [`3c0b3ef`](https://github.com/basvk/maki-browser-plugin/commit/3c0b3efbe4df5dfa5439acfb70bdeac2ba3aea3e) | 2026-09-29 | **Held back.** Useful browser tools and September process fixes, but the documented custom configuration conflicts with current Maki guidance; no verified corrected setup. |
| [g4bwy/maki-plugins](https://github.com/g4bwy/maki-plugins) | [`a9eeaf1`](https://github.com/g4bwy/maki-plugins/commit/a9eeaf1772e6641d41c3f5b65399a6324ba1aec9) | 2026-10-04 | **Websearch and token-metrics selected.** September API updates, detailed setup, and distinct self-hosted search and observability uses. Other modules need more evidence; see below. |
| [sdroege/maki-plugins](https://github.com/sdroege/maki-plugins) | [`4a5132c`](https://github.com/sdroege/maki-plugins/commit/4a5132ce1105a1cd7573ed201e451804f54b7b71) | 2026-10-15 | **Held back.** Active development through October 15 and notes/history test scripts, but placeholder package URLs and no confirmed complete installation path for this monorepo; history also needs a missing API. |
| [zipadoodlez/maki-session-index](https://github.com/zipadoodlez/maki-session-index) | [`3e702ac`](https://github.com/zipadoodlez/maki-session-index/commit/3e702acf7ea9f2b537e3dacc1374dfa23df18828) | 2026-10-13 | **Held back.** Initial implementation and license commits on October 13; author reports limited practical use. More use or runtime evidence is needed before recommendation. |
| [xqqmdy/maki-herdr-pane-title-sync](https://github.com/xqqmdy/maki-herdr-pane-title-sync) | [`494f52e`](https://github.com/xqqmdy/maki-herdr-pane-title-sync/commit/494f52e6e5d5a6bb779a7954821a983398bdf2b5) | 2026-10-03 | **Held back.** One initial commit and a narrow herdr integration; no sustained use or maintenance evidence yet. No license identified. |
| [zipadoodlez/safe-ish-yolo](https://github.com/zipadoodlez/safe-ish-yolo) | [`cbc56a1`](https://github.com/zipadoodlez/safe-ish-yolo/commit/cbc56a1dab978e79e255012bbb4b56b82c582a2e) | 2026-10-10 | **Held back.** Two October 10 commits; documented bypass limits, but insufficient validation evidence for a command guard recommendation. |
| [lu-zero/maki-lua-plugin-template](https://github.com/lu-zero/maki-lua-plugin-template) | [`7bd0a9a`](https://github.com/lu-zero/maki-lua-plugin-template/commit/7bd0a9a8dbe03d53bfb7c51c1933e143f4059e4f) | 2026-08-29 | **Included as a template.** Generation checks and real-host integration-test scaffold; not an end-user package. |
| [g4bwy/maki-goal](https://github.com/g4bwy/maki-goal) | [`cf145bc`](https://github.com/g4bwy/maki-goal/commit/cf145bc70eb74d086f9339d8fcb147bb064fb5fb) | 2026-07-08 | **Held back.** Two July commits; no later compatibility work found. The maintained essential package already covers goals. |
| [Asaf51/maki-review](https://github.com/Asaf51/maki-review) | [`4a38baa`](https://github.com/Asaf51/maki-review/commit/4a38baa1f62c85d20d73e7dfd984009643873c57) | 2026-07-19 | **Held back.** API and key-handling repair PR remains unmerged; no license identified on the default branch. |
| [bzzimmy/maki-claude](https://github.com/bzzimmy/maki-claude) | [`ff39e69`](https://github.com/bzzimmy/maki-claude/commit/ff39e696cd5bfbb1a8538813bde299eb9f6756e3) | 2026-10-03 | **Held back.** Migrated to Lua providers in October and has tests, but subscription OAuth differs from upstream Anthropic support policy. |
| [bzzimmy/maki-antigravity](https://github.com/bzzimmy/maki-antigravity) | [`e69a57f`](https://github.com/bzzimmy/maki-antigravity/commit/e69a57f65730ff3d1e4bbd79a5dc1cbc85434845) | 2026-09-14 | **Held back.** Installation still depends on the legacy executable-provider interface; no current Lua-provider migration found. |
| [arxdeus/maki-claude-oauth](https://github.com/arxdeus/maki-claude-oauth) | [`b1a54e8`](https://github.com/arxdeus/maki-claude-oauth/commit/b1a54e89ca0d02d757b750a7bbd82304772f38d3) | 2026-08-07 | **Held back.** Legacy executable provider; also differs from upstream Anthropic support policy. |
| [arxdeus/maki-openai-oauth](https://github.com/arxdeus/maki-openai-oauth) | [`42731a8`](https://github.com/arxdeus/maki-openai-oauth/commit/42731a8f00ee43250ec988364a07b66485395724) | 2026-09-05 | **Held back.** Legacy executable provider; current Maki already has built-in OpenAI OAuth. |

## Gist evidence

| Resource | Reviewed revision | Commit date | Selection and evidence |
| --- | --- | --- | --- |
| [jenggo/opsx.lua](https://gist.github.com/jenggo/6ae330b67f252dfa143a512638e6eec6) | [`85554d1`](https://gist.github.com/jenggo/6ae330b67f252dfa143a512638e6eec6/85554d164a06ebaca78103f6cbc829f047c45414) | 2026-10-13 | Held back. Useful OpenSpec integration and three revisions, but no installation guide or separate validation evidence. No license identified. |
| [Crandel/formatter.lua](https://gist.github.com/Crandel/8a5fd9c0505c9d3622494b2ee7c168fc) | [`c1cb85b`](https://gist.github.com/Crandel/8a5fd9c0505c9d3622494b2ee7c168fc/c1cb85b68f55dce3af982536d589988604e8893a) | 2026-09-26 | Held back. Formatter hooks with one published revision, but no installation guide or separate validation evidence. No license identified. |

## Selection decisions

Only five entries passed the initial selection. The main README is the recommendation list; the broader evidence table is a research record.

- **Essential plugins:** User-confirmed provider switching, a documented managed install, maintained goals and monitor features, and real-host tests provide a practical starting point. Test presence is not a claim that all current CI targets pass.
- **Parallel:** A packaged search integration with complete setup and real-host integration tests offers a clear hosted-search option.
- **SearXNG:** A maintained, documented alternative for users who run their own search service. Its missing environment permission is a small, explicit setup correction, stated in the main README.
- **Token metrics:** A distinct local-inference observability tool with detailed setup and a fake-host logic harness. Its metrics are server-wide, and the harness includes an author-local file path; it is not portable runtime proof.
- **Lua template:** A documented scaffold with generated-project checks and real-host test examples supports plugin authors. It is not an end-user plugin.

The remaining projects may be useful, but their current evidence is not enough for this curation's recommendation. Fixing a documented issue or providing credible use evidence can change that decision. New projects do not need an arbitrary age or star count to qualify.

## Installation and compatibility notes

### Package installation

[Tony's review](https://github.com/tontinton/maki/pull/1268#pullrequestreview-5548304143) asks authors to advertise `maki.pack.add` installation. It does not say every existing project has a package layout. The essential, Parallel, session-index, and herdr projects document managed installation and have package entry points.

The g4bwy collection, browser module, and snippets need manual installation. The sdroege collection contains separate package directories, but its example `maki.pack.add` URLs contain `<owner>` placeholders for separate repositories. Do not copy those URLs or treat the collection root as a ready-to-load package. Follow the relevant directory's manual layout and Maki's [package API](https://maki.sh/docs/lua-api/#maki-pack-add).

### SearXNG permissions

The selected websearch module reads `SEARXNG_URL` through `maki.uv.os_getenv`, which requires the `env` permission. Its README's install example grants only `net`. Add `env = true` alongside `net = true` in the config directory's manifest. The main entry states this correction explicitly. See the [reviewed source](https://github.com/g4bwy/maki-plugins/blob/a9eeaf1772e6641d41c3f5b65399a6324ba1aec9/websearch/init.lua) and [environment API](https://maki.sh/docs/lua-api/#maki-uv-os_getenv).

### Browser configuration

The browser README advertises settings under `plugins.maki-browser-plugin`. The current [Maki plugin guide](https://maki.sh/docs/plugins/) says custom `plugins.<name>` settings are rejected for third-party plugins. The browser source also calls `register_options`. Its documented custom configuration is therefore not a verified setup for current Maki. A verified setup or corrected installation guide is needed before recommendation.

### Session titles and permissions

The retitle module opens a model session with `maki.agent.session`. Its README only mentions `fs_read`. Current `main` also gates model sessions with the `agent` permission. Check the permission manifest when using it on that build. The README's Maki version floor must not be read as proof that all later API changes have been covered.

### Metrics are server-wide

The token-metrics module reads vLLM Prometheus counters. Its throughput values include other clients of the same server; they are not the focused Maki request's tokens per second or time to first token. The [status-bar discussion](https://github.com/tontinton/maki/discussions/1137) explains the distinction between server metrics and Maki request timing.

### Command guards and snippets

The safe-ish-yolo author explicitly documents that scripts, interpreters, unknown wrappers, and non-bash tools can bypass the guard. These limits and the absence of separate validation evidence keep it out of the main list.

The formatter and OpenSpec gists are source snippets with comments, not packaged projects with full installation guides. File operations, process execution, and session actions need the relevant grants on the Maki build in use. They remain in this review file until installation and validation evidence support a recommendation.

### Provider metadata

The GreenPT README says EUR rates are stored in Maki's dollar fields. Inference Cooperative rates represent the cooperative's upstream spend, not the user's bill. Strata's curated model row names the author's local model; users must adjust it for their own server. None of those metadata choices was independently validated against a live provider for this review.

## Projects held back

### Session modules and early integrations

Replay has a conversion test and a useful export format, but its README gives usage without a complete installation guide for its two Lua modules. Retitle needs updated agent permission instructions, and changes saved session titles through model calls; a current runtime check would support recommending it. The herdr title integration and session-index are new, and the session-index author explicitly reports little practical use. They need more use evidence.

The sdroege collection is actively maintained and includes useful session notes and provider integrations. Its package URLs are placeholders, while the per-directory manual instructions have not been confirmed against a stock Maki package layout in this review. A working, documented path for each selected directory would address that gap. These projects remain discoverable here without presenting an uncertain setup as a recommendation.

### Custom transcript APIs

[g4bwy's table-of-contents module](https://github.com/g4bwy/maki-plugins/tree/a9eeaf1772e6641d41c3f5b65399a6324ba1aec9/toc) explicitly requires `maki.ui.transcript_outline()`, `maki.ui.scroll_to_block()`, and window click events unavailable in stock Maki. Its README warns that the pane cannot jump without them.

[sdroege's history module](https://github.com/sdroege/maki-plugins/tree/4a5132ce1105a1cd7573ed201e451804f54b7b71/history) reads `maki.session.transcript()`. That API is not exported in the reviewed [v0.6.3 session module](https://github.com/tontinton/maki/blob/v0.6.3/maki-lua/src/api/session.rs) or [main session module](https://github.com/tontinton/maki/blob/8bc8e4ccf9ccae5c3149f01f6474621096a46834/maki-lua/src/api/session.rs). Its active development does not remove this compatibility gap.

These can be reconsidered when their host API requirements are released or a supported fork and installation path are documented.

### Review UI and older goal implementation

The review UI has a useful design, but its [API and key-handling repair](https://github.com/Asaf51/maki-review/pull/3) was still open at review time. Its default branch had no commits after July 19. The older `g4bwy/maki-goal` had no commits after July 8. Neither had enough current compatibility evidence for the initial list. Age alone was not the selection test.

### Executable provider scripts

[Maki's migration guide](https://maki.sh/docs/providers/#migrating-from-provider-scripts) says it no longer runs executables from the config `providers/` directory. The reviewed Antigravity and arxdeus providers still rely on that interface. Their old install instructions are not a current-provider recommendation. Maki also has built-in OpenAI OAuth, so an older OpenAI login helper needs a clear additional use case before inclusion.

### Claude subscription login

`bzzimmy/maki-claude` has migrated to the Lua provider API and includes host integration tests. It is not excluded as an abandoned or script-only project. However, the [upstream Maki README](https://github.com/tontinton/maki/blob/8bc8e4ccf9ccae5c3149f01f6474621096a46834/README.md#supported-providers) explicitly supports Anthropic API-key authentication and warns against OAuth. This curation does not recommend third-party subscription login as an upstream-supported approach. The older arxdeus Claude helper has this concern as well as the retired script interface.

## Licenses and future reviews

No license was identified in the reviewed roots of `g4bwy/maki-plugins`, `sdroege/maki-plugins`, or `xqqmdy/maki-herdr-pane-title-sync`, or in the two gists. This review links to those projects; it does not copy or relicense their code. Other reviewed licenses are available in the linked repositories.

These observations are a dated snapshot, not continuous monitoring. Update the entry and this record when an author fixes an installation path, names a new minimum Maki version, releases missing APIs, or supplies new maintenance and runtime evidence. Apply the same criteria to the maintainer's own projects.

## Curation process

The [Awesome manifesto](https://github.com/sindresorhus/awesome/blob/main/awesome.md) asks for recommendations rather than an exhaustive index. That is the reason for the smaller main list and this separate research record. Formatting and contribution guidance were checked against the [Awesome submission checklist](https://github.com/sindresorhus/awesome/blob/main/pull_request_template.md).

This curation is directed by [laudney](https://github.com/laudney). Research, initial drafting, and documentation checks used AI assistance.
