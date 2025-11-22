# Antigravity React Template (Sentry-Enabled)

A "Smart Template" for Google Antigravity that auto-configures React, Firebase, and Sentry.

## 🚀 Quick Start (The "One-Shot")

1. Open a new Antigravity Window.
2. Paste this command into the Agent Chat:

> **Agent, bootstrap this project.**
> 1. Initialize a React app using Vite.
> 2. Install `@sentry/react`.
> 3. Read `GEMINI.md` and configure the Sentry SDK immediately.

## 📂 What's Inside?

- **`GEMINI.md`**: The "Brain." Contains the Sentry Protocol and Project Phases.
- **`agents.md`**: The "Team." Defines Architect, Builder, and QA personas.
- **`mcp_config.json`**: Tool configurations for Linear, GitHub, etc.

## 🛠 Configuration

**Sentry Setup:**
1. Copy `.env.example` to `.env`.
2. Add your DSN: `VITE_SENTRY_DSN=https://...`
3. The Agent will handle the rest.

**MCP Servers:**
- Edit `mcp_config.json` to add your API keys (or better, use env vars).
