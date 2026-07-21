# How DevSwarm Works

DevSwarm is an AI Development Environment (ADE) for **parallel AI coding**. Instead of embedding one assistant in your editor, it lets you run many assistants at once — each isolated on its own Git branch — and review their work as clean diffs before you merge.

## Workspaces

The core unit is a **workspace**: an isolated Git worktree paired with an AI assistant terminal and a code editor. Each workspace has:

- Its own **branch**, created from a source branch you choose
- A separate **working directory** (Git worktree) — no shared checkout to trip over
- Independent **build processes**
- Unique **port assignments** so apps don't collide

Because workspaces are isolated, you can run several simultaneously — one per feature, bug fix, or review — without them interfering with each other.

## Two views per workspace

- **Build Mode** (`Cmd+1` / `Ctrl+1`) — the primary interface: a code editor alongside tabbed AI and shell terminal sessions, with collapsible panels for file exploration and Git operations (stage, commit, push, merge/rebase from the source branch).
- **Review Mode** (`Cmd+2` / `Ctrl+2`) — a diff viewer comparing the workspace branch against its source branch with syntax highlighting.

Open a workspace in an external editor (Cursor, JetBrains, and others) with `Cmd+5` / `Ctrl+5`.

## Bring your own assistant

DevSwarm detects installed CLI-based AI assistants automatically and lets each workspace run its own session. You can open additional AI or shell terminals as tabs within the same workspace. See the full list in [Supported AI Assistants](./supported-ai-assistants.md).

## GitHub and Jira

DevSwarm connects to **GitHub and Jira via OAuth**. Clone repositories from GitHub, browse and filter pull requests with their CI/CD and review status, and create workspaces directly from a **PR or Jira issue** — including bulk operations. The assistant receives the PR or issue context automatically.

## Port variables

Each workspace receives unique values for port environment variables like `PORT`, `API_PORT`, or `DATABASE_PORT`. This lets you run the same application across multiple workspaces at the same time without port conflicts.

## Keyboard-first

Workspace switching, terminal management, and Git operations are all keyboard-driven. Press `Ctrl+Alt+I` (Windows) / `Ctrl+Option+I` (macOS) to open the Shortcuts overlay at any time.

## The philosophy: coder-in-the-loop

DevSwarm is built for **coder-in-the-loop** development, not vibe coding. You direct focused assistants, then verify their output through clean, reviewable diffs. We call this **High Velocity Engineering** — moving fast while building right.

## Learn more

- [Getting Started](./getting-started.md)
- [Supported AI Assistants](./supported-ai-assistants.md)
- [FAQ](./faq.md)
