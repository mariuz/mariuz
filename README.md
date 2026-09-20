### Hi there 👋

I am **Adrian (Popa Marius Adrian)** — a software developer from Romania 🇷🇴 and a long‑time **Firebird RDBMS** contributor ([@FirebirdSQL](https://github.com/FirebirdSQL) member, 40+ PRs across the org).

I build and maintain open‑source tooling around Firebird: the desktop admin GUI, export/copy utilities, a web frontend, drivers, and the CI and containers that ship them. Lately I've been pushing Firebird into places it hasn't been before — **the browser (WASM)**, **Kubernetes**, **vector search**, **Rust**, and **LLM assistants over MCP**.

- 🔭 Maintaining [**FlameRobin**](https://github.com/mariuz/flamerobin) — the cross‑platform Firebird admin tool, shipping releases roughly monthly
- 🧪 Building [**fbvector**](https://github.com/mariuz/fbvector) (pgvector‑style similarity search for Firebird) and [**electric‑firebird**](https://github.com/mariuz/electric-firebird) (Firebird embedded in WASM)
- 🦀 Experimenting with [**fire‑crab**](https://github.com/mariuz/fire-crab) — incremental C++→Rust conversion of the Firebird engine, differential‑tested against the real one
- 💬 Ask me about **Firebird**, SQL, database internals, C++, or FreePascal
- 🌐 [reea.net](https://reea.net) · ✍️ [mapopa.blogspot.com](https://mapopa.blogspot.com)

---

### 🔥 FlameRobin

[![Latest release](https://img.shields.io/github/v/release/mariuz/flamerobin?label=release&color=1f1e34)](https://github.com/mariuz/flamerobin/releases)
[![Stars](https://img.shields.io/github/stars/mariuz/flamerobin?color=1f1e34)](https://github.com/mariuz/flamerobin/stargazers)
[![Last commit](https://img.shields.io/github/last-commit/mariuz/flamerobin?color=1f1e34)](https://github.com/mariuz/flamerobin/commits/master)

A lightweight, cross‑platform admin & development GUI for Firebird 2.5 → 6.0+, written in modern C++ with wxWidgets. Beyond the classics (metadata browser, data grid, DDL editor), it now does JSON field editing, temporal tables, query‑plan visualization, a **vector data editor**, and an embedded **MCP server** so AI assistants can talk to your database directly. → [**flamerobin.org**](http://flamerobin.org)

---

### ⭐ Selected projects

**Tools**

| Project | What it is | Tech |
| --- | --- | --- |
| [**flamerobin**](https://github.com/mariuz/flamerobin) | Cross‑platform admin & dev GUI for Firebird. Vector editor + built‑in MCP server. | C++ / wxWidgets |
| [**fbexport**](https://github.com/mariuz/fbexport) | Import/export data and run SQL scripts; FBCopy copies and compares data across databases. | C++ |
| [**gmarathon‑freepascal**](https://github.com/mariuz/gmarathon-freepascal) | The Marathon SQL IDE, ported from Delphi to Lazarus/FreePascal. | FreePascal |
| [**firebirdwebadmin**](https://github.com/mariuz/firebirdwebadmin) | Administer a Firebird server from the browser. | PHP |
| [**perl-dbd-firebird**](https://github.com/mariuz/perl-dbd-firebird) | `DBD::Firebird` — the Perl DBI driver. | Perl / XS |

**Firebird, in new places**

| Project | What it is | Tech |
| --- | --- | --- |
| [**fbvector**](https://github.com/mariuz/fbvector) | Vector storage and similarity search as a Firebird UDR — L2, cosine, inner product, L1 — SIMD‑accelerated with Google Highway. Think `pgvector`, for Firebird. | C++ |
| [**electric‑firebird**](https://github.com/mariuz/electric-firebird) | The real engine compiled to WASM, running in the browser with no server. PGlite‑style async API. → [**live demo**](https://mariuz.github.io/electric-firebird/) | TypeScript / WASM |
| [**cloudnative‑firebird**](https://github.com/mariuz/cloudnative-firebird) | Kubernetes operator with a `FirebirdCluster` CRD, in the spirit of cloudnative‑pg. | TypeScript |
| [**fire‑crab**](https://github.com/mariuz/fire-crab) 🔥🦀 | Incremental C++→Rust conversion of the engine, bottom‑up from the storage layer, differential‑tested against upstream from the first commit. | Rust |

**Explaining the database**

| Project | What it is |
| --- | --- |
| [**FBSimCity**](https://github.com/mariuz/FBSimCity) | An explorable isometric city that shows how Firebird actually works — Y‑valve, DSQL, page cache, latency. → [**live demo**](https://mariuz.github.io/FBSimCity/) |
| [**conceptual‑architecture‑for‑firebird‑paper**](https://github.com/mariuz/conceptual-architecture-for-firebird-paper) | The Waterloo conceptual‑architecture paper on Firebird, updated and re‑diagrammed. |

---

### 🧩 Talking to Firebird from your language

The upstream drivers I use, package, test against, or send patches to:

| Language | Driver | Notes |
| --- | --- | --- |
| 🐘 PHP | [FirebirdSQL/php-firebird](https://github.com/FirebirdSQL/php-firebird) | PDO + `interbase` extension |
| 🐍 Python | [FirebirdSQL/python3-driver](https://github.com/FirebirdSQL/python3-driver) · [nakagami/pyfirebirdsql](https://github.com/nakagami/pyfirebirdsql) | official & pure‑Python |
| 🐹 Go | [nakagami/firebirdsql](https://github.com/nakagami/firebirdsql) | `database/sql` driver |
| 🌐 Node | [hgourvest/node-firebird](https://github.com/hgourvest/node-firebird) · [asfernandes/node-firebird-driver](https://github.com/asfernandes/node-firebird-driver) | pure JS & TypeScript |
| 🐪 Perl | [**mariuz/perl-dbd-firebird**](https://github.com/mariuz/perl-dbd-firebird) | maintained here |
| 💎 Ruby | [rowland/fb](https://github.com/rowland/fb) | extension library |
| 🦀 Rust | [fernandobatels/rsfbclient](https://github.com/fernandobatels/rsfbclient) | native & embedded |
| ☕ Java | [FirebirdSQL/jaybird](https://github.com/FirebirdSQL/jaybird) | JDBC |
| 🟣 .NET | [FirebirdSQL/NETProvider](https://github.com/FirebirdSQL/NETProvider) | ADO.NET / EF Core |
| 🐳 Docker | [FirebirdSQL/firebird-docker](https://github.com/FirebirdSQL/firebird-docker) | official images |

---

### 🔮 Stack

- **Languages** — C++ · FreePascal · PHP · Python · TypeScript · Go · Rust · Perl · Shell
- **Data** — Firebird · SQLite · PostgreSQL · vector search & embeddings
- **AI** — Model Context Protocol (MCP) · LLM‑assisted database tooling
- **Build & ship** — GitHub Actions · GitLab CI · Docker · CMake · Meson · wxWidgets

---

### 📫 Elsewhere

[🌐 reea.net](https://reea.net) · [✍️ Blog](https://mapopa.blogspot.com) · [👤 LinkedIn](https://www.linkedin.com/in/mariuz/) · [🐘 Mastodon](https://mastodon.social/@mariuz) · [🦋 Bluesky](https://bsky.app/profile/mapopa.bsky.social) · [🧵 Threads](https://www.threads.com/@popa_adrian_marius) · [✉️ Email](mailto:mapopa@gmail.com)

❤️ If FlameRobin or any of this is useful to you, consider [sponsoring](https://github.com/sponsors/mariuz).
