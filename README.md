# Jacob Galperin — Node.js / Open Source

> Building open-source tooling for [Linagora](https://linagora.com)'s collaboration stack (Matrix · JMAP · Cozy · LinShare) while contributing upstream to the libraries I use.

---

## Twake Workplace Ecosystem

A full ecosystem of tools built around Linagora's open-source collaboration platform — each project filling a real gap, built from scratch.

| Project | What it does |
|---------|-------------|
| [twake-cli](https://github.com/JacobiusMakes/twake-cli) | Unified CLI for Twake — chat, mail, drive, share from your terminal. Matrix · JMAP · Cozy · LinShare |
| [twake-automate](https://github.com/JacobiusMakes/twake-automate) | Workflow automation engine — event triggers, scheduled jobs, LUCIE AI actions |
| [twake-search](https://github.com/JacobiusMakes/twake-search) | Server-side unified search across Chat + Mail + Drive — SQLite FTS5, REST API |
| [twake-rag](https://github.com/JacobiusMakes/twake-rag) | RAG service for Drive documents — LUCIE LLM · transformers.js · vector embeddings |
| [twake-tui](https://github.com/JacobiusMakes/twake-tui) | Terminal dashboard — real-time chat/mail/drive in one view, built with ink |
| [twake-mcp](https://github.com/JacobiusMakes/twake-mcp) | MCP server — exposes Twake to any AI assistant (Claude, Cursor, etc.) |
| [twake-notify](https://github.com/JacobiusMakes/twake-notify) | Email-to-chat bridge — JMAP inbox alerts posted to Matrix rooms |
| [twake-linto-bridge](https://github.com/JacobiusMakes/twake-linto-bridge) | Voice transcription bridge — LinTO speech-to-text → Twake Chat threaded replies |
| [twake-migrate](https://github.com/JacobiusMakes/twake-migrate) | Migration tool — Slack → Matrix, Google Workspace → JMAP/Cozy |
| [twake-dashboard](https://github.com/JacobiusMakes/twake-dashboard) | Web search UI — visual frontend for twake-search with demo mode, source filtering |

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

### Hugging Face

| PR | Repo | Description |
|----|------|-------------|
| [#1609](https://github.com/huggingface/transformers.js/pull/1609) | transformers.js | `feat`: emit `progress_total` events from `PreTrainedModel.from_pretrained()` — aggregate download progress for multi-file models |

### ffmpeg.wasm

| PR | Repo | Description |
|----|------|-------------|
| [#938](https://github.com/ffmpegwasm/ffmpeg.wasm/pull/938) | ffmpeg.wasm | `fix`: AbortSignal actually cancels running WASM exec via `setTimeout(1)` — resolves #719 |
| [#936](https://github.com/ffmpegwasm/ffmpeg.wasm/pull/936) | ffmpeg.wasm | `feat`: restore Node.js support via `worker_threads` — mirrors browser API, resolves #897 |
| [#937](https://github.com/ffmpegwasm/ffmpeg.wasm/pull/937) | ffmpeg.wasm | `feat`: allow passing binary WASM data directly to `FFmpeg.load()` — no CDN required |

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
