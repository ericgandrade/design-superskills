# CLAUDE.md

**design-superskills** — 9 AI skills for UI/UX design, brand, design systems, diagrams, and presentations.

- **npm package**: `design-superskills` (v1.0.1) — `npx design-superskills` — **9 skills**
- **GitHub**: `https://github.com/ericgandrade/design-superskills`

## Skills (9)
ui-ux-pro-max, design, design-system, brand, ui-styling, slides, banner-design, excalidraw-diagram, mermaid-diagram

## Version Management
Use `node scripts/release.js [patch|minor|major]`. Publishing via GitHub Actions on `v*` tag push.

## Language

All content in this repository — code comments, documentation, commit messages, skill files, and AI instructions — must be written in **English**. No Portuguese or any other language.

## graphify

This project has a graphify knowledge graph at graphify-out/.

Rules:
- Before answering architecture or codebase questions, read graphify-out/GRAPH_REPORT.md for god nodes and community structure
- If graphify-out/wiki/index.md exists, navigate it instead of reading raw files
- After modifying code files in this session, run `graphify update .` to keep the graph current (AST-only, no API cost)
- **After any important change, run `/graphify --update` before ending the session.** Important changes include: adding or removing a skill, modifying SKILL.md or README.md of any skill, bumping version, or any structural refactor. Do not skip this step — an outdated graph leads to stale answers in future sessions.
