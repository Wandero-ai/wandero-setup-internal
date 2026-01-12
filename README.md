# Wandero Setup

Setup instructions for AI coding agents (Windsurf, Cursor, Claude Code, etc.)

## Usage

Paste this repo URL into your AI agent to set up Wandero:

```
https://github.com/Wandero-ai/wandero-setup-internal
```

The agent will read [AGENTS.md](AGENTS.md) and clone the appropriate repos based on your GitHub permissions.

## What Gets Cloned

```bash
git clone --recurse-submodules https://github.com/Wandero-ai/wandero.git
```

| Your Access | What You See |
|-------------|--------------|
| Everyone | `wandero/` — overviews, public docs |
| Team | `wandero/team/` — processes, playbooks |
| Admin | `wandero/team/admin/` — records, financials |
