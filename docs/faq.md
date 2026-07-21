# Frequently Asked Questions

## What is DevSwarm?

DevSwarm is an AI Development Environment (ADE) — a desktop app for running multiple AI coding assistants in parallel, each isolated on its own Git branch. See [How DevSwarm Works](./how-it-works.md).

## What operating systems does DevSwarm support?

DevSwarm runs on **macOS and Windows**. On Windows it also supports repositories in the Windows Subsystem for Linux (WSL). Native Linux support is a [community request](https://github.com/devswarm-ai/devswarm/issues) we're tracking.

## Which AI coding assistants can I use?

Claude Code, Gemini, Amazon Q, OpenAI Codex, GitHub Copilot, Cursor CLI, Goose, Aider, Amp, and more — see the full [Supported AI Assistants](./supported-ai-assistants.md) list. DevSwarm detects installed assistants automatically.

## Can I run more than one assistant at the same time?

Yes — that's the point. Each workspace is an isolated Git worktree on its own branch, so you can run several assistants simultaneously (for example, a refactor, tests, and docs at once) without them colliding.

## Does DevSwarm send my code or prompts to DevSwarm's servers?

No. Your code stays on your machine, and assistants use **your own credentials or run locally**. Sensitive data stored on-device is encrypted at rest using your operating system's built-in encryption. See [SECURITY.md](../SECURITY.md).

## Do I need my own API keys?

You use whatever credentials your chosen assistant requires — your own API keys or account sign-in, or a local model. DevSwarm doesn't proxy your prompts through a middleman.

## How is this different from an AI assistant inside my editor?

Most tools embed a single assistant in your editor. DevSwarm is built the other way around: **parallel and isolated**. You run multiple assistants across branches and review each as a clean diff before merging — coder-in-the-loop, not vibe coding.

## Do I have to give up my editor?

No. DevSwarm has its own Build and Review modes, but you can open any workspace in an external editor (Cursor, JetBrains, and others) with `Cmd+5` / `Ctrl+5`.

## Does it integrate with GitHub and Jira?

Yes — both via OAuth. Clone from GitHub, browse and filter PRs with CI/CD and review status, and create workspaces directly from a pull request or Jira issue.

## How much does DevSwarm cost?

DevSwarm is currently a **free beta**. [Download it](https://devswarm.ai/download) to try it.

## How do I report a bug or request a feature?

Use this repository's **Issues**: [report a bug](https://github.com/devswarm-ai/devswarm/issues/new?template=bug.yml), [request a feature](https://github.com/devswarm-ai/devswarm/issues/new?template=feature.yml), or [ask a question](https://github.com/devswarm-ai/devswarm/issues/new?template=question.yml). For private matters, email support@devswarm.ai.

## Where do I get help?

Visit [devswarm.ai/support](https://devswarm.ai/support) or email support@devswarm.ai.
