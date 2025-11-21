# antigravity-template

Template repository for Google Antigravity agent-based development with `agents.md`, MCP configuration, and `.gemini` directory structure.

## Overview

This template provides a complete setup for Google Antigravity projects, including:

- **agents.md** - Universal agent instructions compatible with 20k+ projects (Cursor, VS Code, Codex, Aider, etc.)
- **GEMINI.md** - Gemini/Antigravity-specific agent instructions
- **mcp_config.json** - MCP (Model Context Protocol) server configurations
- **.gemini/** - Directory for Gemini CLI and Antigravity persistent context
- Python .gitignore and MIT License

## Quick Start

### 1. Use this template
Click "Use this template" → "Create a new repository" to create your own copy.

### 2. Configure MCP Servers

Edit `mcp_config.json` and add your API keys:

```json
{
  "mcpServers": {
    "linear": {
      "env": {
        "LINEAR_API_KEY": "your-key-here"
      }
    }
  }
}
```

### 3. Open in Antigravity

- Download [Google Antigravity](https://antigravity.google)
- Open your new repository in Antigravity
- MCP servers will automatically connect
- Agents will read `agents.md` and `GEMINI.md` for instructions

## File Structure

```
.
├── agents.md              # Universal agent instructions
├── GEMINI.md              # Gemini-specific instructions
├── mcp_config.json        # MCP server configurations
├── .gemini/
│   └── settings.json      # Gemini CLI configuration
├── .gitignore             # Python gitignore
├── LICENSE                # MIT License
└── README.md
```

## Key Files Explained

### agents.md vs GEMINI.md

- **agents.md**: Universal format supported by Cursor, VS Code, Codex, Aider, Antigravity, and 20k+ projects
- **GEMINI.md**: Gemini/Antigravity-specific instructions
- **Best practice**: Use both files, or symlink GEMINI.md to agents.md

### mcp_config.json

Configures MCP servers for real-time context:
- **Linear**: Project management integration
- **GitHub**: Repository access
- **Notion**: Documentation integration
- **Perplexity Ask**: Web search capabilities

Add more servers via Antigravity's MCP Store.

### .gemini Directory

- **settings.json**: Configures which context file to use (GEMINI.md)
- **antigravity/**: Storage for Antigravity's persistent agent knowledge

## Supported MCP Servers

- Linear
- GitHub
- Notion
- Perplexity Ask
- Firebase
- MongoDB
- Supabase
- And 20+ more via [MCP Store](https://antigravity.google/docs/mcp)

## Security Notes

⚠️ **Never commit API keys to version control**

- Use environment variables for production
- The template includes placeholder keys - replace them
- Add `.env` files to `.gitignore`

## Resources

- [Antigravity Documentation](https://antigravity.google/docs)
- [MCP Protocol](https://modelcontextprotocol.io)
- [agents.md Standard](https://agents.md)

## License

MIT License - see LICENSE file for details
