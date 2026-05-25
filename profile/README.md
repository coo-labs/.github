# coo-labs

coo-labs is the home for **VADE** — a Visual Agent-based Development Environment under construction — and the operational substrate around it. The org structure follows a three-tier framework that distinguishes substrate from product.

## Three-tier framework

**Tier 1 — substrate / OS** *(`coo-*` prefix reserved for this instance)*
Repos the COO agent runs on day-to-day: identity, kernel, logs, dev surface. Other instances of the same pattern would take their own prefix.

**Tier 2 — OSS products** *(short direct names)*
Releasable artifacts useful to the broader Claude Code / agent-substrate community. Versioned, installable.

**Tier 3 — in-development apps / services** *(deployment-derived names)*
Long-range product expression toward a deployed canvas IDE and its public-facing surfaces.

## Repositories

| Repo | Tier | Visibility | Role |
|---|---|---|---|
| [coo-memory](https://github.com/coo-labs/coo-memory) | 1 (substrate) | Private | Canonical identity + memory store: charter, governance, preferences, identity layer, memos, foundations, retrospectives, lineage events, audits, ops docs. The COO's durable record. |
| [coo-harness](https://github.com/coo-labs/coo-harness) | 1 (substrate) | Public | Boot orchestration: SessionStart hooks, integrity checks, MCP projection, PAT routing, session lifecycle, transcript export. The COO's kernel. |
| [coo-logs](https://github.com/coo-labs/coo-logs) | 1 (substrate) | Private | Append-only audit trail: session summaries, transcript sidecars (raw transcripts live in R2), incidents, billing, telemetry. The COO's OS-logs record. |
| [coo-console](https://github.com/coo-labs/coo-console) | 1 (substrate) | Private | Hosted multi-tool dev/observability surface. Currently in development, baked for our needs; visibility flips or splits when ready. |
| [tjsonl](https://github.com/coo-labs/tjsonl) | 2 (OSS) | Public | Community schema spec for Claude Code transcript format + zero-dependency Python CLI. |
| [skills](https://github.com/coo-labs/skills) | 2 (OSS) | Public | Portable Claude Code skills + sub-agent definitions. |
| [coo4one](https://github.com/coo-labs/coo4one) | 2 (OSS) | Public | Apple-native COO architecture as personal-assistant system. |
| [vade-canvas](https://github.com/coo-labs/vade-canvas) | 3 (in-dev) | Public | The canvas: tldraw + React SPA + MCP bridge + Cloudflare Worker. The visual-agent-society IDE. |
| [site](https://github.com/coo-labs/site) | 3 (in-dev) | Public | Public-facing rendered HTML projected from `coo-memory` via Quarto. Deployed at [read.vade-app.dev](https://read.vade-app.dev). |

## License

Per-repo. Each repo declares its own LICENSE. OSS products (Tier 2) are MIT-style; substrate repos vary.

## Read more

- Public-facing reader: [read.vade-app.dev](https://read.vade-app.dev) — foundations, retrospectives, and lineage essays curated from `coo-memory`.

---

*Machine-readable canonical: [`repos.yaml`](https://github.com/coo-labs/.github/blob/main/repos.yaml) in this repo. The table above is the human view; workflows and scripts should derive structural metadata (tier, visibility, status, deployment domain) from `repos.yaml` directly to avoid drift.*
