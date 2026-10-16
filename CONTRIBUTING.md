# Contributing

Help readers find useful Maki projects and understand what they need to run them. Authors are welcome to submit their own work.

## Add or update an entry

Open a pull request with one project or a small related correction. Use the closest existing category and this format:

```markdown
- [author/project](https://github.com/author/project) - Describe the main use. State important requirements or limits.
```

Use the author's GitHub name in the link text. For a repository subdirectory, link directly to that directory. For a gist, use `author/filename.lua`.

Check the following before submission:

- The project solves a clear Maki use case and has public source.
- The link reaches the actual project, not an unrelated fork or a demo.
- Installation instructions work with the stated Maki version. Prefer a tested `maki.pack.add` example and a suitable package layout, as [Maki's maintainer recommends](https://github.com/tontinton/maki/pull/1268#pullrequestreview-5548304143).
- Manual installation, a subdirectory layout, external tools, credentials, and required permissions are stated when relevant. Do not pass a monorepo root to `maki.pack.add` unless it is a working package.
- Required APIs exist in a named Maki release or revision. Mark any dependency on an unreleased build or custom fork.
- The README and source agree on behavior. Avoid unsupported claims about security, compatibility, performance, or provider support.
- Maintenance evidence is available: recent fixes, responses to issues, tests, or a stable implementation with clear support. A recent commit alone does not prove quality; an older commit alone does not prove abandonment.
- New projects are identified as new. State limited testing or known defects that affect a reader's choice.
- The license is identified, or its absence is recorded in the review notes. Linking to a project does not grant permission to copy its code.

Keep descriptions short and factual. Do not add star counts, changing download counts, promotional claims, or tracking links. Do not duplicate an entry across categories without a separate use case.

## Include review evidence

In the pull request, give the project URL, author, use case, Maki version or revision, installation method, and the checks you performed. Link to the author's announcement or relevant issue when available. State clearly whether you ran the project or only reviewed its source.

Update [the review notes](docs/curation.md) when a new entry has a material compatibility limit, changes status, or replaces a project held back there. Keep older review dates attached to their evidence until the entry is checked again.

For documentation changes, check links, section anchors, and the rendered Markdown. No Maki build is required.

## Report a problem

Open an issue or submit a correction when installation fails, an API changes, a project moves, or a description is wrong. Include the Maki version and a source link. Report defects in a listed project to that project's author.
