# CUBRID Labs

<div align="center">

[![GitHub Organization](https://img.shields.io/badge/GitHub-cubrid--labs-181717?logo=github)](https://github.com/cubrid-labs)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

**Modern database tooling for CUBRID — Python, TypeScript, Go**

*A comprehensive ecosystem of drivers, ORMs, and tools for building applications with CUBRID.*

</div>

---

## 한국어 소개

CUBRID Labs는 CUBRID 데이터베이스를 위한 현대적이고 생산성 높은 도구들을 개발하고 유지보수하는 조직입니다. Python, TypeScript, Go 등 다양한 언어로 드라이버, ORM, 예제 코드를 제공하여 개발자들이 CUBRID를 쉽고 효율적으로 사용할 수 있도록 합니다.

---

## Projects

### Drivers & ORMs

| Repository | Language | Description | Status |
|---|---|---|---|
| **[sqlalchemy-cubrid](https://github.com/cubrid-labs/sqlalchemy-cubrid)** | Python | SQLAlchemy 2.0–2.1 dialect with full DDL/DML support, schema reflection, and type mapping | [![Tests](https://img.shields.io/github/actions/workflow/status/cubrid-labs/sqlalchemy-cubrid/ci.yml?label=tests)](https://github.com/cubrid-labs/sqlalchemy-cubrid/actions) [![Coverage](https://img.shields.io/badge/coverage-99.47%25-brightgreen)](https://github.com/cubrid-labs/sqlalchemy-cubrid) [![PyPI](https://img.shields.io/pypi/v/sqlalchemy-cubrid.svg)](https://pypi.org/project/sqlalchemy-cubrid/) |
| **[pycubrid](https://github.com/cubrid-labs/pycubrid)** | Python | Pure Python DB-API 2.0 compliant driver for CUBRID | [![Tests](https://img.shields.io/github/actions/workflow/status/cubrid-labs/pycubrid/ci.yml?label=tests)](https://github.com/cubrid-labs/pycubrid/actions) [![PyPI](https://img.shields.io/pypi/v/pycubrid.svg)](https://pypi.org/project/pycubrid/) |
| **[cubrid-client](https://github.com/cubrid-labs/cubrid-client)** | TypeScript/Node.js | TypeScript-first Node.js client with async/await support | [![Tests](https://img.shields.io/github/actions/workflow/status/cubrid-labs/cubrid-client/ci.yml?label=tests)](https://github.com/cubrid-labs/cubrid-client/actions) [![npm](https://img.shields.io/npm/v/cubrid-client)](https://www.npmjs.com/package/cubrid-client) |
| **[drizzle-cubrid](https://github.com/cubrid-labs/drizzle-cubrid)** | TypeScript | Drizzle ORM dialect for CUBRID with type-safe schema building | [![npm](https://img.shields.io/npm/v/drizzle-cubrid)](https://www.npmjs.com/package/drizzle-cubrid) |
| **[cubrid-go](https://github.com/cubrid-labs/cubrid-go)** | Go | Pure Go `database/sql` driver for CUBRID | [![Go](https://img.shields.io/github/go-mod/go-version/cubrid-labs/cubrid-go)](https://pkg.go.dev/github.com/cubrid-labs/cubrid-go) |
| **[gorm-cubrid](https://github.com/cubrid-labs/gorm-cubrid)** | Go | GORM dialect for CUBRID with ORM features | [![Go](https://img.shields.io/github/go-mod/go-version/cubrid-labs/gorm-cubrid)](https://pkg.go.dev/gorm.io/gorm) |

### Examples & Documentation

| Repository | Description |
|---|---|
| **[cubrid-cookbook](https://github.com/cubrid-labs/cubrid-cookbook)** | Production-ready examples across Python, Node.js, Go, and TypeScript frameworks |

---

## Getting Started

> **New to CUBRID?** Read the [CUBRID in 5 Minutes](https://github.com/cubrid-labs/cubrid-cookbook/blob/main/GETTING_STARTED.md) guide — pick your language and build something in one page.

**Choose your language:**

- **Python**: [`sqlalchemy-cubrid`](https://github.com/cubrid-labs/sqlalchemy-cubrid) (ORM via SQLAlchemy) or [`pycubrid`](https://github.com/cubrid-labs/pycubrid) (native driver)
- **TypeScript/Node.js**: [`cubrid-client`](https://github.com/cubrid-labs/cubrid-client) or [`drizzle-cubrid`](https://github.com/cubrid-labs/drizzle-cubrid) (ORM)
- **Go**: [`cubrid-go`](https://github.com/cubrid-labs/cubrid-go) or [`gorm-cubrid`](https://github.com/cubrid-labs/gorm-cubrid) (ORM)

Each repository includes setup instructions, API documentation, and examples.

---

## Contributing

We welcome contributions! Please see [CONTRIBUTING.md](../.github/CONTRIBUTING.md) for guidelines.

**Community:**
- 💬 Questions? Post in [GitHub Discussions](https://github.com/orgs/cubrid-labs/discussions)
- 🐛 Found a bug? Open an [Issue](https://github.com/cubrid-labs/sqlalchemy-cubrid/issues)
- 📝 Have an idea? Start a [Discussion](https://github.com/orgs/cubrid-labs/discussions)

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
