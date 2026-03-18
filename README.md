# BotIndex MCP Server — Crypto Market Intelligence

> **Not another data feed. A convergence intelligence engine.**

MCP server for [BotIndex](https://botindex.dev) — predictive crypto market intelligence synthesized from whale positions, developer activity, and behavioral demand signals.

## Why BotIndex?

Everyone has CoinGecko data. Nobody has this:

- **🧠 Convergence Scoring** — Multi-source signal synthesis (whale + dev + fear alignment)
- **🐋 Whale Divergence Detection** — Smart money loading while retail sells
- **📡 Network Intelligence** — Ecosystem development velocity as a price predictor
- **🔮 Predictive Signals** — DeepSeek-synthesized with [verifiable track record](https://api.botindex.dev/api/botindex/sentinel/track-record)
- **⚡ Query Surge Intelligence** — What 19K+ daily API consumers are searching for
- **🎯 Risk Radar** — One composite number for the market regime

## Quick Start

```bash
npx -y botindex-mcp
```

### Claude Desktop / Cursor

```json
{
  "mcpServers": {
    "botindex": {
      "command": "npx",
      "args": ["-y", "botindex-mcp"],
      "env": { "BOTINDEX_API_KEY": "your_key" }
    }
  }
}
```

Get a key:
```bash
# Free (3 req/day, raw data)
curl "https://api.botindex.dev/api/botindex/keys/register?plan=free"

# Pro Intelligence ($9.99/mo — convergence, risk radar, network intel)
curl "https://api.botindex.dev/api/botindex/keys/register?plan=pro"

# Sentinel ($49.99/mo — predictive signals, query surge, alerts)
curl "https://api.botindex.dev/api/botindex/keys/register?plan=sentinel"
```

## Intelligence Tools

### Pro ($9.99/mo)

| Tool | Description |
|------|-------------|
| `botindex_smart_money_flow` | Whale accumulation + funding rate convergence analysis |
| `botindex_risk_radar` | Composite market risk score with DeepSeek synthesis |
| `botindex_network_rankings` | Ecosystem momentum scores (8 ecosystems) |
| `botindex_query_intelligence` | What API consumers are searching for (teaser) |

### Sentinel ($49.99/mo)

| Tool | Description |
|------|-------------|
| `botindex_sentinel_signals` | Full predictive signal report with narratives |
| `botindex_track_record` | Prediction accuracy — hit rate by asset and signal type |
| `botindex_query_intelligence_full` | Full endpoint-level demand intelligence |
| `botindex_network_intelligence` | Detailed ecosystem scoring with all components |

### Free (3/day)

| Tool | Description |
|------|-------------|
| `botindex_zora_trending` | Zora trending coins |
| `botindex_whale_alerts` | Hyperliquid whale position alerts |
| `botindex_funding_arb` | Funding rate arbitrage opportunities |
| `botindex_correlation_matrix` | Token correlation matrix |
| `botindex_sentinel_status` | Current alert level |

## Coverage

**16 assets:** BTC, ETH, SOL, KAS, STX, ORDI, BABY, HYPE, PURR, ZORA, AAVE, UNI, LINK, ARB, OP, POL

**8 ecosystems scored:** Ethereum, Solana, Uniswap, Hyperliquid, Base, Aave, Zora, Pump.fun

**Refresh:** Signals every 15 min. Divergence scan every 30 min.

## Track Record

Every prediction logged with entry price. Verified at 24h/72h/7d. No cherrypicking.

**→ [View live accuracy](https://api.botindex.dev/api/botindex/sentinel/track-record)**

## Links

- **Landing:** [botindex.dev](https://botindex.dev)
- **API Docs:** [api.botindex.dev](https://api.botindex.dev/api/botindex/sentinel/track-record)
- **GitHub:** [github.com/Cyberweasel777/King-Backend](https://github.com/Cyberweasel777/King-Backend)
- **AAR Trust Layer:** [aar.botindex.dev](https://aar.botindex.dev)

## License

MIT
