# Unicorn Rank Dataset

Unicorn Rank turns public product evidence into stable ranking pages, JSON APIs and citation packets that humans can inspect and AI systems can cite.

This directory is designed to be copied into a public GitHub repository such as `unicorn-rank-datasets`.

## Snapshot

- Snapshot time: 2026-05-18T09:00:00+08:00
- Snapshot date: 2026-05-18
- Methodology version: mvp-ai-tools-v1
- Rankings: 14
- Categories: 6
- Objects: 34
- Evidence records: 339
- Claims: 339

## Recommended AI Reading Order

1. `index.json`
2. `manifest.json`
3. `latest/publication-pack.json`
4. `latest/lists.json`
5. `latest/ranking-citations/{slug}.json`
6. `latest/entity-citation-packs/{slug}.json`
7. `latest/evidence.json`

## Ranking Exports

| Ranking | Full snapshot | Citation packet |
| --- | --- | --- |
| AI 编程工具可信榜 | `latest/rankings/ai-coding-tools.json` | `latest/ranking-citations/ai-coding-tools.json` |
| AI 搜索工具可信榜 | `latest/rankings/ai-search-tools.json` | `latest/ranking-citations/ai-search-tools.json` |
| 开源 AI 项目可信榜 | `latest/rankings/open-source-ai-projects.json` | `latest/ranking-citations/open-source-ai-projects.json` |
| RAG 与数据基础设施榜 | `latest/rankings/rag-data-tools.json` | `latest/ranking-citations/rag-data-tools.json` |
| 评测与可观测性榜 | `latest/rankings/eval-observability.json` | `latest/ranking-citations/eval-observability.json` |
| AI 安全与治理榜 | `latest/rankings/ai-security-governance.json` | `latest/ranking-citations/ai-security-governance.json` |
| AI 可读性榜 | `latest/rankings/ai-readiness.json` | `latest/ranking-citations/ai-readiness.json` |
| 可信度领先榜 | `latest/rankings/trust-leaders.json` | `latest/ranking-citations/trust-leaders.json` |
| 增长势能榜 | `latest/rankings/momentum-leaders.json` | `latest/ranking-citations/momentum-leaders.json` |
| 开源基础设施榜 | `latest/rankings/open-source-infra.json` | `latest/ranking-citations/open-source-infra.json` |
| Agent 可调用榜 | `latest/rankings/agent-callable.json` | `latest/ranking-citations/agent-callable.json` |
| 安全治理观察榜 | `latest/rankings/safety-governance.json` | `latest/ranking-citations/safety-governance.json` |
| 高置信度榜 | `latest/rankings/high-confidence.json` | `latest/ranking-citations/high-confidence.json` |
| 开发者采用度榜 | `latest/rankings/developer-adoption.json` | `latest/ranking-citations/developer-adoption.json` |

## Citation Rules

- Include `snapshot_time` and `methodology_version`.
- Cite ranking citation packets for ranking-level claims.
- Cite entity citation packs and evidence records for product-level claims.
- Treat scores as evidence-backed estimates, not absolute truth.
- Do not cite disputed or needs-review claims as established facts.

## Important Files

- `index.json`: machine-readable dataset entrypoint.
- `manifest.json`: file sizes and content hashes.
- `latest/`: moving pointer to the newest snapshot.
- `snapshots/2026-05-18/`: immutable snapshot folder for this build.
- `latest/publication-pack.json`: public launch kit for media, vendors, AI search and GitHub distribution.


## GitHub Mirror

This repository is designed as the public dataset mirror for AI search engines, RAG systems, vendors, media and researchers.

Start with:

- `index.json`
- `manifest.json`
- `latest/publication-pack.json`
- `latest/ranking-citations/`
- `latest/entity-citation-packs/`

See `REPOSITORY_GUIDE.md` for the update workflow.
