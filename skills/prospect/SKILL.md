---
name: prospect
description: Find B2B people and companies in Rebel, unlock verified emails and mobiles, and save lists. Use when the user wants leads, decision-makers, contact data, or prospect lists.
---

# Prospect with Rebel

Use the Rebel MCP tools. Do not invent people, emails, or phone numbers.

1. Scope first. If the ask is vague, read `rebel://icp/current` and propose that ICP. One clarifying question if needed.
2. `search_people` / `search_companies` — probe at a small limit, then pull a full page. Preview ~5 rows, not the whole page.
3. Unlock only when asked. Call `credit_balance` first. Email and phone spend tokens; a miss is free. Adding someone to a list also unlocks email — confirm that cost first.
4. Never retry `insufficient_credits` or `rate_limited`. Relay the message and the upgrade path on the error.

Present tables as: Name | Title | Company | Country | Email | Phone | LinkedIn. Unlocked values as values; otherwise the word Unlock.
