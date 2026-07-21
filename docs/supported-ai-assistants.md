# Supported AI Assistants

DevSwarm is assistant-agnostic: you **bring your own** CLI-based AI coding assistant, and DevSwarm runs it inside an isolated [workspace](./how-it-works.md). You can even run different assistants side by side — Claude Code on one branch, OpenAI Codex on another — and compare their diffs.

DevSwarm detects installed assistants automatically in the background. You just need at least one of them installed, plus Git in your `PATH`.

## Supported today

| Assistant | Provider |
|-----------|----------|
| **Claude Code** | Anthropic |
| **Gemini** | Google |
| **Amazon Q** | AWS |
| **OpenAI Codex** | OpenAI |
| **GitHub Copilot** | GitHub |
| **Cursor CLI** | Cursor |
| **Atlassian Rovo** | Atlassian |
| **Goose** | Block |
| **Aider** | Open-source |
| **Amp** | Sourcegraph |
| **Mistral Vibe** | Mistral |
| **Qwen Code** | Alibaba |
| **Auggie** | Augment Code |
| **Open Code** | SST |
| **Crush** | Charmbracelet |
| **Cline** | IDE extension |
| **Plandex** | Terminal workflow |
| **Droid** | Factory AI |

Each workspace runs its own AI terminal session, and you can open additional AI or shell terminals as tabs within the same workspace.

## Bring your own credentials

Assistants run through **your own credentials or API keys**, or locally — DevSwarm doesn't proxy your prompts or code through a middleman. See [Security & Privacy](../SECURITY.md).

## Don't see your assistant?

Want DevSwarm to support another CLI assistant? [Open a feature request](https://github.com/devswarm-ai/devswarm/issues/new?template=feature.yml) — the list grows based on what the community asks for.
