# CUBRID Labs — Ecosystem Roadmap

> **Last updated**: 2026-04-19
>
> This is the unified roadmap for the cubrid-labs ecosystem.
> Milestones are authoritative for "next release" scope.
> This document is authoritative for direction, priorities, and cross-repo dependencies.
>
> 📋 [**Org Project Board**](https://github.com/orgs/cubrid-labs/projects/2) · See [individual repo milestones](#release-focus-by-repo) for execution details.

---

## Ecosystem Map

```mermaid
graph TD
    subgraph Drivers["🔌 Drivers"]
        pycubrid["pycubrid (Python)\nv1.2.0"]
        cubrid_client["cubrid-client (TypeScript)\nv1.1.0"]
        cubrid_go["cubrid-go (Go)\nv0.2.1"]
        cubrid_rs["cubrid-rs (Rust)\nv0.1.0"]
    end

    subgraph ORMs["🏗️ ORMs & Dialects"]
        sqlalchemy["sqlalchemy-cubrid\nv1.3.0"]
        drizzle["drizzle-cubrid\nv0.2.1"]
        gorm["gorm-cubrid\nv0.1.0"]
        sea_orm["sea-orm-cubrid\nv0.1.0"]
    end

    subgraph Meta["📚 Meta"]
        cookbook["cubrid-cookbook"]
        benchmark["cubrid-benchmark"]
    end

    pycubrid --> sqlalchemy
    cubrid_client --> drizzle
    cubrid_go --> gorm
    cubrid_rs --> sea_orm

    sqlalchemy --> cookbook
    drizzle --> cookbook
    gorm --> cookbook
    sea_orm --> cookbook

    pycubrid --> benchmark
    cubrid_client --> benchmark
    cubrid_go --> benchmark
    cubrid_rs --> benchmark
```

---

## Now / Next / Later

### 🟢 Now (Current Focus)

- **Performance profiling & optimization** — Python driver optimized (19% fetch improvement); query compilation cache added to sqlalchemy-cubrid. Ongoing: further gap reduction vs MySQL.
- **Benchmark automation** — Nightly CI runs with extended workloads (connect/disconnect, prepared statements, batch insert, concurrent select)
- **cubrid-rs protocol completion** — Broker handshake, authentication, query execution (v0.2.0)

### 🟡 Next (1–3 Months)

- **v1.0 stabilization** — API freeze for cubrid-go, gorm-cubrid, drizzle-cubrid
- **Connection resilience** — Retry policies, connection health checks (cubrid-client v1.2.0)
- **Registry publishing** — crates.io (cubrid-rs, sea-orm-cubrid); PyPI Trusted Publisher configured ✅ (pycubrid v0.6.0, sqlalchemy-cubrid v0.7.1 published)
- **Cookbook completeness** — Rust examples after crates.io publish, all examples verified working

### 🔵 Later (3–6 Months)

- **JSON type mapping** — CUBRID supports JSON since 10.2; map in sqlalchemy-cubrid, pycubrid, cubrid-client
- **Async driver for Rust** — cubrid-tokio with backpressure handling (cubrid-rs v0.5.0)
- **Connection pool crates** — cubrid-pool for Rust (cubrid-rs v0.6.0)
- **Full SeaORM feature parity** — Entity generation, migrations, crates.io availability
- **Ecosystem documentation portal** — Unified docs site (GitHub Pages)

---

## Dependency Graph

```mermaid
graph LR
    subgraph "Must stabilize first"
        A[pycubrid v1.0.0]
        B[cubrid-go v1.0.0]
        C[cubrid-rs v0.2.0]
        D[cubrid-client v1.2.0]
    end

    subgraph "Depends on driver stability"
        E[sqlalchemy-cubrid v0.8.0]
        F[gorm-cubrid v1.0.0]
        G[drizzle-cubrid v1.0.0]
        H[sea-orm-cubrid v1.0.0]
    end

    subgraph "Depends on all above"
        I[cubrid-cookbook v1.0]
        J[cubrid-benchmark v1.0]
    end

    A --> E
    B --> F
    C --> H
    D --> G
    E --> I
    F --> I
    G --> I
    H --> I
    A --> J
    B --> J
    C --> J
    D --> J
```

---

## Release Focus by Repo

| Repo | Next Milestone | Focus | Link |
|------|---------------|-------|------|
| **pycubrid** | [v0.6.0](https://github.com/cubrid-labs/pycubrid/milestone/2) | Performance — ✅ shipped (19% fetch improvement, 2 optimization cycles) | [Milestones](https://github.com/cubrid-labs/pycubrid/milestones) |
| **pycubrid** | [v1.0.0](https://github.com/cubrid-labs/pycubrid/milestone/1) | Stable release — full PEP 249, connection pooling | [Milestones](https://github.com/cubrid-labs/pycubrid/milestones) |
| **sqlalchemy-cubrid** | [v0.8.0](https://github.com/cubrid-labs/sqlalchemy-cubrid/milestone/1) | Performance & optimization | [Milestones](https://github.com/cubrid-labs/sqlalchemy-cubrid/milestones) |
| **sqlalchemy-cubrid** | [v0.9.0](https://github.com/cubrid-labs/sqlalchemy-cubrid/milestone/2) | Ecosystem & documentation | [Milestones](https://github.com/cubrid-labs/sqlalchemy-cubrid/milestones) |
| **cubrid-client** | [v1.2.0](https://github.com/cubrid-labs/cubrid-client/milestone/1) | Reliability & performance | [Milestones](https://github.com/cubrid-labs/cubrid-client/milestones) |
| **drizzle-cubrid** | [v1.0.0](https://github.com/cubrid-labs/drizzle-cubrid/milestone/1) | Stable release | [Milestones](https://github.com/cubrid-labs/drizzle-cubrid/milestones) |
| **cubrid-go** | [v1.0.0](https://github.com/cubrid-labs/cubrid-go/milestone/1) | Stable release | [Milestones](https://github.com/cubrid-labs/cubrid-go/milestones) |
| **gorm-cubrid** | [v1.0.0](https://github.com/cubrid-labs/gorm-cubrid/milestone/1) | Stable release | [Milestones](https://github.com/cubrid-labs/gorm-cubrid/milestones) |
| **cubrid-rs** | [v0.2.0](https://github.com/cubrid-labs/cubrid-rs/milestone/1) | Protocol completeness | [Milestones](https://github.com/cubrid-labs/cubrid-rs/milestones) |
| **cubrid-rs** | [v1.0.0](https://github.com/cubrid-labs/cubrid-rs/milestone/2) | Stable release | [Milestones](https://github.com/cubrid-labs/cubrid-rs/milestones) |
| **sea-orm-cubrid** | [v1.0.0](https://github.com/cubrid-labs/sea-orm-cubrid/milestone/1) | Stable release | [Milestones](https://github.com/cubrid-labs/sea-orm-cubrid/milestones) |
| **cubrid-cookbook** | [v1.0](https://github.com/cubrid-labs/cubrid-cookbook/milestone/1) | Complete examples | [Milestones](https://github.com/cubrid-labs/cubrid-cookbook/milestones) |
| **cubrid-benchmark** | [v1.0](https://github.com/cubrid-labs/cubrid-benchmark/milestone/1) | Comprehensive benchmarks | [Milestones](https://github.com/cubrid-labs/cubrid-benchmark/milestones) |

---

## Contributing

We welcome contributions to any repo in the ecosystem!

- 🐛 **Found a bug?** Open an issue on the relevant repo
- 💡 **Have a feature idea?** Start a [Discussion](https://github.com/orgs/cubrid-labs/discussions)
- 🔧 **Want to contribute code?** See [CONTRIBUTING.md](CONTRIBUTING.md) and look for `good first issue` labels
- 📋 **Track progress**: [Org Project Board](https://github.com/orgs/cubrid-labs/projects/2)

---

> **Disclaimer**: This roadmap reflects current intentions and priorities. Timelines and scope may change based on community feedback, contributor availability, and technical discoveries. Milestones on individual repos are the most up-to-date source for release planning.
