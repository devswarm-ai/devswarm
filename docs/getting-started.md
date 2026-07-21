# Getting Started with DevSwarm

DevSwarm is a desktop app for running multiple AI coding assistants in parallel, each isolated on its own Git branch. This guide covers installation and your first workspace.

## Requirements

- **macOS or Windows** (Windows includes WSL repository support)
- **Git** available in your `PATH`
- **At least one CLI-based AI assistant** installed — DevSwarm detects them automatically. See [Supported AI Assistants](./supported-ai-assistants.md).

## Install

1. Download the installer from **[devswarm.ai/download](https://devswarm.ai/download)**.
2. Run the installer for your operating system.
3. Launch DevSwarm and sign in with **Google or GitHub**.

After you sign in, DevSwarm opens the home page. If you have no repositories yet, a welcome screen walks you through adding your first one.

## Add a repository

Add a repository by importing one from your local filesystem, cloning from a remote URL, cloning from GitHub via OAuth, or creating a new one. Set the **Default Branch** — DevSwarm uses it as the source branch when it creates workspaces.

> **Tip:** Start from a clean state (everything committed) on the branch you set as default.

## Create your first workspace

A **workspace** is an isolated Git worktree paired with an AI assistant terminal and a code editor. When you create one, DevSwarm:

1. Creates a new branch and worktree from the source branch.
2. Starts your chosen AI assistant's CLI in that worktree.
3. Opens **Build Mode** with an active AI terminal session.

You can also create workspaces directly from a **GitHub pull request** or **Jira issue** — DevSwarm hands the PR or issue context to the assistant automatically.

## Build and review

- **Build Mode** (`Cmd+1` / `Ctrl+1`) — a code editor alongside tabbed AI and shell terminals, with file-explorer and Git panels.
- **Review Mode** (`Cmd+2` / `Ctrl+2`) — a diff viewer showing your workspace branch against its source branch, with syntax highlighting.
- Open the workspace in an external editor (Cursor, JetBrains, and others) with `Cmd+5` / `Ctrl+5`.

## Run several at once

Create more workspaces to run assistants in parallel — a refactor in one, tests in another, docs in a third. Each has its own branch, filesystem, and [port assignments](./how-it-works.md#port-variables), so nothing collides.

## Next steps

- [How DevSwarm Works](./how-it-works.md)
- [Supported AI Assistants](./supported-ai-assistants.md)
- [FAQ](./faq.md)

Questions or bugs? [Open an issue](https://github.com/devswarm-ai/devswarm/issues/new/choose) or email support@devswarm.ai.
