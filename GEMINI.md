# GEMINI.md - Gemini-Specific Agent Instructions

This file contains agent instructions specific to Google Gemini/Antigravity environments.

## Context
This template is designed for Google Antigravity agent-first development with MCP integration.

## Agent Behavior
- Use Gemini 3 Pro for complex reasoning tasks
- Leverage MCP servers for real-time context
- Store persistent knowledge in `.gemini/antigravity/` directory
- Follow agents.md for general project guidelines

## Gemini CLI Configuration
To use this file with Gemini CLI, add to `.gemini/settings.json`:
```json
{
  "contextFileName": "GEMINI.md"
}
```

## Notes
- This file can be a symlink to agents.md if instructions are identical
- Keep Gemini-specific instructions here, universal agent instructions in agents.md
