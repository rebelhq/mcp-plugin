# Rebel MCP plugin

Official Rebel MCP plugin. Search people and companies, unlock verified emails and mobiles, and build lists from Claude, Codex, Grok, or any MCP client.

This repo is the public wrapper. The server lives at [`https://app.getrebelos.com/mcp`](https://app.getrebelos.com/mcp).

## Install

### Claude Code

```bash
claude plugin marketplace add itsrobinwhite/mcp-plugin
claude plugin install rebel@rebel
```

Then `/mcp` → Rebel → sign in.

### Any MCP client

Paste the server URL and sign in with OAuth:

```
https://app.getrebelos.com/mcp
```

Signed-in setup guide: [app.getrebelos.com/mcp/setup](https://app.getrebelos.com/mcp/setup).

## What it does

- Search people and companies
- Unlock verified emails and mobiles (tokens, same rates as the app; misses are free)
- Brief a contact, check balance and daily allowance
- Create and fill lists

Rebel surfaces and enriches data. It does not send outreach.

## Privacy and terms

- [Privacy](https://getrebelos.com/legal/privacy)
- [Terms](https://getrebelos.com/legal/terms)
- Support: hello@getrebelos.com
