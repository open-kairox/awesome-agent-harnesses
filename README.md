# Awesome Agent Harnesses [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated, periodically-updated list of AI Agent harness CLIs — tools that give autonomous agents terminal access, file system control, and multi-step execution capabilities.

## Contents

- [What is an Agent Harness?](#what-is-an-agent-harness)
- [Harnesses](#harnesses)
  - [OpenAI Codex CLI](#openai-codex-cli)
  - [Claude Code](#claude-code)
  - [Hermes Agent](#hermes-agent)
  - [OpenClaw](#openclaw)
- [Comparisons](#comparisons)
- [Community & Discussion](#community--discussion)
- [Contributing](#contributing)
- [License](#license)

## What is an Agent Harness?

An **agent harness** is a CLI tool that wraps an LLM with terminal access, file system control, and multi-step execution capabilities. Unlike chat interfaces or IDE extensions, harnesses give agents autonomous control over a development environment — reading code, running commands, editing files, and iterating until tasks are complete.

Key characteristics:
- **Terminal-native**: Runs in the shell, not in a browser or IDE sidebar
- **Autonomous execution**: Agent decides which tools to use and in what order
- **File system access**: Read, write, and edit project files directly
- **Command execution**: Run shell commands, build tools, tests
- **Multi-step reasoning**: Plan → execute → verify → iterate

---

## Harnesses

### OpenAI Codex CLI

*OpenAI's official coding agent. Runs locally in your terminal, powered by GPT-5.5-Codex. Cloud sandbox, GitHub integration, subagents, and MCP support.*

**Links:** [GitHub](https://github.com/openai/codex) · [Docs](https://developers.openai.com/codex/cli) · [Changelog](https://developers.openai.com/codex/changelog) · [npm](https://www.npmjs.com/package/@openai/codex)

**Quick start:**
```bash
npm i -g @openai/codex
# or
brew install --cask codex
```

**Resources:**

- [**Codex CLI Complete Guide (2026)**](https://www.shareuhack.com/en/posts/openai-codex-cli-agent-guide-2026) — Covers installation, approval modes, Rust performance benchmarks, workflow splitting with Claude Code, and MCP integration.
- [**OpenAI Codex Review 2026 — Updated from Daily Use**](https://zackproser.com/blog/openai-codex-review-2026) — Honest longitudinal review tracking Codex from "promising but rough" to production-capable.
- [**How to Use OpenAI Codex: Complete 2026 Guide**](https://tosea.ai/blog/openai-codex-complete-guide-2026) — Practical walkthrough across CLI, IDE, ChatGPT, and computer-use surfaces. Used by 4M developers weekly.
- [**Codex Workflows and Best Practices**](https://smart-webtech.com/blog/openai-codex-workflows-and-best-practices/) — Session management, context degradation recovery, and forking strategies for degraded threads.
- [**Use Codex with the Agents SDK**](https://developers.openai.com/codex/guides/agents-sdk) — Turn Codex CLI into an MCP server callable from the Agents SDK with `codex()` and `codex-reply()` tools.
- [**Introducing Codex — OpenAI Blog**](https://openai.com/index/introducing-codex/) — Original launch announcement. Cloud-based software engineering agent with sandboxed execution and GitHub integration.
- [**Introducing the Codex App**](https://openai.com/index/introducing-the-codex-app/) — Desktop app evolution, covering the full software development lifecycle from design through shipping.

📄 [Full Codex data →](data/codex.md)

---

### Claude Code

*Anthropic's agentic coding tool. Terminal-first with IDE, desktop, and browser surfaces. SOTA code reasoning, deep codebase understanding, explicit human oversight.*

**Links:** [GitHub](https://github.com/anthropics/claude-code) · [Docs](https://code.claude.com/docs/en/overview) · [npm](https://www.npmjs.com/package/@anthropic-ai/claude-code) · [Product](https://www.anthropic.com/product/claude-code)

**Quick start:**
```bash
npm install -g @anthropic-ai/claude-code
claude
```

**Resources:**

- [**50 Claude Code Tips and Best Practices — Builder.io**](https://www.builder.io/blog/claude-code-tips-best-practices) — Covers Plan Mode, CLAUDE.md, hooks, subagents, worktrees, and keyboard shortcuts.
- [**Claude Code Best Practices: 12 Patterns — Level Up Coding**](https://levelup.gitconnected.com/claude-code-best-practices-12-patterns-agentic-engineers-use-65264e3eb919) — 69 actionable tips across 11 categories with input from Boris Cherny (Claude Code's creator at Anthropic).
- [**Claude Code Tips I Wish I'd Had From Day One — Marmelab**](https://marmelab.com/blog/2026/04/24/claude-code-tips-i-wish-id-had-from-day-one.html) — Practical tips on superpowers skills, TDD with subagents, and real project workflow patterns.
- [**Claude Code Tutorial for Beginners (2026)**](https://codewithmukesh.com/blog/claude-code-for-beginners/) — Learn from scratch in 15 minutes. Installation, CLAUDE.md setup, Plan Mode, and comparison with Copilot/Cursor.
- [**Inside Claude Code: A Deep Dive — Medium**](https://medium.com/@dingzhanjun/inside-claude-code-a-deep-dive-into-anthropics-agentic-cli-assistant-a4bedf3e6f08) — Technical breakdown: Bun + CommanderJS + React Ink rendering as ANSI escape codes.
- [**Claude Code Best Practices — DataCamp**](https://www.datacamp.com/tutorial/claude-code-best-practices) — Plan mode, CLAUDE.md files, TDD, and maximizing context window usage. 14 min read.
- [**Claude Code Best Practice (Community Repo)**](https://github.com/shanraisshan/claude-code-best-practice) — "From vibe coding to agentic engineering." Community-sourced tips from Claude team and users.

📄 [Full Claude Code data →](data/claude-code.md)

---

### Hermes Agent

*Nous Research's open-source agent. Persistent memory, 200+ model support, multi-platform messaging, skills system, and Kanban-based multi-agent coordination. MIT licensed.*

**Links:** [GitHub](https://github.com/nousresearch/hermes-agent) · [Docs](https://hermes-agent.nousresearch.com/docs/) · [Quickstart](https://hermes-agent.nousresearch.com/docs/getting-started/quickstart) · [Product](https://hermes-agent.nousresearch.com/)

**Quick start:**
```bash
pip install hermes-agent
hermes postinstall  # optional: installs Node.js, browser, ripgrep, ffmpeg
```

**Resources:**

- [**Hermes Agent v0.13 Reference**](https://blakecrosley.com/guides/hermes) — Covers tenacity, multi-agent Kanban, /goal command, and pluggable providers. Cross-checked against official docs and release notes.
- [**Hermes Agent v0.9 Review (April 2026)**](https://www.heyuan110.com/posts/ai/2026-04-14-hermes-agent-guide/) — In-depth review: MIT license, no vendor lock-in, data locality in `~/.hermes/`, and the Harness Engineering context.
- [**awesome-hermes-agent — GitHub**](https://github.com/0xNyk/awesome-hermes-agent) — Community-curated list of skills, tools, and integrations. Maturity-tagged. Covers wondelai/skills, hermes-workspace, and mission-control.
- [**Working with Skills — Official Guide**](https://hermes-agent.nousresearch.com/docs/guides/work-with-skills) — How to install, configure, and use skills. Official optional skills, hub installation, and URL-based installation.
- [**Hermes Agent Deep Dive — DEV Community**](https://dev.to/truongpx396/hermes-agent-deep-dive-build-your-own-guide-1pcc) — End-to-end walkthrough of principles, setup, and building with Hermes.
- [**Hermes Agent — AgentWiki**](https://agentwiki.org/hermes_agent) — Architecture reference covering multi-LLM backends, Codex runtime integration, and hybrid execution pipelines.

📄 [Full Hermes Agent data →](data/hermes-agent.md)

---

### OpenClaw

*Open-source agent orchestration platform. 145K+ GitHub stars. Self-hosted gateway daemon, multi-agent fleets, 13K+ skills in ClawHub, and multi-platform channel bindings. BYO API key.*

**Links:** [GitHub](https://github.com/openclaw/openclaw) · [Docs](https://docs.openclaw.ai) · [Product](https://openclaw.ai) · [ClawHub](https://clawhub.com) · [Discord](https://discord.com/invite/clawd)

**Quick start:**
```bash
npm i -g openclaw
openclaw setup
```

**Resources:**

- [**OpenClaw Multi-Agent Orchestration Advanced Guide**](https://zenvanriel.com/ai-engineer-blog/openclaw-multi-agent-orchestration-guide/) — Run multiple isolated agents in one gateway. Agent workspaces, auth profiles, channel bindings, and production patterns.
- [**How OpenClaw Works — Medium**](https://bibek-poudel.medium.com/how-openclaw-works-understanding-ai-agents-through-a-real-architecture-5d59cc7a4764) — Architectural deep dive: gateway daemon, agent workspaces, tool system, and how it differs from chatbots.
- [**OpenClaw Setup Guide: 26 Tools + 53 Skills Explained**](https://yu-wenhao.com/en/blog/openclaw-tools-skills-tutorial/) — Research-backed guide with risk assessment for every tool and skill. Copy-ready config included.
- [**Best OpenClaw Skills: Top 10 & 5 to Avoid (2026)**](https://www.aimakers.co/blog/openclaw-skills-guide/) — Community-tested rankings from r/openclaw's most upvoted daily-use thread.
- [**Building Custom OpenClaw Skills — DataCamp**](https://www.datacamp.com/tutorial/building-open-claw-skills) — Hands-on tutorial building two custom skills with Python, triggered via Telegram slash commands.
- [**Custom Skills and Plugin Development — Tencent Cloud**](https://www.tencentcloud.com/techpedia/140775) — When to use skills vs plugins, how to build each, and API integration patterns for SaaS services.
- [**OpenClaw + YouWare: No-Code Orchestration**](https://www.youware.com/guide/openclaw-youware-no-code-ai-agent-orchestration) — Democratizes OpenClaw access through AI-powered no-code tooling.

📄 [Full OpenClaw data →](data/openclaw.md)

---

## Comparisons

| Feature | Codex CLI | Claude Code | Hermes Agent | OpenClaw |
|---------|-----------|-------------|--------------|----------|
| **License** | Apache 2.0 | Proprietary | MIT | MIT |
| **Self-hosted** | ☐ Cloud | ☐ Cloud | ✅ Yes | ✅ Yes |
| **Multi-model** | OpenAI only | Anthropic only | 200+ models | Any OpenAI-compatible |
| **Multi-agent** | Subagents | Subagents | Kanban + subagents | Full orchestration fleet |
| **Messaging** | CLI, Web, IDE | CLI, IDE, Browser | Telegram, Discord, Slack, WhatsApp, Signal, CLI | Telegram, Discord, WhatsApp, Signal, Slack, IRC, more |
| **Skills** | MCP + marketplace | Skills + hooks | Skills + plugins | Skills + plugins (13K+ in ClawHub) |
| **Memory** | Session | CLAUDE.md | Persistent (Honcho/FTS5) | MEMORY.md + memory/*.md |
| **Scheduling** | ☐ | ☐ | ✅ Cron | ✅ Cron |

**Recommended comparisons:**
- [Hermes vs. Claude Code vs. OpenClaw — MindStudio](https://www.mindstudio.ai/blog/hermes-agent-vs-claude-code-vs-openclaw-which-self-improving-ai-agent-right-for-workflow)
- [The Race to Build a Personal AI Agent — Creator Economy](https://creatoreconomy.so/p/the-race-to-build-a-personal-ai-agent-openclaw-hermes-claude-codex-gemini)
- [Best AI Agents in 2026 — RemoteOpenClaw](https://www.remoteopenclaw.com/blog/best-ai-agents-2026)
- [The Anatomy of an Agent — Medium](https://medium.com/design-bootcamp/the-anatomy-of-an-agent-what-lives-inside-claude-code-openclaw-and-hermes-agent-41cc467f42a6)

📄 [Full comparisons →](comparisons.md)

---

## Community & Discussion

- [**OpenClaw Discord**](https://discord.com/invite/clawd) — Agent orchestration, skills, and multi-agent workflows
- [**r/hermesagent**](https://www.reddit.com/r/hermesagent/) — Hermes Agent setups, profiles, and integrations
- [**r/ClaudeCode**](https://www.reddit.com/r/ClaudeCode/) — Claude Code workflows and configurations
- [**r/openclaw**](https://www.reddit.com/r/openclaw/) — OpenClaw tips, skills, and community
- [**ClawHub.com**](https://clawhub.com) — Skill registry for OpenClaw (13K+ skills)

## Contributing

Contributions welcome! See [CONTRIBUTING.md](./contributing.md) for guidelines.

## License

[MIT](./LICENSE) © 2025-present Kairox-Agents
