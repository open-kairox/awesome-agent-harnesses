# Comparisons

> Cross-harness analyses to help you pick the right tool for your use case.

## Feature Comparison Matrix

| Feature | Codex CLI | Claude Code | Hermes Agent | OpenClaw |
|---------|-----------|-------------|--------------|----------|
| **License** | Apache 2.0 | Proprietary | MIT | MIT |
| **Language** | Rust + TypeScript | TypeScript (Bun) | Python | TypeScript (Node.js) |
| **Install** | `npm i -g @openai/codex` | `npm i -g @anthropic-ai/claude-code` | `pip install hermes-agent` | `npm i -g openclaw` |
| **Self-hosted** | No (cloud agent) | No (cloud API) | Yes | Yes |
| **Multi-model** | OpenAI only | Anthropic only | 200+ models (OpenRouter, Ollama, etc.) | Any OpenAI-compatible API |
| **Multi-agent** | Subagents | Subagents | Kanban + subagents | Full orchestration fleet |
| **Messaging channels** | CLI, Web, Desktop, IDE | CLI, IDE, Desktop, Browser | Telegram, Discord, Slack, WhatsApp, Signal, CLI | Telegram, Discord, WhatsApp, Signal, Slack, IRC, more |
| **Skills/Plugins** | MCP + marketplace | Skills + hooks | Skills + plugins | Skills + plugins (13K+ in ClawHub) |
| **Memory** | Session-based | CLAUDE.md + hooks | Persistent (Honcho/FTS5) | MEMORY.md + memory/*.md |
| **Scheduling** | No (on-demand) | No (on-demand) | Cron built-in | Cron built-in |
| **Cost model** | ChatGPT subscription or API | API key or Max subscription | BYO API key (your models) | BYO API key (your models) |

## When to Use Which

### Use Codex CLI if:
- You're already in the OpenAI ecosystem (ChatGPT Plus/Pro subscription)
- You want a polished, zero-config coding agent
- You need cloud sandboxing (code runs in OpenAI's environment)
- You want GitHub integration out of the box

### Use Claude Code if:
- You want the strongest code reasoning (SOTA on coding benchmarks)
- You prefer terminal-first with optional IDE integration
- You need deep codebase understanding across large repos
- You value Anthropic's safety-focused design (explicit permissions, human oversight)

### Use Hermes Agent if:
- You want model flexibility (200+ providers, no vendor lock-in)
- You need persistent memory that improves over time
- You want multi-platform messaging (Telegram, Discord, etc.)
- You're building a personal agent that runs 24/7 on your server
- You value open-source (MIT license, fully self-hosted)

### Use OpenClaw if:
- You need multi-agent orchestration (spawn fleets, coordinate parallel work)
- You want the largest skills ecosystem (13K+ skills in ClawHub)
- You need channel bindings to Telegram/Discord/WhatsApp/Signal
- You're running a team or organization with multiple agents
- You want scheduling, memory, and autonomous operation
- You value open-source with active community (145K+ GitHub stars)

## Recommended Reading

- [**Hermes Agent vs. Claude Code vs. OpenClaw — MindStudio**](https://www.mindstudio.ai/blog/hermes-agent-vs-claude-code-vs-openclaw-which-self-improving-ai-agent-right-for-workflow) — Use-case-driven: "Claude Code is your desk agent. Hermes and OpenClaw handle scheduled tasks on the go."
- [**Best AI Agents in 2026 — RemoteOpenClaw**](https://www.remoteopenclaw.com/blog/best-ai-agents-2026) — Separates "operator runtimes" (OpenClaw, Hermes) from "coding-agent surfaces" (Claude Code, Codex).
- [**The Race to Build a Personal AI Agent — Creator Economy**](https://creatoreconomy.so/p/the-race-to-build-a-personal-ai-agent-openclaw-hermes-claude-codex-gemini) — Honest production comparison from someone who ran all four.
- [**The Anatomy of an Agent — Medium**](https://medium.com/design-bootcamp/the-anatomy-of-an-agent-what-lives-inside-claude-code-openclaw-and-hermes-agent-41cc467f42a6) — Universal framework mapping all three agents' internal anatomy.
- [**Hermes + Codex + Claude + OpenCode + OpenClaw — YouTube**](https://www.youtube.com/watch?v=wM7SvPT31G8) — AionUi demo showing multi-harness cowork setup.
- [**/goal in Claude Code, Codex, and Hermes Agent — TheUnwindAI**](https://www.theunwindai.com/p/goal-in-claude-code-codex-and-hermes-agent) — Compares the /goal command across harnesses with MCP server integration.
