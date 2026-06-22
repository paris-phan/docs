# Documentation project instructions

## About this project

- This is the **engineering knowledge base for Paris Phan**, built on [Mintlify](https://mintlify.com).
- It documents three ventures (**GreekCore**, **Relic**, **Mavri Studio**), a set of research/hackathon **labs**, and the agent-first **engineering** workflow behind them.
- Pages are MDX files with YAML frontmatter; configuration lives in `docs.json`.
- Run `mint dev` to preview locally and `mint broken-links` to check links.

## Structure

The navigation in `docs.json` has four tabs:

- **Overview** — the hub (`index`), the [ecosystem](overview/ecosystem.mdx) map, and the [repository directory](overview/repositories.mdx).
- **Ventures** — `ventures/<name>/index.mdx` (product overview) + `architecture.mdx` (deep dive) for GreekCore, Relic, and Mavri.
- **Labs** — the Pelagic AI deep dive and a project index.
- **Engineering** — workstation, Claude Code config, conventions, and workspace orchestration.

## Terminology

- **Venture** = a product (GreekCore, Relic, Mavri Studio). **Lab** = a research or hackathon build.
- Use **Brand Kit** (Mavri), **skill** (Relic), **chapter** and **tenant** (GreekCore) as those products do.
- Refer to repos by `owner/name` (e.g. `buildrelic/relic-core`).

## Style preferences

- Use active voice and second person ("you").
- Keep sentences concise — one idea per sentence.
- Use sentence case for headings.
- Bold for UI elements: Click **Settings**.
- Code formatting for file names, commands, paths, and code references.
- Reference source files as repo-relative paths in `code` (e.g. `api/packages/db/src/context.ts`), not local `file://` links.

## Content boundaries

- Content is sourced from the project dossiers and GitHub organization listings. Do not invent features, metrics, or file paths that aren't in those sources.
- Mark repository visibility (public/private) accurately; most venture repos are private.
- When a fact is referenced only in a dossier and not verifiable in a public repo, present it as such rather than asserting it as confirmed.
