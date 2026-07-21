# DevSwarm — Public Repository Guide

This file is public. Keep everything here matter-of-fact and safe for anyone to read. Do not add internal notes, credentials, roadmaps, private URLs, or confidential product details.

## What this repository is

`devswarm-ai/devswarm` is the **public landing page and issue tracker** for DevSwarm. The DevSwarm application itself is a separate, proprietary product and does not live here. This repo contains:

- Marketing/overview docs: `README.md`, `SECURITY.md`, `CONTRIBUTING.md`, `CODE_OF_CONDUCT.md`, `LICENSE`
- GitHub issue templates: `.github/ISSUE_TEMPLATE/` (bug, feature, question)

## What DevSwarm is (public description)

DevSwarm is an AI Development Environment (ADE): a **macOS and Windows** desktop app for running multiple AI coding assistants in parallel. The core unit is a **workspace** — an isolated Git worktree paired with an AI assistant terminal and a code editor, running on its own branch. Users run many workspaces at once and review clean per-branch diffs before merging.

- Supported assistants (auto-detected): Claude Code, Gemini, Amazon Q, OpenAI Codex, GitHub Copilot, Cursor CLI, Atlassian Rovo, Goose, Aider, Amp, and others.
- Integrations: GitHub and Jira via OAuth; create workspaces from PRs or Jira issues.
- Requirements: Git in `PATH` and at least one CLI-based AI assistant.
- Download: https://devswarm.ai/download

## Terminology

Use **"workspace"** in all user-facing text (this is the current product term). Older material sometimes said "builder" — treat the two as the same concept, and prefer "workspace" here.

## Keeping this repo accurate

The product is the source of truth; this repo only mirrors **public-safe** facts about it. When the product changes (especially on a new release), the facts here — supported assistants, platforms, requirements, feature list, current version — should be refreshed to match.

The DevSwarm team maintains this with a sync routine run from the product repo on each release. When updating by hand, only carry over information that is already appropriate for a public audience.

## Issue tracking

People file bugs, feature requests, and questions here via the templates in `.github/ISSUE_TEMPLATE/`. Labels: `type:bug`, `type:feature`, `type:question`, `needs-triage`.

To review what's open:

```shell
gh issue list --repo devswarm-ai/devswarm --state open
```

### Open requests snapshot (updated 2026-07-20)

| # | Title | Type |
|---|-------|------|
| 6 | Image Support | feature |
| 5 | Add Linux support for DevSwarm | feature |
| 4 | Ergonomics around injecting environment variables into the Claude session | feature |
| 3 | Load and use the virtual environment from my original worktree | feature |
| 2 | Notify the user when the editor is out of date with the underlying filesystem | bug/feature |
| 1 | Support OPTION-ARROW keybinding in the prompt dialog | feature |

This table is a convenience snapshot; the live Issues list is authoritative. Refresh it during release sync.
