# Rebel MCP

Remote MCP server: [`https://app.getrebelos.com/mcp`](https://app.getrebelos.com/mcp)

Search people and companies, unlock verified emails and mobiles, and build lists. OAuth binds the connection to your Rebel workspace. Rebel surfaces and enriches data — it does not send.

## Plugins

Installs the MCP server plus skills. Sign in with OAuth on first use.

### Claude Code

```bash
claude plugin marketplace add rebelhq/mcp-plugin
claude plugin install rebel@rebel
```

Then `/mcp` → Rebel → sign in.

### Codex

```bash
codex plugin marketplace add rebelhq/mcp-plugin
codex plugin add rebel@rebel
```

Then `codex mcp login rebel`.

### Cursor

```
/add-plugin rebelhq/mcp-plugin
```

Or add the server URL to `~/.cursor/mcp.json` (below).

### Grok Build

```bash
grok plugin install rebelhq/mcp-plugin --trust
```

## Any MCP client

Use the server URL with streamable HTTP. Sign in when prompted.

```json
{
  "mcpServers": {
    "rebel": {
      "url": "https://app.getrebelos.com/mcp"
    }
  }
}
```

| Client | How |
|---|---|
| Claude | Customize → Connectors → Add custom connector |
| ChatGPT | Settings → Connectors (Developer mode) |
| Grok | grok.com/connectors → Custom |
| Claude Code | `claude mcp add --transport http rebel https://app.getrebelos.com/mcp` |
| Codex CLI | `[mcp_servers.rebel] url = "https://app.getrebelos.com/mcp"` then `codex mcp login rebel` |

## Privacy and terms

- [Privacy](https://getrebelos.com/legal/privacy)
- [Terms](https://getrebelos.com/legal/terms)
- Support: hello@getrebelos.com
