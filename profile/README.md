# CUBRID Labs

<div align="center">

[![GitHub Organization](https://img.shields.io/badge/GitHub-cubrid--labs-181717?logo=github)](https://github.com/cubrid-labs)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

**Modern database tooling for CUBRID — Python, TypeScript, Go, Rust**

*A comprehensive ecosystem of drivers, ORMs, and tools for building applications with CUBRID.*

</div>

---

## 한국어 소개

CUBRID Labs는 CUBRID 데이터베이스를 위한 현대적이고 생산성 높은 도구들을 개발하고 유지보수하는 조직입니다. Python, TypeScript, Go, Rust 등 다양한 언어로 드라이버, ORM, 예제 코드를 제공하여 개발자들이 CUBRID를 쉽고 효율적으로 사용할 수 있도록 합니다.

---

## Projects

### Drivers

| Repository | Language | Description | Status |
|---|---|---|---|
| **[pycubrid](https://github.com/cubrid-labs/pycubrid)** | Python | Pure Python DB-API 2.0 compliant driver | [![Tests](https://img.shields.io/github/actions/workflow/status/cubrid-labs/pycubrid/ci.yml?label=tests)](https://github.com/cubrid-labs/pycubrid/actions) |
| **[cubrid-client](https://github.com/cubrid-labs/cubrid-client)** | TypeScript | TypeScript-first Node.js client with async/await | [![Tests](https://img.shields.io/github/actions/workflow/status/cubrid-labs/cubrid-client/ci.yml?label=tests)](https://github.com/cubrid-labs/cubrid-client/actions) [![npm](https://img.shields.io/npm/v/cubrid-client)](https://www.npmjs.com/package/cubrid-client) |
| **[cubrid-go](https://github.com/cubrid-labs/cubrid-go)** | Go | Pure Go `database/sql` driver | [![Tests](https://img.shields.io/github/actions/workflow/status/cubrid-labs/cubrid-go/ci.yml?label=tests)](https://github.com/cubrid-labs/cubrid-go/actions) |
| **[cubrid-rs](https://github.com/cubrid-labs/cubrid-rs)** | Rust | Async Rust driver (reverse-engineered CAS protocol) | [![Tests](https://img.shields.io/github/actions/workflow/status/cubrid-labs/cubrid-rs/ci.yml?label=tests)](https://github.com/cubrid-labs/cubrid-rs/actions) |

### ORMs & Dialects

| Repository | Language | Description | Status |
|---|---|---|---|
| **[sqlalchemy-cubrid](https://github.com/cubrid-labs/sqlalchemy-cubrid)** | Python | SQLAlchemy 2.0–2.1 dialect | [![Tests](https://img.shields.io/github/actions/workflow/status/cubrid-labs/sqlalchemy-cubrid/ci.yml?label=tests)](https://github.com/cubrid-labs/sqlalchemy-cubrid/actions) [![Coverage](https://img.shields.io/badge/coverage-99.47%25-brightgreen)](https://github.com/cubrid-labs/sqlalchemy-cubrid) |
| **[drizzle-cubrid](https://github.com/cubrid-labs/drizzle-cubrid)** | TypeScript | Drizzle ORM dialect with type-safe schema | [![npm](https://img.shields.io/npm/v/drizzle-cubrid)](https://www.npmjs.com/package/drizzle-cubrid) |
| **[gorm-cubrid](https://github.com/cubrid-labs/gorm-cubrid)** | Go | GORM dialect for CUBRID | [![Tests](https://img.shields.io/github/actions/workflow/status/cubrid-labs/gorm-cubrid/ci.yml?label=tests)](https://github.com/cubrid-labs/gorm-cubrid/actions) |
| **[sea-orm-cubrid](https://github.com/cubrid-labs/sea-orm-cubrid)** | Rust | SeaORM backend for CUBRID | [![Tests](https://img.shields.io/github/actions/workflow/status/cubrid-labs/sea-orm-cubrid/ci.yml?label=tests)](https://github.com/cubrid-labs/sea-orm-cubrid/actions) |

### Tools & Resources

| Repository | Description |
|---|---|
| **[cubrid-cookbook](https://github.com/cubrid-labs/cubrid-cookbook)** | Production-ready examples across Python, TypeScript, Go, and Rust |
| **[cubrid-benchmark](https://github.com/cubrid-labs/cubrid-benchmark)** | Multi-language benchmark suite (CUBRID vs MySQL) |

---

## Roadmap

See the **[Ecosystem Roadmap](https://github.com/cubrid-labs/.github/blob/main/ROADMAP.md)** for cross-repo priorities and timeline.

Track execution on the **[Project Board](https://github.com/orgs/cubrid-labs/projects/2)**.

---

## Getting Started

> **New to CUBRID?** Read the [CUBRID in 5 Minutes](https://github.com/cubrid-labs/cubrid-cookbook/blob/main/GETTING_STARTED.md) guide — pick your language and build something in one page.

**Choose your language:**

- **Python**: [`sqlalchemy-cubrid`](https://github.com/cubrid-labs/sqlalchemy-cubrid) (ORM) or [`pycubrid`](https://github.com/cubrid-labs/pycubrid) (driver)
- **TypeScript/Node.js**: [`drizzle-cubrid`](https://github.com/cubrid-labs/drizzle-cubrid) (ORM) or [`cubrid-client`](https://github.com/cubrid-labs/cubrid-client) (driver)
- **Go**: [`gorm-cubrid`](https://github.com/cubrid-labs/gorm-cubrid) (ORM) or [`cubrid-go`](https://github.com/cubrid-labs/cubrid-go) (driver)
- **Rust**: [`sea-orm-cubrid`](https://github.com/cubrid-labs/sea-orm-cubrid) (ORM) or [`cubrid-rs`](https://github.com/cubrid-labs/cubrid-rs) (driver)

Each repository includes setup instructions, API documentation, and examples.

---

## Contributing

We welcome contributions! Please see [CONTRIBUTING.md](../.github/CONTRIBUTING.md) for guidelines.

**Community:**
- 💬 Questions? Post in [GitHub Discussions](https://github.com/orgs/cubrid-labs/discussions)
- 🐛 Found a bug? Open an issue on the relevant repo
- 📝 Have an idea? Start a [Discussion](https://github.com/orgs/cubrid-labs/discussions)
- 📋 Track progress: [Project Board](https://github.com/orgs/cubrid-labs/projects/2)

---

## License

All projects are licensed under the **MIT License**. See individual repositories for details.

---

## Security

If you discover a security vulnerability, please report it via [GitHub Security Advisories](https://github.com/cubrid-labs/sqlalchemy-cubrid/security/advisories) or email the maintainers. Do not open a public issue. See [SECURITY.md](../.github/SECURITY.md) for details.

---

<div align="center">

Made with ❤️ by the CUBRID Labs team

[GitHub](https://github.com/cubrid-labs) • [Discussions](https://github.com/orgs/cubrid-labs/discussions)

</div>
