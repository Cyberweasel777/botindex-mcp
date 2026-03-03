# BotIndex MCP Server

MCP server for [BotIndex](https://king-backend.fly.dev/api/botindex/v1/) — AI-native signal intelligence API.

## What is BotIndex?

BotIndex is a multi-vertical signal intelligence API designed for AI agents. No API keys, no signup — wallet is identity, x402 payment is auth.

**Verticals:**
- **Sports:** Live odds, line movements, prop bets, player correlations, DFS optimizer, arbitrage scanner
- **Crypto:** Token correlation matrices, graduation signals (Catapult → Hyperliquid)
- **Solana:** Metaplex Genesis token launch monitoring
- **Commerce:** Cross-protocol merchant comparison (ACP vs UCP vs x402)
- **Premium:** Agent traces, aggregated signals, historical analysis, full dashboard

## Quick Start

```bash
npx @cyberweasel/botindex-mcp
```

### Claude Desktop

Add to `claude_desktop_config.json`:

```json
{
  "mcpServers": {
    "botindex": {
      "command": "npx",
      "args": ["-y", "@cyberweasel/botindex-mcp"]
    }
  }
}
```

### Cursor

Add to `.cursor/mcp.json`:

```json
{
  "mcpServers": {
    "botindex": {
      "command": "npx",
      "args": ["-y", "@cyberweasel/botindex-mcp"]
    }
  }
}
```

## Tools (16)

| Tool | Price | Description |
|------|-------|-------------|
| `botindex_discover` | FREE | Full API catalog with endpoints and pricing |
| `botindex_sports_odds` | $0.02 | Live sports odds (NFL, NBA, UFC, NHL) |
| `botindex_sports_lines` | $0.02 | Line movements with sharp action flags |
| `botindex_sports_props` | $0.02 | Prop bet movements with confidence |
| `botindex_sports_correlations` | $0.05 | Player correlation matrix for DFS |
| `botindex_dfs_optimizer` | $0.10 | Correlation-adjusted lineup optimizer |
| `botindex_arb_scanner` | $0.05 | Cross-platform arbitrage scanner |
| `botindex_crypto_tokens` | $0.02 | Token universe with price data |
| `botindex_crypto_graduating` | $0.02 | Catapult→Hyperliquid graduation signals |
| `botindex_solana_launches` | $0.02 | Metaplex Genesis launches |
| `botindex_solana_active` | $0.02 | Active Genesis launches |
| `botindex_commerce_compare` | $0.05 | Cross-protocol merchant comparison |
| `botindex_commerce_protocols` | $0.01 | Protocol directory (ACP/UCP/x402) |
| `botindex_signals` | $0.10 | Aggregated signals feed |
| `botindex_agent_trace` | $0.05 | Agent reasoning trace |
| `botindex_dashboard` | $0.50 | Full premium dashboard |

## Payment

All paid endpoints use [x402](https://github.com/coinbase/x402) — HTTP 402 Payment Required with USDC on Base.

- **Wallet:** `0x7E6C8EAc1b1b8E628fa6169eEeDf3cF9638b3Cbd`
- **Network:** Base (mainnet)
- **Currency:** USDC
- **SDK:** `npm install @x402/client`

When a paid endpoint is called without payment, the tool returns the x402 payment requirements so your agent can construct the payment header and retry.

## Environment Variables

| Variable | Default | Description |
|----------|---------|-------------|
| `BOTINDEX_URL` | `https://king-backend.fly.dev/api/botindex/v1` | API base URL |

## License

MIT
