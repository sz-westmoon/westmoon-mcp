# MoonClaw MCP plugin

Connects Cursor and Grok Bot to the MoonClaw MCP server at `https://mcp.moonclaw.com/mcp`.

## What it does

- `catalog_search` / `catalog_explain` / `command_schema`: find WestMonth ERP commands and their arguments.
- `invoke_read`: run read-only commands, e.g. `mall.platform-store.shop.list` (shop list).
- `invoke_write_preview` / `invoke_write`: preview a write, then run it with `confirm: true`.

## Sign-in

OAuth via your WestMonth UMC account. The first call opens the UMC login page; no API key needed.

## Install locally for testing

```bash
cp -R . ~/.cursor/plugins/local/moonclaw
```

Then reload Cursor and check the `moonclaw` MCP server under Customize.
