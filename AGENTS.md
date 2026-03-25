# AGENTS.md

## Purpose
This repository holds organization-wide community health files for `cubrid-labs`.

## Read First
- `README.md`
- `CONTRIBUTING.md`
- `SECURITY.md`
- `SUPPORT.md`
- `docs/agent-playbook.md`

## Working Rules
- Treat this repo as policy and template infrastructure, not product code.
- Keep contributor-facing guidance consistent across files.
- When behavior or policy changes, update every affected document in the same change.
- Prefer small edits that preserve existing wording unless a policy change is intentional.

## Validation
- Manually review Markdown rendering and link targets.
- If examples or command snippets change, verify they still match current org conventions.

## Competition Context (공모전 — Performance Loop System)

> **Timeline**: 2026-03-25 ~ 2026-11-04
> **Board**: [CUBRID Ecosystem Roadmap](https://github.com/orgs/cubrid-labs/projects/2)

### What This Is

A Korean open-source competition project that proves a **continuous Performance Loop**:
benchmark → profile → optimize driver/ORM → re-benchmark → CI-verified regression prevention.

### Core Repos (공모전 범위)

| Repo | Role | Current State |
|------|------|---------------|
| `cubrid-benchmark` | Benchmark suite (Python/TS/Go × CUBRID/MySQL) | Tier 0+1+Extended, CI, GitHub Pages — **most mature** |
| `pycubrid` | Python driver (PEP 249) | v0.5.0, published PyPI — **4.5-6× slower than MySQL, optimization not started** |
| `sqlalchemy-cubrid` | SQLAlchemy 2.0 dialect | v2.1.1, published PyPI — **ORM optimization not started** |
| `cubrid-cookbook` | Runnable examples across all languages | Broad coverage — **expected outputs not standardized** |

### Supporting Repos (에코시스템 증거, 공모전 핵심 범위 아님)

`cubrid-client` (TS, v1.1.0), `cubrid-go`, `cubrid-rs`, `drizzle-cubrid`, `gorm-cubrid`, `sea-orm-cubrid`

### Execution Phases

| Phase | Period | Focus |
|-------|--------|-------|
| R0: Baseline Reset | Week 1-2 | Scope reset, baseline recording, plan rewrite |
| R1: Measurement | Week 3-5 | Tier 2 ORM benchmarks, reproducibility policy |
| R2: Python Optimization | Week 6-10 | pycubrid profiling, serialization + cursor fetch optimization |
| R3: ORM Validation | Week 11-14 | sqlalchemy-cubrid optimization, 2nd pycubrid cycle |
| R4: Stability | Week 15-18 | cubrid-client resilience (nice-to-have) |
| R5: CI & Regression | Week 19-22 | Compare script, cookbook standardization |
| R6: Competition | Week 23-32 | Evidence pack, demo, submission |

### Hero Metric

**Python driver MySQL 대비 성능 갭 감소** — before/after 수치가 공모전 핵심 스토리.

### Decision Gate (Week 8)

pycubrid 최적화 결과 +10% 이상이면 계속, 미만이면 Go/TS 성과 중심으로 내러티브 피벗.

### Competition Narrative

"Build Once, Improve Continuously" — 매일 밤 자동 벤치마크, PR마다 회귀 감지, 재현 가능한 one-command 데모.

### Must-Have Deliverables

1. pycubrid before/after 성능 수치
2. Tier 2 ORM 벤치마크
3. Performance Loop 2회 이상 완주 증명
4. one-command 재현 데모 (`docker compose up && make demo`)
5. 공모전 증거팩 (차트, 영상, 보고서)
