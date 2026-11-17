# Dadan MCP Server

Official remote MCP server for [Dadan](https://www.dadan.io/dadan-mcp). Record, edit, transcribe, translate and share videos, plus meeting notes and analytics (70 tools).

- **Endpoint:** `https://mcp.dadan.io/mcp`
- **Transport:** Streamable HTTP
- **Auth:** OAuth 2.1, with sign-in in your browser (no API keys)
- **Cost:** free to connect on all Dadan plans, including free

## Install in Cline

Add this to `cline_mcp_settings.json`:

```json
{
  "mcpServers": {
    "dadan": {
      "type": "streamableHttp",
      "url": "https://mcp.dadan.io/mcp"
    }
  }
}
```

The first time a tool runs, a browser window opens so you can sign in to Dadan.

## Other clients

Use the same URL (`https://mcp.dadan.io/mcp`) as a remote/custom MCP server in Claude, ChatGPT, Cursor, VS Code and other MCP clients.

## Install in Windsurf / Devin Desktop

Add this to `.devin/mcp_config.json` (project) or `~/.config/devin/mcp_config.json` (user):

```json
{
  "mcpServers": {
    "dadan": {
      "url": "https://mcp.dadan.io/mcp",
      "transport": "http"
    }
  }
}
```

Sign in to Dadan when prompted (OAuth).

## Links

- Docs: https://www.dadan.io/dadan-mcp
- Website: https://www.dadan.io
