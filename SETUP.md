# Connect Rebel

The Rebel MCP server is already declared in this plugin. After install, authenticate so tools run against your workspace.

Server URL: `https://app.getrebelos.com/mcp`

OAuth binds the connection to the workspace that was active when you signed in. Revoke anytime from Rebel.

## Claude Code

1. Install this plugin (marketplace or `--plugin-dir`).
2. Run `/mcp` and pick **Rebel**.
3. Sign in with your Rebel account in the browser.

If the browser does not open, use the URL Claude Code prints. Re-auth from `/mcp` if the session expires.

## Claude

1. Open **Customize → Connectors**.
2. Add Rebel from the directory once listed, or **Add custom connector** with the server URL above.
3. Connect and sign in.

## Codex / ChatGPT

1. Add Rebel from the Plugins directory once listed, or paste the server URL as a custom MCP connector (ChatGPT: Developer mode).
2. Sign in with your Rebel account when prompted.

## Grok

1. Open grok.com/connectors → New Connector → Custom.
2. Name it Rebel, paste the server URL, sign in.

## Cursor and other MCP clients

```json
{
  "mcpServers": {
    "rebel": {
      "url": "https://app.getrebelos.com/mcp"
    }
  }
}
```

Approve the sign-in prompt when the client connects.

## Check it worked

Ask: "What's my Rebel token balance?" or "Search for people named …".

You need a Rebel account. Search is free; unlocking emails and mobiles spends tokens at the same rates as the app.
