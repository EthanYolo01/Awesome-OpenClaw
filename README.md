<div align="center">

<img src="ecosystem-map.svg" alt="OpenClaw Ecosystem Map" width="100%"/>

# 🦞 Awesome OpenClaw

**A carefully curated list of awesome OpenClaw resources — not everything, just the best.**

*Skills · Plugins · MCP · Tools · Deployments · Security · Research · Alternatives*

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](CONTRIBUTING.md)
[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg?style=flat-square)](https://creativecommons.org/publicdomain/zero/1.0/)
[![Last Updated](https://img.shields.io/badge/last%20updated-March%202026-blue?style=flat-square)](https://github.com/openclaw/awesome-openclaw/commits/main)
[![Link Check](https://img.shields.io/github/actions/workflow/status/EthanYolo01/Awesome-OpenClaw/link-checker.yml?label=links&style=flat-square)](https://github.com/EthanYolo01/Awesome-OpenClaw/actions)
[![Stars](https://img.shields.io/github/stars/EthanYolo01/Awesome-OpenClaw?style=flat-square)](https://github.com/EthanYolo01/Awesome-OpenClaw/stargazers)
[![Contributors](https://img.shields.io/github/contributors/EthanYolo01/Awesome-OpenClaw?style=flat-square)](https://github.com/EthanYolo01/Awesome-OpenClaw/graphs/contributors)

> **Opinionated curation over exhaustive listing.**
> Every entry was reviewed. Where other lists stop at a URL, we tell you *why* it matters and *when* to use it.

**OpenClaw at a Glance (March 2026):** ⭐ 247K GitHub Stars &nbsp;·&nbsp; 🔱 47.7K Forks &nbsp;·&nbsp; 🧩 13,729 ClawHub Skills &nbsp;·&nbsp; 🌍 10+ Channels

---

🌐 Language / 语言切换：**English** | [中文](README_CN.md)

</div>

---

## 📋 Table of Contents

- [🏁 Start Here — What is OpenClaw?](#-start-here--what-is-openclaw)
- [⏳ Timeline & Milestones](#-timeline--milestones)
- [🏠 Official Resources](#-official-resources)
- [⚡ Getting Started & Installation](#-getting-started--installation)
- [🧠 Core Architecture](#-core-architecture)
- [🤖 LLM Model Selection Guide](#-llm-model-selection-guide)
- [💰 Cost Estimation Guide](#-cost-estimation-guide)
- [🔧 Skills & Plugins](#-skills--plugins)
- [🤖 MCP Integrations](#-mcp-integrations)
- [🖥️ UIs & Companion Apps](#️-uis--companion-apps)
- [🌐 Platform Channels & Messaging](#-platform-channels--messaging)
- [☁️ Deployment & Infrastructure](#️-deployment--infrastructure)
- [🏢 Enterprise Deployment](#-enterprise-deployment)
- [🧠 Memory & Knowledge Systems](#-memory--knowledge-systems)
- [🔒 Security](#-security)
- [🆚 OpenClaw vs Other Agent Frameworks](#-openclaw-vs-other-agent-frameworks)
- [🌍 Ecosystem & Agent Platforms](#-ecosystem--agent-platforms)
- [🛠️ Developer Tooling](#️-developer-tooling)
- [🏗️ Alternative Implementations](#️-alternative-implementations)
- [📖 Tutorials, Blogs & Articles](#-tutorials-blogs--articles)
- [🎥 Videos & Talks](#-videos--talks)
- [📚 Research & Academic Resources](#-research--academic-resources)
- [💼 Use Cases & Showcases](#-use-cases--showcases)
- [❓ FAQ & Troubleshooting](#-faq--troubleshooting)
- [🤝 Community & Support](#-community--support)
- [🗺️ Related Awesome Lists](#️-related-awesome-lists)
- [🤝 Contributing](#-contributing)

---

## 🏁 Start Here — What is OpenClaw?

OpenClaw (formerly **Clawdbot**, briefly **Moltbot**) is an open-source, **local-first autonomous AI agent framework**. You run a persistent process called the **Gateway** on hardware you control — a Mac mini, a VPS, a Raspberry Pi — and it connects to messaging apps you already use. When you send a message, OpenClaw runs an agent turn powered by an LLM, invokes tools or skills, and responds — often taking real actions on your behalf.

**Key design decisions that explain the hype:**

- **Messaging app as UI** — No new app to install. WhatsApp, Telegram, Discord, Slack, iMessage — whatever you already live in becomes your agent interface.
- **Local-first, self-hosted** — Your data stays on your machine. No third-party server sees your context.
- **Skills/Plugins architecture** — Capabilities are tiny markdown-declared plugins. Anyone can write one in under an hour.
- **Persistent memory** — Flat-file Markdown memory (`MEMORY.md`, `SOUL.md`) persists across restarts without a vector database.
- **Model-agnostic** — Works with Claude, GPT-5, Gemini, local Ollama models, and OpenRouter.

---

## ⏳ Timeline & Milestones

Understanding OpenClaw's history explains its current architecture and community dynamics.

```
Nov 2025  ──  Peter Steinberger (@steipete) releases "Clawdbot"
              TypeScript, Claude-only, WhatsApp + Telegram support
              Day 1: 5K stars. Week 1: 30K stars.

Dec 2025  ──  Anthropic trademark dispute → renamed "Moltbot"
              72 hours later renamed again to "OpenClaw"
              Community skill ecosystem begins forming spontaneously
              ClawHub launched as community skill registry

Jan 2026  ──  OpenClaw goes supernova: 68K → 120K stars in 2 weeks
              CVE-2026-25253 disclosed — WebSocket RCE vulnerability
              341 malicious skills discovered on ClawHub
              Alternative implementations start appearing:
              ZeroClaw (Rust), NanoClaw (Python), PicoClaw (Go)

Feb 2026  ──  Steinberger joins OpenAI
              Project transferred to OpenClaw Foundation (independent)
              ClawHub adds VirusTotal scanning for all submitted skills
              NemoClaw (NVIDIA, sandboxed) released
              Moltis (Rust, enterprise-grade) hits 1.0

Mar 2026  ──  247K stars, 47.7K forks
              OpenClaw Foundation announces governance model
              13,729 skills on ClawHub
              v1.9.x stable release series
```

---

## 🏠 Official Resources

| Resource | Description |
|---|---|
| [openclaw/openclaw](https://github.com/openclaw/openclaw) | Main repository — TypeScript monorepo |
| [openclaw/skills](https://github.com/openclaw/skills) | Official skills repository |
| [clawhub.ai](https://clawhub.ai) | Official skills marketplace & registry |
| [OpenClaw Blog](https://openclaw.ai/blog/) | Announcements, security advisories, feature deep-dives |
| [OpenClaw Docs](https://docs.openclaw.ai) | Official documentation |
| [OpenClaw Changelog](https://github.com/openclaw/openclaw/releases) | Release notes and version history |
| [Latest Updates & Roadmap](https://x.com/openclaw) | Official X account — feature previews, release news, community highlights |

**Monorepo package map:**

| Package | Description |
|---|---|
| `packages/core` | Core framework, provider interfaces, base classes |
| `packages/gateway` | WebSocket control plane (port 18789), session management, channel routing |
| `packages/agent` | Agent runtime with RPC mode, tool streaming, block streaming |
| `packages/cli` | CLI for onboarding, gateway control, messaging |
| `packages/sdk` | SDK for building custom tools and plugins |
| `packages/ui` | WebChat interface + Control UI dashboard |

---

## ⚡ Getting Started & Installation

### Quick Install

```bash
# Requires Node.js 20+
npm install -g openclaw

# Interactive onboarding wizard
openclaw onboard

# Or specify your provider directly
openclaw onboard --auth-choice anthropic-api-key
openclaw onboard --auth-choice openai-api-key
openclaw onboard --auth-choice openrouter        # Recommended for cost optimization
```

### Docker (Recommended for Production)

```bash
docker run -d \
  -p 127.0.0.1:18789:18789 \
  -v ~/openclaw-data:/data \
  -e ANTHROPIC_API_KEY=your_key \
  --restart unless-stopped \
  openclaw/openclaw:stable
```

> ⚠️ **Critical:** Bind to `127.0.0.1`, not `0.0.0.0`. See [Security](#-security) for why this matters.

### Release Channels

| Channel | Command | Use Case |
|---|---|---|
| `stable` | `npm i -g openclaw` | All users — recommended |
| `beta` | `npm i -g openclaw@beta` | Early adopters, testing new skills |
| `dev` | `npm i -g openclaw@dev` | Core contributors only — may be broken |

### Install Guides

- [Official Quickstart](https://docs.openclaw.ai/quickstart) — 5-minute path to a working agent
- [Docker Setup Guide](https://docs.openclaw.ai/install/docker) — Recommended for all production deployments
- [Nix/NixOS Setup](https://docs.openclaw.ai/install/nix) — Reproducible, declarative via `nix-openclaw`
- [DigitalOcean 1-Click](https://marketplace.digitalocean.com/apps/openclaw) — Fastest cloud deploy
- [VPS Hosting & Deployment Guide](https://docs.openclaw.ai/vps) — Nginx, SSL, firewall
- [Raspberry Pi Setup](https://www.raspberrypi.com/news/turn-your-raspberry-pi-into-an-ai-agent-with-openclaw/) — Runs on Pi 4 4GB+
- [Mac Mini as Home Server](https://docs.openclaw.ai/zh-CN/install/macos-vm) — Highly recommended homelab
- [Ansible Playbook](https://github.com/openclaw/openclaw-ansible) — Automated secure installation with Tailscale VPN, UFW firewall and Docker isolation

---

## 🧠 Core Architecture

Five concepts unlock the entire ecosystem:

### 1. The Gateway
A WebSocket server (port 18789) that is the single orchestration point. It normalizes heterogeneous messaging protocols — WhatsApp via Baileys, Telegram via grammY, Slack Events API, Discord gateway — into a canonical internal message format. No intelligence lives here. It is a pure traffic controller.

### 2. Skills vs Plugins vs MCP

| | Skills | Plugins | MCP Integrations |
|---|---|---|---|
| **Format** | `SKILL.md` markdown | TypeScript npm package | Separate process, any language |
| **Complexity** | Zero-code | Full code + lifecycle hooks | Full code + separate runtime |
| **Distribution** | ClawHub registry | npm / GitHub | Any URL or local |
| **Isolation** | None (in-process) | Application-level | Process-level |
| **Best for** | Quick capabilities, integrations | Deep system access, custom providers | External service integrations |
| **Example** | Gmail skill, Notion skill | ClawRouter, SecureClaw | Playwright MCP, GitHub MCP |

### 3. Memory Architecture
OpenClaw uses **filesystem-as-truth** memory — no vector database required by default.

| File | Purpose | Mutable by Agent? |
|---|---|---|
| `MEMORY.md` | Long-term distilled facts | ✅ Yes |
| `SOUL.md` | Core identity and values | ✅ Yes (unless locked) |
| `AGENTS.md` | Immutable operating instructions | ❌ No — agent cannot touch this |
| `memory/YYYY-MM-DD.md` | Daily episodic logs | ✅ Auto-appended |

### 4. Context Engineering
When approaching token limits, OpenClaw triggers **session compaction** — summarizing oldest turns while preserving tool call-result pairs. Sessions reset at configurable boundaries (default: 4 AM UTC). Result: effectively unlimited conversation length.

### 5. Channel Isolation
Each connected messaging platform is a **channel** with its own context namespace. Skills can be scoped per channel using `channels:` in the skill manifest. Run 10+ channels simultaneously with per-channel permission sets.

---

## 🤖 LLM Model Selection Guide

> This is one of the most common questions new users ask, and no other resource covers it well. Here is the community consensus as of March 2026.

### Model Comparison at a Glance

| Model | Provider | Strength | Weakness | Best OpenClaw Use Case |
|---|---|---|---|---|
| **Claude Sonnet 4** | Anthropic | Best tool-calling reliability; nuanced instruction following | Higher cost than Gemini | Default recommendation; daily driver for most users |
| **Claude Haiku 4** | Anthropic | Very fast, cheap | Less capable for complex multi-step tasks | High-volume triage, simple automations, notifications |
| **GPT-5** | OpenAI | Strong reasoning, very capable coding | Cost; sometimes over-verbose in tool calls | Complex coding tasks, analytical workflows |
| **Gemini 2.5 Pro** | Google | Longest context window (1M tokens); best price at scale | Tool call formatting occasionally inconsistent | Document-heavy workflows, research, long sessions |
| **Gemini 2.5 Flash** | Google | Fastest response, cheapest capable model | Less reliable on complex tool chains | Real-time automations, cost-sensitive deployments |
| **Llama 4 Scout** (Ollama) | Meta / Local | Free, fully private, no API key needed | Needs capable hardware (16GB+ VRAM recommended) | Air-gapped environments, privacy-critical data |
| **Qwen3-32B** (Ollama) | Alibaba / Local | Strong multilingual; excellent for non-English workloads | Hardware requirements | Multilingual deployments |
| **OpenRouter** | Multi | Automatic routing, unified billing, fallback logic | Adds latency, another dependency | Teams wanting flexibility; ClawRouter power users |

### Recommendation by Use Case

**Personal productivity agent (email, calendar, tasks):**
→ **Claude Sonnet 4** as primary. **Claude Haiku 4** for simple reminders and quick lookups. Route with ClawRouter.

**Software development assistant:**
→ **GPT-5** or **Claude Sonnet 4**. Both excel at code. GPT-5 slightly stronger on large refactors; Sonnet 4 more reliable on multi-step tool chains.

**Research and document processing:**
→ **Gemini 2.5 Pro** for its 1M token context window. Process entire codebases or large PDFs without chunking.

**Privacy-first / air-gapped deployment:**
→ **Llama 4 Scout** (16GB VRAM) or **Qwen3-14B** (8GB VRAM) via Ollama. No data leaves your machine.

**Cost-optimized high-volume:**
→ **Gemini 2.5 Flash** or **Claude Haiku 4**. Use ClawRouter to auto-route cheap tasks to these and expensive tasks to Sonnet/GPT-5.

### Configuring Multiple Models

```bash
# Configure a primary and fallback model
openclaw config set model.primary "Claude Sonnet 4.6"
openclaw config set model.fallback "gemini-2.5-flash"
openclaw config set model.coding "gpt-5"

# Or use OpenRouter for automatic routing
openclaw config set provider "openrouter"
openclaw config set model.primary "openrouter/auto"
```

### Local Model Setup with Ollama

```bash
# Install Ollama
curl -fsSL https://ollama.ai/install.sh | sh

# Pull a recommended model
ollama pull llama4:scout        # 16GB VRAM
ollama pull qwen3:14b           # 8GB VRAM
ollama pull mistral-nemo:12b    # 6GB VRAM (minimum viable)

# Point OpenClaw at local Ollama
openclaw config set provider "ollama"
openclaw config set model.primary "llama4:scout"
```

---

## 💰 Cost Estimation Guide

> One of the top reasons people hesitate to try OpenClaw. Here are real numbers.

### API Cost by Provider (March 2026 Pricing)

| Model | Input (per 1M tokens) | Output (per 1M tokens) | Typical turn cost |
|---|---|---|---|
| Claude Sonnet 4 | $3.00 | $15.00 | ~$0.005–0.02 |
| Claude Haiku 4 | $0.80 | $4.00 | ~$0.001–0.005 |
| GPT-5 | $10.00 | $30.00 | ~$0.01–0.05 |
| Gemini 2.5 Pro | $1.25 | $5.00 | ~$0.003–0.015 |
| Gemini 2.5 Flash | $0.15 | $0.60 | ~$0.0003–0.002 |
| Llama 4 / Ollama | $0 | $0 | Hardware cost only |

> *"Typical turn cost"* = one user message + agent response, including tool calls. Complex multi-step tasks cost more.

### Monthly Cost Estimates by Usage Profile

| Profile | Description | Est. Monthly API Cost |
|---|---|---|
| **Light** | ~50 messages/day, mostly simple tasks | $3–8/month |
| **Moderate** | ~200 messages/day, mix of simple and complex | $15–40/month |
| **Heavy** | ~500 messages/day, complex workflows with many tool calls | $50–150/month |
| **Team (5 people)** | Shared instance, ~1000 messages/day | $100–300/month |
| **Enterprise** | Custom; ClawTeam managed billing | Contact vendors |

> **Actual costs vary dramatically** based on model choice, skill complexity, and conversation length. The `cost-tracker` skill gives you real per-conversation data.

### Cost Optimization Strategies

**1. Use ClawRouter for intelligent routing (40–60% savings)**
```bash
openclaw skill install BlockRunAI/clawrouter
# Routes simple tasks (reminders, lookups) to Haiku/Flash
# Routes complex tasks (code, research) to Sonnet/GPT-5
# Users report 40-60% cost reduction
```

**2. Context window hygiene**
```bash
# Enable aggressive session compaction
openclaw config set context.compaction_threshold 0.7
openclaw config set context.reset_schedule "0 4 * * *"  # 4am UTC daily
```

**3. Scope skills narrowly**
Skills with broad triggers (`use this when the user asks anything about...`) consume more tokens evaluating whether to activate. Narrow trigger conditions = fewer wasted tokens.

**4. Use local models for bulk tasks**
Run Ollama locally for high-volume, lower-complexity tasks (email sorting, routine summaries). Zero marginal API cost.

### Total Cost of Ownership: Self-Hosted vs Managed

| | Self-Hosted VPS | Managed (ClawHost) | Self-Hosted Homelab |
|---|---|---|---|
| **Infrastructure** | $5–18/month (Hetzner/DO) | $10–30/month | ~$0/month (existing hardware) |
| **Setup time** | 30–120 min | 5–15 min | 2–4 hours |
| **Maintenance** | 1–2 hrs/month | None | 1–2 hrs/month |
| **Privacy** | High | Medium | Maximum |
| **Reliability** | High (99.9% SLA typical) | High | Depends on hardware |
| **Best for** | Most users | Beginners, busy professionals | Power users, homelabbers |

---

## 🔧 Skills & Plugins

### Official Skill Registry (ClawHub)

[**clawhub.ai**](https://clawhub.ai) — The official marketplace. **13,729 community-built skills** as of March 2026.

```bash
openclaw skill install steipete/slack
openclaw skill install community/playwright-mcp
openclaw skill list
openclaw skill remove steipete/slack
```

> ⚠️ ClawHub is open-submission. Not all skills are vetted. Always review source before installing. See the [Security](#-security) section.

### Curated "Must-Have" Skills

**🛡️ Install This First:**

| Skill | What it does | Why essential |
|---|---|---|
| `secureclaw` | Audits your install for CVEs, misconfigurations, prompt injection risks | **Install before anything else** |

**Productivity Core:**

| Skill | What it does | Stars / Installs |
|---|---|---|
| `playwright-mcp` | Full browser automation — browse, click, scrape, fill forms | Most-installed skill |
| `agentmail` | AI email triage, auto-replies, LLM-driven inbox management | 30–50% inbox time reduction (reported) |
| `notion-direct` | Bidirectional Notion sync | Best knowledge management integration |
| `obsidian-direct` | Reads/writes Obsidian vault directly | For Markdown-native PKM users |
| `google-calendar` | Full calendar management, natural language | "Book a meeting Tuesday afternoon" just works |
| `linear` | Create, update, triage Linear issues via chat | Essential for engineering teams |
| `github-mcp` | Full GitHub integration via MCP | PR reviews, issue management, code search |
| `composio` | Connect to 250+ apps via managed auth | Best for broad SaaS coverage |

**Development:**

| Skill | What it does |
|---|---|
| `claude-code` | Runs Claude Code as a sub-agent for coding tasks |
| `docker-manager` | Manage containers, images, and compose stacks |
| `cost-tracker` | Real-time LLM API cost monitoring and budget alerts |
| `cron-backup` | Scheduled backups with version tracking |

**Research & Data:**

| Skill | What it does |
|---|---|
| `web-research` | Multi-source web research with citation tracking |
| `arxiv-search` | Search and summarize arXiv papers |
| `perplexity-search` | Deep web search via Perplexity API |
| `supermemory` | External memory layer backed by Supermemory.ai |

### Skills by Category
For the full categorized index of 5,400+ vetted skills:
➡️ [**VoltAgent/awesome-openclaw-skills**](https://github.com/VoltAgent/awesome-openclaw-skills) — 1M+ monthly views, the #1 community skills resource.

### Building Your Own Skills

A skill is a `SKILL.md` file. Minimum viable skill:

```markdown
# my-skill

Use this skill when the user asks to [TRIGGER CONDITION].

## Setup
- Requires: API_KEY environment variable

## Tools

### do_thing
Does the thing.
Parameters:
- query (string): What to do

## Instructions
When triggered, call do_thing with the user's request.
Return the result in a friendly format.
```

**Skill authoring resources:**
- [Official Skills Documentation](https://docs.openclaw.ai/tools/skills) — SKILL.md loading mechanics, scope priority, token cost formula
- [SKILL.md Format Specification](https://github.com/openclaw/clawhub/blob/main/docs/skill-format.md) — frontmatter fields, env var declarations, binary dependencies, install spec
- [ClawHub CLI Publishing Tool](https://github.com/openclaw/clawhub) — `clawhub publish <path>`, `clawhub inspect <slug>`, versioning, soft-delete/restore
- [Skills: Install & Custom Development in Practice](https://openclawsetup.info/en/blog/openclaw-skills-install-and-write) — Real-world SKILL.md examples (ClickUp, Outlook, GitHub) with minimal permission configs
- [OpenClaw Skills Developer Guide (2026)](https://www.growexx.com/blog/openclaw-skills-development-guide-for-developers/) — Skill architecture, security boundaries, private registry setup
- [DigitalOcean: The Complete OpenClaw Skills Guide](https://www.digitalocean.com/resources/articles/what-are-openclaw-skills) — Beginner-friendly intro with security review tips

---

## 🤖 MCP Integrations

MCP (Model Context Protocol, originally by Anthropic) is the dominant architecture for new professional-grade OpenClaw skills. MCP servers run as independent processes, offering better isolation and language-agnosticism.

```bash
npm install -g mcporter
openclaw mcp add --url https://mcp.github.com/sse --name github
openclaw mcp add --local /path/to/my-mcp-server --name local-tools
```

### Notable MCP Servers

| Server | Category | Notes |
|---|---|---|
| [playwright-mcp](https://github.com/microsoft/playwright-mcp) | Browser | Most-used MCP in OpenClaw; full browser automation |
| [github-mcp](https://github.com/github/github-mcp-server) | DevOps | Official GitHub MCP |
| [filesystem-mcp](https://github.com/modelcontextprotocol/servers/tree/main/src/filesystem) | System | Read/write files with explicit path control |
| [memory-mcp](https://github.com/JamesANZ/memory-mcp) | Memory | Knowledge graph memory |
| [brave-search-mcp](https://github.com/brave/brave-search-mcp-server) | Search | Web search via Brave API |
| [fetch-mcp](https://github.com/zcaceres/fetch-mcp) | HTTP | Web fetching and scraping |
| [postgres-mcp](https://github.com/crystaldba/postgres-mcp) | Database | Read-only PostgreSQL access |
| [slack-mcp](https://mcp.slack.com) | Comms | Official Slack MCP |
| [gmail-mcp](https://gmail.mcp.claude.com) | Email | Gmail via MCP |
| [ToolRouter](https://toolrouter.com) | Multi-tool | One gateway to 150+ tools for AI agents. One API key replaces managing dozens of provider accounts. Includes SEO, screenshots, web search, image generation, video, security scanning, and more. Works with ChatGPT, Claude, Cursor. Growing daily. `npx -y toolrouter-mcp` |

Browse 13,000+ MCP servers at [mcp.so](https://mcp.so) or the [official MCP server directory](https://github.com/modelcontextprotocol/servers).

---

## 🖥️ UIs & Companion Apps

### Web UIs

| Tool | Description | Key Feature |
|---|---|---|
| [openclaw-studio](https://github.com/grp06/openclaw-studio) | Full-featured web dashboard | Skill management, memory viewer, cost analytics |
| [vibeclaw](https://github.com/jasonkneen/vibeclaw) | Browser-native interface — no local install | Test skills before production deploy |
| [openclaw-ui](https://docs.openclaw.ai/web/control-ui) | Official WebChat + Control UI | Ships with core |
| [ClawDash](https://clawdash.pro/) | OpenClaw agent interface | Advanced Next.js 15 UI boilerplate with 50+ components, modular layout and professional dashboard design |
| [OpenClaw Directory](https://openclawdir.com/) | Community skill/tool catalog | Searchable, community-rated |

### Desktop Apps

| Tool | Platform | Description |
|---|---|---|
| [OpenClaw for macOS](https://docs.openclaw.ai/platforms/macos) | macOS | Menu bar companion app; manages/connects to local Gateway and exposes macOS capabilities as nodes to the agent |
| [OpenClaw Manager](https://github.com/miaoxworld/openclaw-manager) | macOS / Windows | Desktop chat interface with visual file management |
| [OpenClaw Windows Hub](https://github.com/openclaw/openclaw-windows-node) | Windows | Windows companion suite for OpenClaw (AI personal assistant) |

### Mobile

| Tool | Platform | Description |
|---|---|---|
| [OpenClaw iOS App](https://docs.openclaw.ai/platforms/ios) | iOS | **Internal preview — not yet publicly released.** Connects to Gateway via WebSocket (LAN or tailnet); exposes node capabilities: canvas, screenshot, camera capture, location, call mode, voice wake. Receives `node.invoke` commands and reports node status events |
| [OpenClaw Android Node](https://docs.openclaw.ai/platforms/android) | Android | Official Android platform docs; community APK build at [openclaw-android-node-apk](https://github.com/bighamx/openclaw-android-node-apk) |

---

## 🌐 Platform Channels & Messaging

| Platform | Status | Notes |
|---|---|---|
| **Telegram** | ✅ Native | Best-supported; works on all implementations |
| **WhatsApp** | ✅ Native (Baileys) | Most popular for personal use; requires QR scan |
| **Discord** | ✅ Native | Guild + DM; slash commands available |
| **Slack** | ✅ Native | Full Events API + Block Kit |
| **iMessage** | ✅ macOS only | Needs BlueBubbles bridge on Linux/Windows |
| **Signal** | ✅ Via signal-cli | Best privacy option |
| **Google Chat** | ✅ Native | Workspace integration |
| **Microsoft Teams** | ✅ Beta | Bot Framework integration |
| **SMS** | ✅ Via Twilio | Pay-per-message |
| **Email** | ✅ Via skills | IMAP/SMTP or AgentMail plugin |
| **Voice** | 🧪 Experimental | OpenAI Realtime API, early-stage |
| **Web widget** | ✅ Via openclaw-ui | Embeddable for websites |

**Multi-channel tips:**
- Each channel has its own conversation namespace — skills can be scoped per channel
- Dedicate a cheap Telegram bot to low-priority tasks; keep WhatsApp for high-priority work
- Channel-level permission sets: restrict dangerous skills to trusted channels only

---

## ☁️ Deployment & Infrastructure

### Managed Hosting

| Service | Starting Price | Best For |
|---|---|---|
| [ClawHost](https://clawhost.cloud/) | $25–$350/month | Choose from 45+ provider servers to match your needs |
| [Tinkerclaw](https://tinkerclaw.com) | ~$49/month | Full onboarding support + OpenClaw Manager |
| [OpenClaw Launch](https://openclawlaunch.com) | ~$20/month | Simple managed + pre-configured skills |
| [DigitalOcean 1-Click](https://marketplace.digitalocean.com/apps/openclaw) | $12/month | Self-hosted but fast; full root access |

### Self-Hosted: Docker Compose

```yaml
version: '3.8'
services:
  openclaw:
    image: openclaw/openclaw:stable
    restart: unless-stopped
    ports:
      - "127.0.0.1:18789:18789"   # NEVER bind to 0.0.0.0 directly
    volumes:
      - ./data:/data
      - ./skills:/skills
    environment:
      - ANTHROPIC_API_KEY=${ANTHROPIC_API_KEY}
      - OPENCLAW_MEMORY_DIR=/data/memory
      - OPENCLAW_LOG_LEVEL=warn
    user: "1000:1000"
    read_only: true
    tmpfs: ["/tmp"]
    security_opt:
      - no-new-privileges:true
    healthcheck:
      test: ["CMD", "curl", "-f", "http://localhost:18789/health"]
      interval: 30s
      timeout: 10s
      retries: 3
```

### Self-Hosted: NixOS

```nix
services.openclaw = {
  enable = true;
  package = pkgs.openclaw;
  settings = { port = 18789; memoryDir = "/var/lib/openclaw/memory"; };
  environmentFile = "/run/secrets/openclaw-env";
};
```

See [nix-openclaw](https://github.com/openclaw/nix-openclaw) for the community NixOS module.

### VPS Price Comparison

| Provider | Tier | Cost | Notes |
|---|---|---|---|
| Hetzner | CX22 (2GB) | €4.15/mo | Best price/performance in EU |
| DigitalOcean | Basic 2GB | $18/mo | Most tutorials target this; 1-click available |
| Vultr | Regular 2GB | $12/mo | Good global coverage |
| Linode/Akamai | Nanode 1GB | $5/mo | Tight on RAM; upgrade if adding many skills |
| Oracle Cloud | Always Free 1GB | $0 | Free; performance varies |

### Homelab & Edge

| Resource | Notes |
|---|---|
| [Raspberry Pi Guide](https://www.raspberrypi.com/news/turn-your-raspberry-pi-into-an-ai-agent-with-openclaw/) | Pi 4 4GB+ required; Pi 5 preferred |
| [Mac Mini Setup](https://docs.openclaw.ai/zh-CN/install/macos-vm) | Recommended: silent, efficient, reliable |
| [Ansible Playbook](https://github.com/openclaw/openclaw-ansible) | Automated install with Tailscale VPN, UFW firewall and Docker isolation |
| [OpenClaw on Proxmox](https://merox.dev/blog/moltbot-proxmox-deployment/) | Community tutorial: complete Proxmox VE deployment guide |

---

## 🏢 Enterprise Deployment

> For teams and organizations with compliance, multi-tenancy, and governance requirements.

### Authentication & Access Control

**Single Sign-On (SSO):**
```bash
# SAML 2.0 via Nginx auth_request
# OpenClaw itself is auth-agnostic; put auth in your reverse proxy layer
# Community guide: https://docs.openclaw.ai/enterprise/sso
```

| Tool | Description |
|---|---|
| [agent-access-control skill](https://clawhub.ai/community/agent-access-control) | Tiered access control — restrict which users trigger which actions |

### Multi-Tenancy Patterns

OpenClaw does not have native multi-tenancy. Enterprise teams use one of three patterns:

**Pattern A — One instance per team/user (Recommended)**
```
User A → Gateway A (port 18789) → Memory A
User B → Gateway B (port 18790) → Memory B
```
Complete isolation. Simple. Works with Ansible or Docker Compose per user.

**Pattern B — Shared instance, per-channel isolation**
One Gateway, multiple channels, channel-scoped skills and permissions. Lower cost; shared memory is a risk.

**Pattern C — ClawTeam managed multi-tenancy**
ClawTeam handles auth, routing, and billing. Best for teams >10 people who don't want to manage infra.

### Compliance & Auditing

| Tool | Description | Standard |
|---|---|---|
| [agent-audit-trail](https://clawhub.ai/community/agent-audit-trail) | Tamper-evident hash-chained action logs | SOC 2 Type II compatible |
| [SecureClaw](https://github.com/adversa-ai/secureclaw) | 55-point security audit; OWASP ASI + MITRE ATLAS mappings | OWASP ASI Top 10 |
| [NemoClaw](https://github.com/nvidia/nemoclaw) | NVIDIA-sandboxed build; GPU-accelerated, fully isolated | Air-gap ready |

### Data Residency

By default, your data goes to your chosen LLM provider's API. For organizations with data residency requirements:

- **EU:** Use Anthropic EU endpoints or Gemini EU-hosted endpoints; deploy OpenClaw on Hetzner Germany
- **Air-gap:** Run Ollama locally — zero data leaves your network. See [Ollama × OpenClaw Integration Guide](https://docs.ollama.com/integrations/openclaw)
- **On-premise:** NemoClaw for fully isolated deployments with local GPU inference

### Disaster Recovery

```bash
# Backup your entire OpenClaw state
tar -czf openclaw-backup-$(date +%Y%m%d).tar.gz \
  ~/openclaw-data/memory \
  ~/openclaw-data/skills \
  ~/.openclaw/config.json

# Restore
tar -xzf openclaw-backup-20260315.tar.gz -C ~/openclaw-data/
```

The `cron-backup` skill automates this on a schedule and optionally uploads to S3, Backblaze B2, or any S3-compatible provider.

---

## 🧠 Memory & Knowledge Systems

### Built-in Memory Files

| File | Purpose | Mutable by Agent |
|---|---|---|
| `MEMORY.md` | Long-term distilled facts and preferences | ✅ |
| `SOUL.md` | Core identity, values, operating instructions | ✅ (lock recommended) |
| `AGENTS.md` | Immutable rules — agent cannot override | ❌ |
| `memory/YYYY-MM-DD.md` | Daily episodic logs | ✅ Auto-appended |

### External Memory Integrations

| Tool | Description | Best For |
|---|---|---|
| [Supermemory](https://supermemory.ai) | Managed external memory with semantic search | Teams needing shared memory across instances |
| [Graphiti](https://github.com/getzep/graphiti) | Temporal knowledge graph memory | Complex relational knowledge over time |
| [MemOS](https://github.com/MemTensor/MemOS) | Hierarchical memory OS for LLM agents | Research-grade memory architecture |
| [mem0](https://github.com/mem0ai/mem0) | Self-improving personalized memory | Personalization-heavy workflows |

### Memory Best Practices

1. **Keep `SOUL.md` short and opinionated.** 200–300 words. Specific beats generic.
2. **Use `AGENTS.md` for non-negotiable rules.** Security policies, content restrictions, tool limits — the agent cannot override it.
3. **Prune `MEMORY.md` monthly.** Old facts accumulate. Review and remove stale entries.
4. **Separate work and personal contexts** using channel-scoped memory with different channel configurations.
5. **Never put credentials in memory files.** Use environment variables or the secrets manager.

---

## 🔒 Security

> This section exists because no other Awesome OpenClaw list treats security seriously enough. OpenClaw runs with broad system access. Security is not optional.

### Known CVEs & Incidents

| CVE / Incident | Severity | Description | Mitigation |
|---|---|---|---|
| **CVE-2026-25253** | 🔴 Critical | WebSocket RCE — unauthenticated remote code execution if gateway exposed to internet | Update to v1.8.4+. Never expose port 18789 directly. |
| **ClawHub Malicious Skills (Jan 2026)** | 🔴 High | 341 malicious skills; some exfiltrated data via Base64-chunked requests to unknown endpoints. 26% of popular skills had at least one high-severity vector (Cisco research) | Use SecureClaw + `skill-guard` before installing any skill |
| **41K+ Exposed Instances (Feb 2026)** | 🔴 High | 41,600 OpenClaw gateways publicly exposed; 2,100+ leaking API keys | Audit firewall rules. Use the SecureClaw network audit. |
| **Prompt Injection via Skill Descriptions** | 🟠 Medium | Malicious skills embed hidden instructions overriding user intent | SecureClaw behavioral rules; review skill source |
| **API Key in Memory Logs** | 🟡 Low–Medium | Agent wrote API keys to daily logs when processing config messages | Fixed in v1.9.1; audit old `memory/` logs |

### Essential Security Tools

#### SecureClaw (Install First)

[**SecureClaw**](https://github.com/adversa-ai/secureclaw) by Adversa AI:
- 55 audit checks across the full attack surface
- 15 behavioral rules (~1,150 tokens) against prompt injection
- Maps to OWASP ASI Top 10 and MITRE ATLAS

```bash
openclaw plugin add secureclaw
openclaw skill install adversa-ai/secureclaw
openclaw secureclaw audit --full
openclaw secureclaw harden
```

#### Other Security Tools

| Tool | Description |
|---|---|
| [skill-guard](https://clawhub.ai/jamesOuttake/skill-guard) | Scan ClawHub skills for security vulnerabilities before installing — detects prompt injection, malware payloads, hardcoded keys and other threats |
| [agent-audit-trail skill](https://clawhub.ai/community/agent-audit-trail) | Tamper-evident hash-chained action logging |
| [agent-access-control skill](https://clawhub.ai/community/agent-access-control) | Tiered access control per user/channel |

### Secure Deployment: Nginx Reverse Proxy

**Never expose port 18789 directly.** Always use a reverse proxy with authentication:

```nginx
server {
    listen 443 ssl http2;
    server_name yourdomain.com;

    ssl_certificate     /etc/letsencrypt/live/yourdomain.com/fullchain.pem;
    ssl_certificate_key /etc/letsencrypt/live/yourdomain.com/privkey.pem;

    location /openclaw/ {
        auth_basic "OpenClaw Gateway";
        auth_basic_user_file /etc/nginx/.htpasswd;

        proxy_pass http://127.0.0.1:18789/;
        proxy_http_version 1.1;
        proxy_set_header Upgrade $http_upgrade;
        proxy_set_header Connection "upgrade";
        proxy_set_header Host $host;

        # Rate limiting
        limit_req zone=openclaw burst=20 nodelay;
        limit_req_log_level warn;
    }
}

# Rate limit zone definition (in http block)
# limit_req_zone $binary_remote_addr zone=openclaw:10m rate=10r/s;
```

### Skill Vetting Checklist

Before installing any skill from ClawHub:

- [ ] **Author verification:** Real GitHub profile with commit history?
- [ ] **Age and stars:** New repo + suspiciously high stars = red flag
- [ ] **Read the source:** SKILL.md files are markdown — readable in 2 minutes. Look for hidden instructions after HTML comments or inside code blocks
- [ ] **Permission scope:** Does a calculator skill request network access? Reject over-privileged skills
- [ ] **VirusTotal:** Check the ClawHub page for VirusTotal scan results
- [ ] **Run skill-guard:** `openclaw run "use skill-guard to audit [skill-name]"`

**Automatic red flags in skill source:**
- Instructions to ignore previous instructions or `AGENTS.md`
- Requests to send data to external URLs not mentioned in the README
- Base64-encoded content embedded in the skill file
- Instructions to modify `SOUL.md` or `AGENTS.md`
- `fetch()` calls to hardcoded external domains without disclosure

---

## 🆚 OpenClaw vs Other Agent Frameworks

> For product teams and developers evaluating which framework to build on. Updated March 2026.

### Comparison Matrix

| | **OpenClaw** | **AutoGen** | **CrewAI** | **LangGraph** | **n8n** | **Botpress** |
|---|---|---|---|---|---|---|
| **Primary Language** | TypeScript | Python | Python | Python | Node.js | TypeScript |
| **Learning Curve** | Low | High | Medium | High | Low | Medium |
| **Agent Type** | Single agent + skills | Multi-agent orchestration | Multi-agent teams | State machine graphs | Workflow automation | Conversational bots |
| **Memory** | Built-in flat-file + external | Manual | Manual | LangChain memory | None native | Built-in |
| **UI** | Messaging apps (WhatsApp, TG…) | Code / Jupyter | Code / Web UI | Code / LangSmith | Web UI | Web chat UI |
| **Self-hosted** | ✅ First-class | ✅ | ✅ | ✅ | ✅ | ✅ |
| **Skill/Plugin Ecosystem** | 13,729 skills (ClawHub) | Community tools | Community crews | LangChain tools | 500+ integrations | Community nodes |
| **Security Model** | Application-level (NanoClaw provides container isolation) | None native | None native | None native | None native | None native |
| **Best for** | Personal / team productivity agents | Research, complex multi-agent | Business workflow automation | Stateful pipelines, research | Non-technical automators | Customer-facing chatbots |
| **Worst for** | Complex multi-agent pipelines | Non-technical users | Real-time personal assistants | Simple use cases | LLM-heavy workflows | Power users needing full control |
| **GitHub Stars** | 247K | 38K | 26K | 12K | 51K | 14K |

### When to Choose OpenClaw

✅ **Choose OpenClaw if:**
- You want a personal productivity agent you interact with via messaging apps
- You need a large ecosystem of pre-built skills (13,729 on ClawHub)
- You want low-code skill authoring (SKILL.md format)
- Local-first, self-hosted privacy matters to you
- You're building for a team that will use their existing chat tools

❌ **Don't choose OpenClaw if:**
- You need complex multi-agent orchestration with elaborate handoff protocols (→ use AutoGen or CrewAI)
- You're building a customer-facing chatbot with conversation flows (→ use Botpress)
- You need a visual no-code automation builder for non-technical users (→ use n8n)
- You're doing research requiring fine-grained state machine control (→ use LangGraph)

### OpenClaw vs AutoGen

The most common comparison. Key difference: AutoGen is designed for **multi-agent systems** where agents collaborate in code. OpenClaw is designed for **single-agent productivity** with a rich skill ecosystem. If you want an AI assistant that takes actions on your behalf via chat, OpenClaw wins. If you want agents collaborating to solve complex research problems, AutoGen wins.

### OpenClaw vs n8n

n8n is a visual workflow automation tool for non-technical users. OpenClaw is a conversational agent for power users. They're complementary: many users run n8n for scheduled workflows and OpenClaw for on-demand conversational tasks. The `n8n-webhook` skill bridges the two.

---

## 🌍 Ecosystem & Agent Platforms

### Agent Social & Collaboration

| Platform | Description |
|---|---|
| [Moltbook](https://moltbook.com) | Agent-native social network — agents post, follow, and interact |
| [Clawk](https://clawk.ai/) | 𝕏/Twitter for AI Agents — the place to discover what agents are up to, up to 400 characters at a time |
| [AgentDo](https://agentdo.dev) | Task marketplace — post tasks for agents or have your agent pick up work |

### Agent-to-Agent (A2A)

| Resource | Description |
|---|---|
| [A2A Protocol Spec](https://github.com/a2aproject/A2A) | Open agent interoperability protocol, initiated by Google |
| [ACP — Agent Communication Protocol](https://agentcommunicationprotocol.dev/) | Open agent interoperability protocol designed to address the growing challenge of connecting AI agents, applications and more |
| [agent-team-orchestration skill](https://clawhub.ai/community/agent-team-orchestration) | Multi-agent teams with roles, tasks, handoffs, review |
| [agentgate skill](https://clawhub.ai/community/agentgate) | API gateway with human-in-the-loop write approval |

---

## 🛠️ Developer Tooling

### Deployment & Management

| Tool | Description |
|---|---|
| [openclaw-ansible](https://github.com/openclaw/openclaw-ansible) | Official automated install with Tailscale VPN, UFW firewall and Docker security hardening |

### Development & Testing

| Tool | Description |
|---|---|
| [Plugin SDK Documentation](https://docs.openclaw.ai/tools/plugin) | Plugin SDK ships as sub-path exports within the main package (`openclaw/plugin-sdk/core`, `/telegram`, `/discord`, etc.) — no separate package |
| [Vibeclaw](https://github.com/jasonkneen/vibeclaw) | Browser-based sandbox — test without touching production |
| [ClawHub CLI](https://github.com/openclaw/clawhub) | Official publishing tool: `clawhub publish`, `clawhub inspect`, versioning, soft-delete/restore |

### Monitoring & Observability

| Tool | Description |
|---|---|
| [openclaw-dashboard](https://github.com/tugcantopaloglu/openclaw-dashboard) | Secure real-time monitoring dashboard with authentication, TOTP MFA, cost tracking, live data streaming and memory browser |
| [cost-tracker skill](https://clawhub.ai/community/cost-tracker) | Per-conversation API cost tracking with budget alerts |

### Cost Optimization

| Tool | Description |
|---|---|
| [ClawRouter](https://github.com/BlockRunAI/ClawRouter) | Agent-native LLM router supporting 41+ models, sub-1ms routing latency, USDC payments via x402 on Base and Solana |
| [Model Router](https://clawhub.ai/MrJootta/model-router-premium) | Routes model requests based on configured models, costs and task complexity — general/low-complexity requests to the cheapest available model, higher-complexity to stronger models |

---

## 🏗️ Alternative Implementations

### Decision Matrix

| | OpenClaw | NanoClaw | ZeroClaw | Moltis | PicoClaw | Nanobot |
|---|---|---|---|---|---|---|
| **Language** | TypeScript | Python | Rust | Rust | Go | Python |
| **RAM** | ~1.52 GB | ~100 MB | ~7.8 MB | ~120 MB | <10 MB | ~110 MB |
| **Binary** | 28 MB+ | N/A | 3.4 MB | ~12 MB | <10 MB | N/A |
| **Startup** | ~6 sec | ~2 sec | <10 ms | ~1.5 sec | ~1 sec | ~3 sec |
| **Isolation** | Application | Container | Multi-layer | Process | None | None |
| **Skills Ecosystem** | 13,729 (ClawHub) | Via skills | MCP-based | Limited | Limited | MCP-based |
| **Best For** | Max features | Security-first | Edge/IoT | Enterprise | Embedded | Learning |

### Implementations

**[OpenClaw](https://github.com/openclaw/openclaw)** — Reference implementation. Choose when: you want the largest skill ecosystem and accept the resource tradeoffs as the cost of maturity.

**[NanoClaw](https://github.com/qwibitai/nanoclaw)** — Python, mandatory container isolation, ~700 lines (auditable in an afternoon). Choose when: security and auditability matter more than skill count. Regulated environments.

**[ZeroClaw](https://github.com/zeroclaw-labs/zeroclaw)** — Rust, 3.4MB binary, <10ms startup, 7.8MB RAM (194× smaller than OC), direct OpenClaw config import, 22+ providers. Choose when: resource efficiency matters, or you want a migration path from OpenClaw.

**[Moltis](https://github.com/moltis-org/moltis)** — A trusted Rust-native Claw. One binary — sandboxed, secure, auditable. Built-in voice, memory, MCP tools and multi-channel access. Choose when: your team needs a trustworthy enterprise-grade Rust implementation.

**[PicoClaw](https://github.com/sipeed/picoclaw)** — Go, <10MB RAM, 1-second startup, targets $10 RISC-V hardware. Choose when: IoT, home automation, embedded Linux, cheapest possible hardware.

**[Nanobot](https://github.com/HKUDS/nanobot)** — Python, ~4,000 lines, maximum readability, MCP-only tools. Choose when: learning agent internals, prototyping architectures, academic research.

**[NullClaw](https://github.com/nullclaw/nullclaw)** — Zig, 1MB RAM, 678KB binary. Choose when: absolute minimal footprint, microcontroller-adjacent.

| Project | Language | Key Idea |
|---|---|---|
| [ClawGo](https://github.com/openclaw/clawgo) | Go | Headless, voice + text, embedded Linux |
| [MimiClaw](https://github.com/memovai/mimiclaw) | C | ESP32 microcontroller version |
| [Carapace](https://github.com/carapace-sh/carapace) | Various | Governance/compliance first |

---

## 📖 Tutorials, Blogs & Articles

### Getting Started
- [Official OpenClaw Quickstart](https://docs.openclaw.ai/quickstart)
- [Deep Dive: Architecture, Code & Ecosystem](https://medium.com/@dingzhanjun/deep-dive-into-openclaw-architecture-code-ecosystem-e6180f34bd07)
- [What Are OpenClaw Skills? A 2026 Developer's Guide](https://www.digitalocean.com/resources/articles/what-are-openclaw-skills)
- [The Ecosystem: ClawHub and Skills](https://repovive.com/roadmaps/openclaw/what-is-openclaw/the-ecosystem-clawhub-and-skills)
- [Top 6 OpenClaw Tools Developers Are Using in 2026](https://www.indiehackers.com/post/top-6-openclaw-tools-developers-are-using-in-2026-f25e9a48ae)

### Intermediate & Advanced
- [OpenClaw New Features 2026](https://openclaw.ai/blog/) — Official blog roundup
- [Best Skills, Plugins and Automations: The Ultimate Guide](https://www.pcbuildadvisor.com/best-openclaw-skills-plugins-and-automations-the-ultimate-guide-2026/)
- [Maximize Efficiency: Top 10 Plugins for 2026](https://openclawforge.com/blog/best-openclaw-plugins-productivity-2026/)

### Security
- [CVE-2026-25253 Post-mortem](https://openclaw.ai/blog/) — Official security analysis
- [SecureClaw: Dual Stack Security Plugin](https://www.helpnetsecurity.com/2026/02/18/secureclaw-open-source-security-plugin-skill-openclaw/)
- [A Security-First Guide to OpenClaw Alternatives](https://www.shareuhack.com/en/posts/openclaw-alternatives-guide)

### Alternatives & Ecosystem
- [Best OpenClaw Variants](https://medium.com/data-science-in-your-pocket/best-openclaw-variants-to-know-2aac9eb6bd6d) — Categorized breakdown
- [Everything is Agent: Alternatives Deep Dive](https://x.com/KSimback/status/2028429891050275053)
- [The Claw Craziness Continues](https://evoailabs.medium.com/openclaw-nanobot-picoclaw-ironclaw-and-zeroclaw-this-claw-craziness-is-continuing-87c72456e6dc)

### Learning Paths
- [Repovive OpenClaw Roadmap](https://repovive.com/roadmaps/openclaw) — 9-hour structured course, 165 units

---

## 🎥 Videos & Talks

| Resource | Type | Description |
|---|---|---|
| [Lex Fridman #491: OpenClaw — The AI Agent Breaking the Internet](https://www.youtube.com/watch?v=YFjfBk8HI5o) | Interview (3h15m) | Creator Steinberger in deep conversation with Lex Fridman: origin story, architecture, Moltbook controversy, security risks, the future of autonomous agents. **Best first video for understanding OpenClaw** |
| [OpenClaw Creator: Full Real-World Demo](https://www.youtube.com/watch?v=AcwK1Uuwc0U) | Demo interview | Peter Yang (Creator Economy) talks to Steinberger: automated flight check-in, smart home control, counterintuitive AI coding workflows (no Plan Mode, no MCP). 2.71M views |
| ["I Ship Code I Haven't Read" — OpenClaw Creator Interview](https://newsletter.pragmaticengineer.com/p/the-creator-of-clawd-i-ship-code) | Podcast / video | Pragmatic Engineer (Gergely Orosz) interviews Steinberger in London just before the viral explosion — deep dive into AI-assisted development workflows. Available on YouTube and Spotify |
| [OpenClaw Creator × OpenAI Developer Experience Lead](https://techcrunch.com/2026/02/25/openclaw-creators-advice-to-ai-builders-is-to-be-more-playful-and-allow-yourself-time-to-improve/) | Podcast | OpenAI Builders Unscripted episode 1: Steinberger and Romain Huet on the early journey and advice for AI builders |
| [50 Days of Real Workflows: 20 Prompt Templates](https://gist.github.com/velvet-shark/b4c6724c391f612c4de4e9a07b0a74b6) | Companion resource | GitHub Gist with 20 real, copy-paste-ready prompts: morning briefings, backups, YouTube analytics, multilingual onboarding assistants and more |

---

## 📚 Research & Academic Resources

### Key Papers

| Paper | Relevance |
|---|---|
| [Defensible Design for OpenClaw (2026)](https://arxiv.org/abs/2603.13151) | Comprehensive security framework; maps attack surface to OWASP ASI |
| [ToolSword: Safety Issues in Tool Learning (2024)](https://arxiv.org/abs/2402.10753) | Foundational work on tool-invocation safety — directly applicable to skills |
| [AgentBench: Evaluating LLMs as Agents (2023)](https://arxiv.org/abs/2308.03688) | Benchmark framework; used to evaluate OpenClaw variants |
| [Prompt Injection Attacks (2023)](https://arxiv.org/abs/2306.05499) | Defines the prompt injection threat model affecting skill security |
| [ReAct: Reasoning + Acting (2022)](https://arxiv.org/abs/2210.03629) | The ReAct pattern that OpenClaw's agent loop is based on |

### Academic Projects
- [OWASP Agentic Security Initiative](https://genai.owasp.org/initiatives/agentic-security-initiative/) — OpenClaw used as reference implementation for ASI Top 10
- [MITRE ATLAS](https://atlas.mitre.org) — Globally accessible, continuously updated knowledge base of adversarial tactics and techniques against AI systems, based on real-world attack observations from AI red teams and security groups; SecureClaw includes formal MITRE ATLAS mappings
- [Nanobot](https://github.com/HKUDS/nanobot) — Best platform for studying agent internals; easy to instrument

---

## 💼 Use Cases & Showcases

### By Domain

**Personal Productivity:**
- Email → zero: Route all email through OpenClaw; auto-triage, draft for approval, auto-send routine responses
- Calendar management: Natural language scheduling that actually understands context
- Personal CRM: Remember context from all your relationships; briefed before meetings automatically

**Software Development:**
- PR review assistant: Daily summaries of open PRs across all your repos
- Incident responder: Monitors logs, pages on-call, drafts incident reports
- Dependency auditor: Weekly scan for outdated or vulnerable packages

**Business Operations:**
- Meeting notetaker: Record, transcribe, summarize, distribute
- CRM intelligence: Monitor email, update HubSpot/Salesforce automatically
- Report generator: Weekly metrics drafted and sent every Monday morning

**Research & Data:**
- Literature monitor: Daily digest of new arXiv papers matching your interests
- Competitive intelligence: Monitor competitors' GitHub, blog posts, job postings
- Data pipeline: Scrape → clean → analyze → summarize on a schedule

**Showcase Collections:**
- [hesamsheikh/awesome-openclaw-usecases](https://github.com/hesamsheikh/awesome-openclaw-usecases) — The definitive use case collection
- [LAMBDASOFT-org/awesome-openclaw-ecosystem](https://github.com/LAMBDASOFT-org/awesome-openclaw-ecosystem) — Agent-native platform showcases

---

## ❓ FAQ & Troubleshooting

### Installation & Setup

**Q: What are the minimum hardware requirements?**
A: Node.js 20+ for OpenClaw core. Minimum 1GB RAM (2GB recommended for comfortable operation with several skills). Any modern 64-bit OS. For local models via Ollama: 8GB VRAM minimum; 16GB recommended.

**Q: What's the difference between `openclaw onboard` and `openclaw start`?**
A: `onboard` is a one-time interactive wizard that sets up your config, connects your first channel, and installs essential skills. `start` just starts the gateway with existing config. Always run `onboard` first.

**Q: Do I need a paid API key to get started?**
A: No. You can run fully locally using Ollama + an open-source model (Llama 4, Qwen3). The experience is less capable but costs nothing. Most users start with a Claude or OpenAI API key for the best out-of-the-box quality.

---

### Gateway & Connection Issues

**Q: Gateway starts but I can't connect from my messaging app.**
A: Check these in order:
1. Confirm port 18789 is not blocked: `curl http://localhost:18789/health`
2. If using Docker, ensure you're binding correctly: `127.0.0.1:18789:18789` (not `0.0.0.0`)
3. If accessing remotely, confirm your reverse proxy is correctly configured
4. Check logs: `openclaw logs --tail 50`

**Q: WhatsApp keeps disconnecting every few hours.**
A: This is a Baileys (WhatsApp Web library) limitation. Solutions:
- Keep the QR-scanned device active and connected to the internet
- Configure auto-reconnect rules in `AGENTS.md`, or use a deployment script with watchdog support
- Consider switching to Telegram as your primary channel — it's more stable for server deployments

**Q: My Telegram bot stopped responding.**
A: 99% of the time this is a bot token issue or a conflicting webhook. Check:
```bash
openclaw channel status telegram
openclaw channel reconnect telegram
```

---

### Performance & Memory

**Q: OpenClaw is using 2GB+ of RAM. Is that normal?**
A: With the full skill ecosystem loaded, yes. Mitigation strategies:
- Use `openclaw skill list --active` to audit which skills are loaded
- Uninstall skills you don't use: `openclaw skill remove [name]`
- Consider ZeroClaw (7.8MB RAM) if resource efficiency is critical

**Q: Responses are getting slower over long conversations.**
A: Context window is filling up. Solutions:
- Enable aggressive compaction: `openclaw config set context.compaction_threshold 0.7`
- Schedule daily resets: `openclaw config set context.reset_schedule "0 4 * * *"`
- Configure health checks and auto-restart in your `docker-compose.yml`

**Q: Memory is growing unboundedly. `MEMORY.md` is now 50,000 words.**
A: The agent will write memories indefinitely if not pruned. Best practices:
- Set a monthly calendar reminder to review and prune `MEMORY.md`
- Use the `memory-manager` skill to auto-summarize and compress old entries
- Hard limit: Add to `AGENTS.md`: "Keep MEMORY.md under 10,000 words. Summarize and compress when approaching that limit."

---

### Skills & Security

**Q: I installed a skill and now my agent is behaving strangely.**
A: Likely prompt injection via a malicious or poorly written skill. Steps:
1. Disable the skill: `openclaw skill disable [name]`
2. Review its source code for hidden instructions
3. Run `openclaw secureclaw audit --full`
4. Report to ClawHub if it's genuinely malicious

**Q: How do I prevent a skill from accessing the internet?**
A: Add to `AGENTS.md`:
```
[skill-name] must never make external network requests except to [approved-domain].
```
For stronger enforcement, use agent-access-control skill or switch to NanoClaw which offers container-level isolation.

**Q: My API key was accidentally written to a memory log. What do I do?**
1. Immediately rotate the key at your provider's console
2. Delete the affected log: `rm ~/openclaw-data/memory/[date].md`
3. Run `openclaw secureclaw audit` to check for other exposures
4. Add to `AGENTS.md`: "Never write, log, or repeat API keys, tokens, or credentials under any circumstances."

---

### Costs & Models

**Q: My API costs are much higher than expected.**
A: Common causes:
1. Skills with very broad trigger conditions → audit with `cost-tracker` skill
2. No session compaction → conversations accumulate context indefinitely
3. Wrong model for the task → use ClawRouter to route cheap tasks to cheap models
4. Context window leaks from a poorly written skill loading large documents

**Q: Can I set a monthly spending cap?**
A: Not natively in OpenClaw core, but:
- The `cost-tracker` skill sends alerts when you hit thresholds
- Set hard limits directly at your API provider (Anthropic, OpenAI all support this)
- ClawRouter can be configured to stop routing to expensive models after a cost limit

---

### Updates & Migrations

**Q: How do I safely update OpenClaw?**
```bash
# Backup first
tar -czf ~/openclaw-backup-$(date +%Y%m%d).tar.gz ~/openclaw-data/

# Update
npm update -g openclaw

# Verify
openclaw --version
openclaw health check
```

**Q: How do I migrate from OpenClaw to ZeroClaw?**
ZeroClaw supports direct config import:
```bash
zeroclaw migrate --from ~/.openclaw
# Memory and config files are compatible; most skills work via MCP bridge
```

---

## 🤝 Community & Support

### Official Channels

| Channel | Description |
|---|---|
| [GitHub Issues](https://github.com/openclaw/openclaw/issues) | Bug reports, feature feedback, CVE disclosures |
| [Discord](https://discord.gg/openclaw) | Real-time help; #skills, #deployment, #security channels |
| [X / Twitter](https://x.com/openclaw) | News, tips, community highlights |

### Key People to Follow

| Handle | Why |
|---|---|
| [@steipete](https://x.com/steipete) | Creator; shares architectural thinking |
| [@voltagent_dev](https://x.com/voltagent_dev) | Maintains awesome-openclaw-skills |
| [@KSimback](https://x.com/KSimback) | Best ongoing alternatives ecosystem analysis |
| [@adversa_ai](https://x.com/adversa_ai) | Security researchers behind SecureClaw |

### Newsletters

| Newsletter | Focus |
|---|---|
| [OpenClaw Newsletter](https://buttondown.com/openclaw-newsletter) | Daily updates: releases, community highlights, security alerts and ecosystem news, curated by community maintainers on Buttondown |

---

## 🗺️ Related Awesome Lists

| List | Scope |
|---|---|
| [VoltAgent/awesome-openclaw-skills](https://github.com/VoltAgent/awesome-openclaw-skills) | 5,400+ curated skills — the specialized skills index |
| [hesamsheikh/awesome-openclaw-usecases](https://github.com/hesamsheikh/awesome-openclaw-usecases) | Real-world use cases by domain |
| [vincentkoc/awesome-openclaw](https://github.com/vincentkoc/awesome-openclaw) | General community list |
| [awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers) | Full MCP ecosystem |
| [awesome-ai-agents](https://github.com/e2b-dev/awesome-ai-agents) | Broader AI agent landscape |
| [awesome-llm-apps](https://github.com/Shubhamsaboo/awesome-llm-apps) | LLM application patterns |
| [awesome-selfhosted](https://github.com/awesome-selfhosted/awesome-selfhosted) | Self-hosting ecosystem |

---

## 🤝 Contributing

Contributions are welcome! This list aims to be **opinionated and high-quality**, not exhaustive.

**Before submitting a PR:**
1. Have you actually used or read this resource? No link-farming.
2. Add a description — every entry needs context: what, who, why.
3. Check for duplicates first.
4. Match the existing table/list format.
5. Security resources get priority review.

See [CONTRIBUTING.md](CONTRIBUTING.md) for the full guide and [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) for community standards.

**To report a malicious skill or security issue:** Open an Issue with the `security` label. Do not submit CVEs as PRs.

---

<div align="center">

**Found this useful?** Give it a ⭐ and share it with your team.
**Something missing or wrong?** [Open an issue](https://github.com/EthanYolo01/Awesome-OpenClaw/issues) or submit a PR.

*Last updated: March 2026 · Maintained with ❤️ by the community*

🌐 Language / 语言切换：**English** | [中文](README_CN.md)

</div>
