---
name: setup
description: Connect and authenticate the Rebel MCP server. Use when the user installs this plugin, Rebel tools are missing, auth failed, or they ask how to sign in.
---

# Rebel setup

Follow [SETUP.md](../../SETUP.md). Server URL: `https://app.getrebelos.com/mcp`. Plugin repo: `rebelhq/mcp-plugin`.

1. Confirm the Rebel MCP server is enabled in this session.
2. If tools are missing or return auth errors, have the user sign in (Claude Code: `/mcp` → Rebel). Do not ask for API keys — Rebel uses OAuth.
3. After sign-in, call `credit_balance` or `usage_status` to verify the workspace.

If they have no Rebel account, send them to https://getrebelos.com.
