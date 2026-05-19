# OpenClaw

> An open-source, self-hosted agent orchestration platform that transforms LLMs into active agents capable of executing complex tasks across devices and platforms. 145,000+ GitHub stars. Runs a local gateway daemon with multi-agent support, skills, plugins, and channel bindings (Telegram, Discord, WhatsApp, Signal, Slack, and more).

## Official Docs & Repos

- [**OpenClaw — GitHub**](https://github.com/openclaw/openclaw) — The main repo. Open-source agent orchestration platform with gateway daemon, agent workspaces, tools, skills, and multi-platform channel support.
- [**OpenClaw — Official Docs**](https://docs.openclaw.ai) — Comprehensive documentation covering installation, configuration, tools, skills, plugins, multi-agent setup, and channel bindings.
- [**OpenClaw — Product Site**](https://openclaw.ai/) — Landing page showcasing use cases: email management, deck reviews, CLI tool building, Google Ads optimization, and orchestrating Codex workers across Discord.
- [**ClawHub — Skill Registry**](https://docs.openclaw.ai/clawhub) — The official skill registry. 13,000+ skills. Search, install, and publish skills via `openclaw` CLI or the `clawhub` CLI for publishing workflows.
- [**ClawHub — GitHub**](https://github.com/openclaw/clawhub) — The open-source registry code. Vector search, moderation hooks, version management, and a CLI-friendly API.

## Skills & Plugins

- [**Skills — Official Docs**](https://docs.openclaw.ai/tools/skills) — How skills work, how plugins ship skills, and how to configure them in your workspace.
- [**OpenClaw Setup Guide: 26 Tools + 53 Skills Explained**](https://yu-wenhao.com/en/blog/openclaw-tools-skills-tutorial/) — Research-backed guide breaking down all 26 tools and 53 official skills with risk assessment and a copy-ready config.
- [**Best OpenClaw Skills: Top 10 to Install & 5 to Avoid (2026)**](https://www.aimakers.co/blog/openclaw-skills-guide/) — Community-tested rankings based on r/openclaw's most upvoted "what skill do you actually use every day?" thread.
- [**OpenClaw Skills: How to Find, Install, and Build Your Own — DeployHQ**](https://www.deployhq.com/blog/openclaw-skills-guide) — Guide to finding skills in ClawHub registry, installing on your VPS, and building custom skills from scratch.
- [**OpenClaw Skills Guide — LumaDock**](https://lumadock.com/tutorials/openclaw-skills-guide) — When to build your own skills, what to check before installing third-party bundles, and repeatable behavior patterns.
- [**Building Custom OpenClaw Skills: A Hands-On Tutorial — DataCamp**](https://www.datacamp.com/tutorial/building-open-claw-skills) — Step-by-step tutorial building two custom skills with `uv` for Python dependencies, triggered via Telegram slash commands.
- [**Custom Skills and Plugin Development Guide — Tencent Cloud**](https://www.tencentcloud.com/techpedia/140775) — Deep guide to both systems: when to use skills vs plugins, how to build each properly, and API integration patterns.
- [**Custom API Integration with Skills and Plugins — LumaDock**](https://lumadock.com/tutorials/openclaw-custom-api-integration-guide) — Practical guide to integrating SaaS services (GitHub, Stripe, weather APIs, CRMs) through skills and plugins.

## Tutorials & Guides

- [**OpenClaw Multi-Agent Orchestration Advanced Guide — Zen Van Riel**](https://zenvanriel.com/ai-engineer-blog/openclaw-multi-agent-orchestration-guide/) — Learn to run multiple isolated agents in one gateway. Covers agent workspaces, auth profiles, channel bindings, and orchestration patterns.
- [**How OpenClaw Works: Understanding AI Agents Through a Real Architecture — Medium**](https://bibek-poudel.medium.com/how-openclaw-works-understanding-ai-agents-through-a-real-architecture-5d59cc7a4764) — Architectural deep dive explaining the gateway, agent workspaces, tool system, and how it differs from chatbots.
- [**OpenClaw AI Agent Orchestration: Complete Guide — Progressive Robot**](https://www.progressiverobot.com/2026/03/23/openclaw-ai-agent-orchestration-complete-guide-to-build-production-ready-ai-agents/) — Guide to deploying, managing, and scaling AI agents without requiring deep technical expertise.
- [**The Complete Guide to OpenClaw Agent Orchestration — Skywork**](https://skywork.ai/skypage/en/openclaw-agent-orchestration/2049110034606260225) — Covers the self-hosted gateway, orchestration layer, and how it transforms LLMs into active agents.
- [**Multi-Agent Orchestration — LearnOpenClaw**](https://learnopenclaw.org/multiagent.html) — How OpenClaw spawns fleets of sub-agents, coordinates parallel work, merges results, and resolves conflicts automatically.
- [**Mastering OpenClaw Skills — Tencent Cloud**](https://www.tencentcloud.com/techpedia/139672) — Installing and applying OpenClaw skills with the browser operation plugin and application templates.

## Community

- [**OpenClaw Discord**](https://discord.com/invite/clawd) — Official Discord for community discussion, skill recommendations, and announcements.
- [**r/openclaw (Reddit)**](https://www.reddit.com/r/openclaw/) — Community subreddit. Active discussions on setups, skills, and workflows.
- [**ClawHub.com**](https://clawhub.com) — Public skill registry for browsing and discovering community skills.
- [**OpenClaw Wiki**](https://openclaw-wiki.com/wiki.php) — Community-maintained knowledge base covering history, features, and ecosystem.

## Ecosystem & Integrations

- [**OpenClaw Mission Control — GitHub**](https://github.com/abhi1693/openclaw-mission-control) — Centralized operations and governance platform for running OpenClaw across teams and organizations.
- [**OpenClaw + YouWare: No-Code AI Agent Orchestration**](https://www.youware.com/guide/openclaw-youware-no-code-ai-agent-orchestration) — Democratizes OpenClaw access through AI-powered no-code tooling.
- [**OpenClaw GitHub Resources Guide — BoilerplateHub**](https://boilerplatehub.com/blog/openclaw-github) — Guide to navigating the official repo, ClawHub registry, and community resources.

## Videos & Talks

- [**Hermes + Codex + Claude + OpenClaw Agentic CoWork OS — YouTube**](https://www.youtube.com/watch?v=wM7SvPT31G8) — Introduces AionUi, a free local open-source cowork app supporting multiple agent harnesses.

## Cross-Harness Comparisons

- [**The Race to Build a Personal AI Agent — Creator Economy**](https://creatoreconomy.so/p/the-race-to-build-a-personal-ai-agent-openclaw-hermes-claude-codex-gemini) — Opinionated comparison from someone who ran all four in production. Honest about OpenClaw's maintenance trade-offs.
- [**The Anatomy of an Agent — Medium**](https://medium.com/design-bootcamp/the-anatomy-of-an-agent-what-lives-inside-claude-code-openclaw-and-hermes-agent-41cc467f42a6) — Dissects Claude Code, OpenClaw, and Hermes and maps their internal anatomy onto a universal framework.

## Release Notes

- OpenClaw ships frequent releases. Check the [GitHub releases page](https://github.com/openclaw/openclaw/releases) for the latest. Current version: 2026.3.x.
