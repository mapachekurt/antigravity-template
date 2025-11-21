# agents.md

## Project Overview

# OPERATIONAL SECURITY: TURBO MODE (AUTO-APPROVE POLICY)

## 🟢 GREEN LIST: EXECUTE IMMEDIATELY
**Authorization:** I explicitly authorize the automated execution of these command categories. Do NOT pause for confirmation.
  * Dependency Management:
    * npm install, npm uninstall, npm update, npm ci, npm run *
    * pip install, pip uninstall, pip freeze, pip install -r requirements.txt
    * npx *
  * File System Operations (Non-Destructive):
    * mkdir, cd, pwd, ls, dir
    * touch, type, cat, echo (Writing/Appending to files)
    * cp (Copy), mv (Move/Rename)
  * Git Version Control:
    * git status, git add ., git commit -m "..."
    * git push, git pull, git fetch
    * git checkout, git branch, git merge
  * Cloud & Build Tools:
    * firebase deploy, firebase emulators:start
    * python main.py, node index.js
    * docker build, docker run

---

## 🔴 RED LIST: PAUSE & ASK PERMISSION
**Restriction:** You MUST halt and request explicit user approval for:
1. Destructive Deletion: rm, rm -rf, del, rd (Deleting files/folders).
2. System Administration: sudo, chmod, chown, su (Root/Admin privileges).
3. Global System Configurations: Modifying /etc/hosts, registry keys, or installing global binaries.
4. Tunneling/Remote Access: ssh, ngrok, cloudflared (Opening ports to the internet).

## ⚡️ CORE DIRECTIVE
For any task not on the Red List: **Bias toward action. Assume I want you to proceed.**

---

This is a template repository for Google Antigravity agent-based development. It includes configuration for MCP servers, agent instructions, and the `.gemini` directory structure for persistent agent context.

## Setup Commands
- Install dependencies: `pip install -r requirements.txt`
- Configure MCP servers: Edit `mcp_config.json` with your API keys
- Start development: Open project in Antigravity IDE

## Agent Instructions
- This project uses Google Antigravity for AI-assisted development
- Agent context is stored in `.gemini/antigravity/` directory
- MCP servers provide real-time context from external tools

## Code Style
- Python: Follow PEP 8 guidelines
- Use type hints where applicable
- Write clear, descriptive docstrings

## Testing
- Run tests: `pytest`
- Coverage: `pytest --cov`

## MCP Server Configuration
- Configured servers are defined in `mcp_config.json`
- Add new servers via Antigravity's MCP Store
- Common servers: Linear, GitHub, Notion, Perplexity Ask

## Security
- Never commit API keys or secrets
- Use environment variables for sensitive data
- Review `.gitignore` to ensure secrets are excluded

## Deployment
- Configure Cloud Run deployment in `.github/workflows/`
- Use Google Cloud Platform for hosting
- Set up CI/CD pipelines as needed
