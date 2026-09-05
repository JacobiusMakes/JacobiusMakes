# Jacob Galperin - Node.js / Open Source

> Building open-source tooling for [Linagora](https://linagora.com)'s collaboration stack (Matrix · JMAP · Cozy · LinShare) while contributing upstream to the libraries I use.

---

## ParlayAPI: real-time sports odds for developers and AI agents

[ParlayAPI](https://parlay-api.com) is a real-time sports odds API I built and run: 30+ sportsbooks, 90+ sport keys, player props, arbitrage detection, prediction markets, and closing lines with continuous history from 2005. The free tier is 1,000 credits per month, no card required, and the keyless demo endpoint (`GET https://parlay-api.com/v1/try/{sport}/odds`) needs no account at all. Start with the [docs](https://parlay-api.com/docs), [pricing](https://parlay-api.com/pricing), or the [MCP page](https://parlay-api.com/mcp).

Everything below is open source and works with the free tier.

**For agent builders**

| Repo | What it gives you |
|------|-------------------|
| [parlayapi-betting-agent-starter](https://github.com/JacobiusMakes/parlayapi-betting-agent-starter) | The "how do I start" repo: live odds to no-vig fair lines, one marked hole for your model. One click in Colab or Codespaces, keyless |
| [parlay-api-mcp](https://github.com/JacobiusMakes/parlay-api-mcp) | MCP server: live odds, props, and arbitrage as 22 tools in Claude, Cursor, or any MCP client. Hosted endpoint, no install: `POST https://parlay-api.com/mcp/http` |
| [parlayapi-agent-tools](https://github.com/JacobiusMakes/parlayapi-agent-tools) | Ready made odds tools for LangChain, LlamaIndex, and raw OpenAI/Anthropic function calling |
| [parlayapi-betting-agent-starter](https://github.com/JacobiusMakes/parlayapi-betting-agent-starter) | Betting agent starter: live moneylines in, no-vig fair lines out, one marked hole where your model goes. Runs keyless in Colab, Codespaces, or one git clone |

**For data people**

| Repo | What it gives you |
|------|-------------------|
| [sports-odds-datasets](https://github.com/JacobiusMakes/sports-odds-datasets) | Free datasets of real sportsbook closing lines, exported from production. CC BY 4.0 |
| [parlayapi-notebooks](https://github.com/JacobiusMakes/parlayapi-notebooks) | Jupyter notebooks: no-vig pricing, EV, line movement, closing line value. One click Open in Colab |
| [betting-model-starter](https://github.com/JacobiusMakes/betting-model-starter) | Template for a betting model: fetch odds and props, devig, scan edges, backtest closing line value |
| [parlayapiR](https://github.com/JacobiusMakes/parlayapiR) | R client with devigging and Kelly sizing, keyless sandbox mode |
| [awesome-sports-betting-data](https://github.com/JacobiusMakes/awesome-sports-betting-data) | Curated map of the whole space: odds APIs, historical datasets, tools, communities |

**For integrators**

| Repo | What it gives you |
|------|-------------------|
| [parlay-api-python](https://github.com/JacobiusMakes/parlay-api-python) | Python SDK: `pip install parlay-api` |
| [parlay-api-js](https://github.com/JacobiusMakes/parlay-api-js) | JavaScript/TypeScript SDK, zero dependencies |
| [parlayapi-collections](https://github.com/JacobiusMakes/parlayapi-collections) | Ready-to-import collections for Bruno, Postman, Insomnia, and HTTPie |
| [parlayapi-odds-action](https://github.com/JacobiusMakes/parlayapi-odds-action) | GitHub Action that pulls odds into JSON or CSV on a cron |
| [parlayapi-sheets](https://github.com/JacobiusMakes/parlayapi-sheets) | Live odds, line shopping, and devig as Google Sheets formulas |
| [parlayapi-discord-bot](https://github.com/JacobiusMakes/parlayapi-discord-bot) | Self-hostable Discord bot: lines, moves, and a parlay checker |
| [parlayapi-raycast](https://github.com/JacobiusMakes/parlayapi-raycast) | Raycast extension: best available lines and betting math from your launcher |
| [parlayapi-obs-overlay](https://github.com/JacobiusMakes/parlayapi-obs-overlay) | OBS best-line ticker for betting streamers, one HTML file, keyless |
| [parlayapi-line-shopper](https://github.com/JacobiusMakes/parlayapi-line-shopper) | Shop the line from your terminal: every book's price per outcome |
| [parlayapi-arb-scanner](https://github.com/JacobiusMakes/parlayapi-arb-scanner) | CLI arbitrage scanner, zero setup against keyless sandbox endpoints |
| [parlay-api-arb-starter](https://github.com/JacobiusMakes/parlay-api-arb-starter) | Cross-book arbitrage in under 150 lines of Python |

Skeptics welcome: [odds-api-benchmarks](https://github.com/JacobiusMakes/odds-api-benchmarks) lets you rerun every published comparison number from your own machine, and [parlayapi-data-bounty](https://github.com/JacobiusMakes/parlayapi-data-bounty) pays free credits when you catch us serving a wrong line.

---

## Twake Workplace Ecosystem

A full ecosystem of tools built around Linagora's open-source collaboration platform - each project filling a real gap, built from scratch.

| Project | What it does |
|---------|-------------|
| [twake-cli](https://github.com/JacobiusMakes/twake-cli) | Unified CLI for Twake - chat, mail, drive, share from your terminal. Matrix · JMAP · Cozy · LinShare |
| [twake-automate](https://github.com/JacobiusMakes/twake-automate) | Workflow automation engine - event triggers, scheduled jobs, LUCIE AI actions |
| [twake-search](https://github.com/JacobiusMakes/twake-search) | Server-side unified search across Chat + Mail + Drive - SQLite FTS5, REST API |
| [twake-rag](https://github.com/JacobiusMakes/twake-rag) | RAG service for Drive documents - LUCIE LLM · transformers.js · vector embeddings |
| [twake-tui](https://github.com/JacobiusMakes/twake-tui) | Terminal dashboard - real-time chat/mail/drive in one view, built with ink |
| [twake-mcp](https://github.com/JacobiusMakes/twake-mcp) | MCP server - exposes Twake to any AI assistant (Claude, Cursor, etc.) |
| [twake-notify](https://github.com/JacobiusMakes/twake-notify) | Email-to-chat bridge - JMAP inbox alerts posted to Matrix rooms |
| [twake-linto-bridge](https://github.com/JacobiusMakes/twake-linto-bridge) | Voice transcription bridge - LinTO speech-to-text → Twake Chat threaded replies |
| [twake-migrate](https://github.com/JacobiusMakes/twake-migrate) | Migration tool - Slack → Matrix, Google Workspace → JMAP/Cozy |
| [twake-dashboard](https://github.com/JacobiusMakes/twake-dashboard) | Web search UI - visual frontend for twake-search with demo mode, source filtering |
| [twake-monitor](https://github.com/JacobiusMakes/twake-monitor) | Health check + uptime monitor - probes 5 real Twake endpoints, Prometheus metrics, TLS cert expiry |

---

## Open Source Contributions

### Linagora

| PR | Repo | Description |
|----|------|-------------|
| [#925](https://github.com/linagora/twake-drive-legacy/pull/925) | twake-drive-legacy | `fix(database)`: PostgreSQL auto-reconnect with exponential backoff |
| [#924](https://github.com/linagora/twake-drive-legacy/pull/924) | twake-drive-legacy | `fix(postgres)`: empty SET clause crash in upsertOne |
| [#923](https://github.com/linagora/twake-drive-legacy/pull/923) | twake-drive-legacy | `fix(i18n)`: missing Russian translations |
| [#922](https://github.com/linagora/twake-drive-legacy/pull/922) | twake-drive-legacy | `fix(i18n)`: sidebar language mixup race condition on first load |
| [#921](https://github.com/linagora/twake-drive-legacy/pull/921) | twake-drive-legacy | `refactor`: consolidate email templates with i18n |
| [#920](https://github.com/linagora/twake-drive-legacy/pull/920) | twake-drive-legacy | `fix`: NaN date display in file browser |
| [#919](https://github.com/linagora/twake-drive-legacy/pull/919) | twake-drive-legacy | `fix`: password visible as plaintext on shared link input |
| [#78](https://github.com/linagora/jmap-client-ts/pull/78) | jmap-client-ts | `fix`: upgrade axios + node-fetch to resolve 4 high-severity CVEs |
| [#349](https://github.com/linagora/ToM-server/pull/349) | ToM-server | `fix`: graceful fallback when LDAP URI is missing - prevents server crash on startup |
| [#722](https://github.com/linagora/twake-calendar-frontend/pull/722) | twake-calendar-frontend | `fix`: type-safe window config replacing `(window as any)` globals |

### Hugging Face

| PR | Repo | Description |
|----|------|-------------|
| [#1609](https://github.com/huggingface/transformers.js/pull/1609) | transformers.js | `feat`: emit `progress_total` events from `PreTrainedModel.from_pretrained()` - aggregate download progress for multi-file models |

### ffmpeg.wasm

| PR | Repo | Description |
|----|------|-------------|
| [#938](https://github.com/ffmpegwasm/ffmpeg.wasm/pull/938) | ffmpeg.wasm | `fix`: AbortSignal actually cancels running WASM exec via `setTimeout(1)` - resolves #719 |
| [#936](https://github.com/ffmpegwasm/ffmpeg.wasm/pull/936) | ffmpeg.wasm | `feat`: restore Node.js support via `worker_threads` - mirrors browser API, resolves #897 |
| [#937](https://github.com/ffmpegwasm/ffmpeg.wasm/pull/937) | ffmpeg.wasm | `feat`: allow passing binary WASM data directly to `FFmpeg.load()` - no CDN required |

### Scaleway

| PR | Repo | Description |
|----|------|-------------|
| [#2860](https://github.com/scaleway/scaleway-sdk-js/pull/2860) | scaleway-sdk-js | `feat`: async config loading + file permission security check |

### Mistral AI

| PR | Repo | Description |
|----|------|-------------|
| [#200](https://github.com/mistralai/client-ts/pull/200) | client-ts | `fix`: graceful handling of malformed JSON in structured output parsing |

---

## Stack

```
Node.js · TypeScript · Fastify · Commander.js · SQLite FTS5
Matrix (m.room.message) · JMAP (RFC 8621) · Cozy API (JSON:API) · OAuth2/PKCE/OIDC
ink (React for terminal) · transformers.js · ffmpeg.wasm · better-sqlite3
```

---

*Based in Atlanta → moving to Paris. Open to R&D Node.js roles.*
