# agents.md

## Project Overview
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
