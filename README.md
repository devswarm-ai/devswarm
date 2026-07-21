# DevSwarm — Parallel AI Coding for Your Desktop

**DevSwarm is an AI Development Environment (ADE): a desktop app for running multiple AI coding assistants in parallel, each isolated on its own Git branch.**

Spin up as many **workspaces** as you need. Each one is an isolated Git worktree paired with an AI assistant terminal and a code editor — separate working directory, independent build, its own branch. Point Claude Code at a refactor in one workspace, Codex at tests in another, and a third at docs, all at the same time. When they're done, review clean diffs side by side and merge with confidence.

Built for **coder-in-the-loop**, not vibe coding. Keep the CLI and editor you already use. Move fast without changing how you ship.

We call this **High Velocity Engineering**: the art of moving fast and building right.

## What DevSwarm does

- **Parallel workspaces** — run many AI assistants at once, each in an isolated Git worktree with its own branch, filesystem, and ports.
- **Clean diffs and reviews** — a built-in Review Mode diffs each workspace branch against its source branch with syntax highlighting.
- **Bring your own assistant** — DevSwarm detects installed CLI assistants automatically. Supported today: Claude Code, Gemini, Amazon Q, OpenAI Codex, GitHub Copilot, Cursor CLI, Atlassian Rovo, Goose, Aider, Amp, and more.
- **GitHub & Jira built in** — connect via OAuth, browse and filter PRs, and create workspaces directly from a pull request or Jira issue.
- **Port variables** — each workspace gets unique port assignments so you can run the same app in several workspaces without conflicts.
- **Keyboard-first** — switch workspaces, manage terminals, and drive Git operations without leaving the keyboard.

## Why DevSwarm

Most tools drop AI inside your editor. DevSwarm is built the other way around — parallel, isolated, developer-first. Run multiple assistants, compare branches, and stay in control of your code.

## Documentation

- [Getting Started](./docs/getting-started.md) — install and create your first workspace
- [How DevSwarm Works](./docs/how-it-works.md) — workspaces, review, integrations
- [Supported AI Assistants](./docs/supported-ai-assistants.md) — the full list
- [FAQ](./docs/faq.md) — common questions
- [Changelog](./CHANGELOG.md) — what's new

## Requirements

- **macOS or Windows** (Windows includes WSL repository support)
- **Git** available in your `PATH`
- **At least one CLI-based AI assistant** installed (Claude Code, Gemini, Amazon Q, Codex, and others)

## Get DevSwarm

- **Download the free beta: [devswarm.ai/download](https://devswarm.ai/download)**
- Install, launch, and sign in with Google or GitHub.
- **Star this repo** if you believe in coder-in-the-loop, parallel AI coding.
- Follow along: [GitHub](https://github.com/devswarm-ai/) · [LinkedIn](https://www.linkedin.com/company/devswarm/) · [Twitter / 𝕏](https://x.com/devswarm_ai)

## What this repo is

This is the **public landing page and issue tracker** for DevSwarm. The application itself is a separate, proprietary product. Use **Issues** here to report bugs, request features, or ask questions:

- [Open an issue](https://github.com/devswarm-ai/devswarm/issues/new/choose)
- Contact: support@devswarm.ai

## Security and privacy

Your code stays on your machine, and AI assistants use your own credentials or run locally. See [SECURITY.md](./SECURITY.md). For sensitive reports, email security@devswarm.ai.

## Contributing

We welcome feedback, ideas, and real-world use cases. See [CONTRIBUTING.md](./CONTRIBUTING.md).

## License

© 2025–2026 21st Idea, Inc. (dba DevSwarm). All rights reserved. DevSwarm™ and the DevSwarm logo are trademarks of 21st Idea, Inc. The DevSwarm application is proprietary; see [LICENSE](./LICENSE).
