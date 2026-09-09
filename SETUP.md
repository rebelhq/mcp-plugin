# Connect Rebel

Server URL: `https://app.getrebelos.com/mcp`

OAuth binds the connection to the workspace that was active when you signed in. Revoke anytime from Rebel.

## Plugins

```bash
claude plugin marketplace add rebelhq/mcp-plugin && claude plugin install rebel@rebel
codex plugin marketplace add rebelhq/mcp-plugin && codex plugin add rebel@rebel
grok plugin install rebelhq/mcp-plugin --trust
```

Then sign in: Claude Code `/mcp` → Rebel · Codex `codex mcp login rebel` · Grok on first tool call.

## MCP URL only

Paste `https://app.getrebelos.com/mcp` into the client’s custom connector settings, or:

```bash
claude mcp add --transport http rebel https://app.getrebelos.com/mcp
```

```toml
[mcp_servers.rebel]
url = "https://app.getrebelos.com/mcp"
```

```json
{
  "mcpServers": {
    "rebel": {
      "url": "https://app.getrebelos.com/mcp"
    }
  }
}
```

Claude: Customize → Connectors → Add custom connector.  
ChatGPT: Settings → Connectors (Developer mode).  
Grok: grok.com/connectors → Custom.

## Check it worked

Ask: "What's my Rebel token balance?"

You need a Rebel account. Search is free; unlocking emails and mobiles spends tokens at the same rates as the app.
