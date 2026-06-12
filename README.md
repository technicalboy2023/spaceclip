---
title: HuggingClip
emoji: 📎
colorFrom: gray
colorTo: purple
sdk: docker
app_port: 7861
pinned: true
license: mit
secrets:
  - name: HF_TOKEN
    description: Hugging Face API token for database backup.
  - name: CLAUDE_CODE_OAUTH_TOKEN
    description: Anthropic Claude API key for Claude-powered agents.
  - name: GEMINI_API_KEY
    description: Google Gemini API key for Gemini-powered agents.
  - name: OPENAI_API_KEY
    description: OpenAI API key for GPT-powered agents.
  - name: CLOUDFLARE_WORKERS_TOKEN
    description: "Cloudflare API token — auto-creates a Worker proxy and KeepAlive monitor."
---

<!-- Badges -->
<p align="center">
  <a href="https://github.com/technicalboy2023/spaceclip/stargazers"><img src="https://img.shields.io/github/stars/technicalboy2023/spaceclip?style=for-the-badge&logo=github&color=gold" alt="GitHub Stars"></a>
  <a href="https://github.com/technicalboy2023/spaceclip/network"><img src="https://img.shields.io/github/forks/technicalboy2023/spaceclip?style=for-the-badge&logo=github&color=blue" alt="GitHub Forks"></a>
  <a href="https://github.com/technicalboy2023/spaceclip/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge&logo=open-source-initiative" alt="License: MIT"></a>
  <a href="https://huggingface.co/spaces/technicalboy2023/HuggingClip"><img src="https://img.shields.io/badge/🤗%20HuggingFace-Space-blue?style=for-the-badge" alt="HF Space"></a>
  <a href="https://github.com/technicalboy2023/spaceclip/commits/main"><img src="https://img.shields.io/github/last-commit/technicalboy2023/spaceclip?style=for-the-badge&logo=git&color=brightgreen" alt="Last Commit"></a>
  <a href="https://paperclip.ing"><img src="https://img.shields.io/badge/Paperclip-AI%20Agents-purple?style=for-the-badge" alt="Paperclip"></a>
</p>

<!-- Loading animation for HF Space -->
<div align="center">
  <img src="https://img.shields.io/badge/Status-Online-success?style=flat-square&logo=statuspage" alt="Status"/>
  <img src="https://img.shields.io/badge/Runtime-Docker-blue?style=flat-square&logo=docker" alt="Docker"/>
  <img src="https://img.shields.io/badge/Database-PostgreSQL-4169E1?style=flat-square&logo=postgresql" alt="PostgreSQL"/>
  <img src="https://img.shields.io/badge/GPU-Free-brightgreen?style=flat-square&logo=nvidia" alt="Free GPU"/>
</div>

<br/>

<h1 align="center">HuggingClip 🚀</h1>
<p align="center"><strong>Deploy a fully-featured AI agent orchestration platform on Hugging Face Spaces for free.</strong><br/>Run Claude Code, OpenAI GPT, and Google Gemini agents with persistent storage, auto failover, and zero maintenance.</p>

<hr/>

## Why HuggingClip?

Most AI agent platforms require expensive cloud servers or complex Kubernetes setups. **HuggingClip** runs the entire [Paperclip](https://paperclip.ing) platform on Hugging Face's **free Docker Space tier** (2 vCPU, 16GB RAM). No credit card, no server management, no Docker experience needed.

```bash
# One click to deploy — that's it.
# 1. Go to: https://huggingface.co/spaces/technicalboy2023/HuggingClip
# 2. Click "Duplicate this Space"
# 3. Add your API key
# Done. Your agents are running.
```

---

## ✨ Features

| Category | Feature | What it means for you |
|----------|---------|----------------------|
| 🤖 **Multi-LLM** | Claude, GPT, Gemini | Pick the best model per task — or use all three |
| ⚡ **One-click Deploy** | Duplicate & run | No config, no CLI, no AWS — just a browser |
| 💾 **Auto Persistence** | HF Dataset backup | PostgreSQL auto-syncs to a private dataset — zero data loss on restart |
| 📊 **Live Dashboard** | Real-time health monitor | See uptime, backup status, plugin count at a glance |
| 🌐 **Cloudflare Proxy** | Bypass network blocks | Automatically routes blocked APIs (Telegram, Discord, etc.) through Cloudflare |
| ⏰ **Keep-Awake Cron** | Auto cron pings | Cloudflare Worker pings your Space every 10 minutes — prevents sleep |
| 🔒 **Secure by Default** | Auto secrets rotation | Randomized passwords, encrypted storage, non-root execution |
| 🏠 **100% HF-Native** | Free tier friendly | Runs entirely on Hugging Face's free infrastructure |

---

## 👥 Who Is This For?

| If you... | HuggingClip is for you |
|-----------|----------------------|
| 🤯 Are tired of paying $20–$200/mo for AI agent hosting | ✅ **Free on HF Spaces** |
| 🔧 Want to use Claude Code without a local machine | ✅ **Browser-based Claude Code** |
| 💼 Need persistent agent workflows that survive restarts | ✅ **Auto backup to HF Dataset** |
| 🌐 Want to connect agents to Telegram, Discord, email | ✅ **Built-in Cloudflare proxy** |
| 🐍 Prefer Python for automation | ✅ **Runs any LLM, any agent** |
| ☁️ Are new to Docker but want AI agents | ✅ **No Docker skills needed** |

---

## 🚀 Quick Start (3 Minutes)

### Step 1: Duplicate the Space

[![Duplicate this Space](https://huggingface.co/datasets/huggingface/badges/resolve/main/duplicate-this-space-xl.svg)](https://huggingface.co/spaces/technicalboy2023/HuggingClip?duplicate=true)

### Step 2: Add Your API Key

In your Space's **Settings → Variables and secrets**, add one (or more) of these:

| Secret | Provider | Get Your Key |
|--------|----------|-------------|
| `ANTHROPIC_API_KEY` | **Claude** (Anthropic) | [console.anthropic.com](https://console.anthropic.com) |
| `GEMINI_API_KEY` | **Gemini** (Google) | [ai.google.dev](https://ai.google.dev) |
| `OPENAI_API_KEY` | **GPT** (OpenAI) | [platform.openai.com](https://platform.openai.com) |
| `HF_TOKEN` | **Backup** (HF Dataset) | [huggingface.co/settings/tokens](https://huggingface.co/settings/tokens) |

> [!TIP]
> Always add `HF_TOKEN` for database persistence. Without it, your agents, tasks, and conversations reset on every restart.

### Step 3: Launch

The Space builds automatically (~60s). Open the **Logs** tab, wait for `HuggingClip is ready!`, then visit your Space URL.

### Step 4: Create Admin Account

On first boot, the dashboard shows an admin invite URL. Click it → set up your account → start building agents.

---

## 💡 Use Cases

- **Personal AI Assistant Hub** — One dashboard for Claude, GPT, and Gemini agents
- **Code Review Automation** — Claude Code reviews PRs, writes tests, refactors code
- **Content Workflow** — Gemini drafts, GPT edits, Claude publishes
- **DevOps Agent** — Monitor logs, restart services, respond to alerts
- **Research Pipeline** — Web research → summarization → report generation
- **Social Media Bot** — Auto-post to Telegram, Discord, Twitter via Cloudflare proxy

---

## 🔑 Configuration Reference

### Secrets (Set in HF Space Settings)

| Variable | Required? | Default | Description |
|----------|-----------|---------|-------------|
| `ANTHROPIC_API_KEY` | No* | — | Claude API key — enables Claude Code agents |
| `GEMINI_API_KEY` | No* | — | Google Gemini API key |
| `OPENAI_API_KEY` | No* | — | OpenAI API key for GPT agents |
| `HF_TOKEN` | No | — | HF write token — enables database backup persistence |
| `CLAUDE_CODE_OAUTH_TOKEN` | No | — | Long-lived Claude OAuth token (1 year, no per-token cost) |
| `CLOUDFLARE_WORKERS_TOKEN` | No | — | Auto-creates proxy + keep-awake workers |

*\*At least one LLM key required for agents to work.*

### Environment Variables

| Variable | Default | Description |
|----------|---------|-------------|
| `PAPERCLIP_DEPLOYMENT_MODE` | `authenticated` | `authenticated` or `local` |
| `BACKUP_DATASET_NAME` | `huggingclip-backup` | HF Dataset name for backups |
| `SYNC_INTERVAL` | `3600` | Backup interval in seconds |
| `SYNC_MAX_FILE_BYTES` | `52428800` | Max backup size (50MB) |
| `BETTER_AUTH_SECRET` | auto-generated | Auth secret (auto-persisted) |

---

## 🏗️ Architecture

```
┌──────────────┐    Port 7861     ┌──────────────────┐
│   Browser    │ ──────────────►  │  health-server.js │
│  (Dashboard) │                  │  (Dashboard +     │
└──────────────┘                  │   Reverse Proxy)  │
                                  └───────┬──────────┘
                                          │ proxy
                                          ▼
                                  ┌──────────────────┐
                                  │   Paperclip App   │  Port 3100
                                  │  (Agent Engine)   │
                                  └───────┬──────────┘
                                          │
                  ┌───────────────────────┼───────────────────────┐
                  ▼                       ▼                       ▼
          ┌──────────────┐      ┌──────────────────┐     ┌──────────────┐
          │  PostgreSQL   │      │  HF Dataset       │     │  Cloudflare   │
          │  (Embedded)   │◄────►│  (Backup/Restore) │     │  Worker(s)    │
          └──────────────┘      └──────────────────┘     │  (Proxy +     │
                                                         │   KeepAlive)  │
                                                         └──────────────┘
```

### Startup Flow

```
1. Validate LLM keys ─► 2. Start PostgreSQL ─► 3. Restore backup from HF Dataset
4. Start sync loop ──► 5. Launch health server (7861) ──► 6. Generate config
7. Launch Paperclip (3100) ──► 8. Bootstrap admin ──► 9. Ready!
```

---

## 🛠️ Local Development

```bash
git clone https://github.com/technicalboy2023/spaceclip.git
cd spaceclip
cp .env.example .env
# Edit .env with your API keys

# Option A: Docker
docker build -t spaceclip .
docker run -p 7861:7861 -e HF_TOKEN=hf_xxxx spaceclip

# Option B: Docker Compose
docker-compose up -d
# Dashboard: http://localhost:7861/
```

---

## 🌐 Cloudflare Integration (Optional)

Hugging Face Spaces blocks some outbound connections. HuggingClip auto-provisions Cloudflare Workers to solve this:

| Worker | Purpose | Cron |
|--------|---------|------|
| **Proxy Worker** | Routes blocked API traffic through Cloudflare | On-demand |
| **KeepAlive Worker** | Pings `/health` every 10 min to prevent Space sleep | `*/10 * * * *` |

**Setup:** Add `CLOUDFLARE_WORKERS_TOKEN` as a Space secret. Everything else is automatic.

Proxied domains by default: Telegram, Discord, WhatsApp, Facebook, Twitter/X, LinkedIn, TikTok, Reddit, OpenAI, SendGrid, Google APIs.

---

## 🔍 Troubleshooting

| Problem | Solution |
|---------|----------|
| ❌ Agents don't run | Add at least one LLM API key to Space secrets |
| 🔄 Data lost on restart | Set `HF_TOKEN` — backup must run once before restart |
| 😴 Space keeps sleeping | Add `CLOUDFLARE_WORKERS_TOKEN` for auto keep-awake |
| ⚠️ 502 errors on dashboard | Wait 60–90s for Paperclip to finish booting |
| 📦 Backup too large | Increase `SYNC_MAX_FILE_BYTES` or archive old agent runs |
| 🐢 Sync not running | Verify `HF_TOKEN` is valid and has write permissions |

---

## 📈 Project Status

**Current:** Active development — deploying Paperclip v1 on HF Spaces.

**Planned:**
- 🔄 Multi-Space federation
- 📦 Backup versioning
- 📊 Prometheus/Grafana monitoring
- 🐳 Kubernetes manifests

---

## ❤️ Support

If SpaceClip saves you time, consider buying me a coffee!

**BEP-20 (Binance Smart Chain)**

```
0xe8b80722fc68c66248b68f31f3e4af9c126766bc
```

> [!WARNING]
> Send **BEP-20 tokens only**. Other networks will result in permanent loss.

---

## 📚 Links

- **[Paperclip Docs](https://paperclip.ing)** — Platform documentation
- **[Paperclip GitHub](https://github.com/paperclipai/paperclip)** — Upstream project
- **[HuggingFace Spaces](https://huggingface.co/docs/hub/spaces)** — HF Spaces guide
- **[HF Token Setup](https://huggingface.co/settings/tokens)** — Get your API token
- **[Cloudflare API Tokens](https://dash.cloudflare.com/profile/api-tokens)** — For proxy + keep-awake

---

## 🤝 Contributing

Contributions are welcome! Check [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

## 📄 License

MIT — see [LICENSE](LICENSE) for details.

*Made with ❤️ by [@technicalboy2023](https://github.com/technicalboy2023) for the Paperclip community.*