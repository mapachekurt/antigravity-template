# Antigravity React Template (Sentry-Enabled)

A "Smart Template" for Google Antigravity that auto-configures React, Firebase, and Sentry.

## 🚀 Quick Start

### Option A: New Project (React/Vite)
1. Open a new Antigravity Window.
2. Paste this command into the Agent Chat:

> **Agent, bootstrap this project.**
> 1. Initialize a React app using Vite.
> 2. Install `@sentry/react`.
> 3. Read `GEMINI.md` and configure the Sentry SDK immediately.

### Option B: Existing Project (Any Language)
*Use this when you open an existing folder (like `mapachev1`) and want to add Antigravity powers.*

1. Open your existing project.
2. Paste this command into the Agent Chat:

> **Agent, apply the Antigravity Template to this project.**
> 1. Read `GEMINI.md`, `agents.md`, and `mcp_config.json` from my local template repo at:
>    `c:\Users\Kurt Anderson\github projects\antigravity\antigravity-template\`
> 2. Copy these files to the root of my current workspace.
> 3. Create a `.env` file from the template's `.env.example` (if I don't have one).
> 4. Update `.gitignore` to respect these new files.

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
