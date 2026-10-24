### Hi there 👋

I am **Adrian (Popa Marius Adrian)** — a software developer from Romania 🇷🇴 and a long‑time **Firebird RDBMS** contributor ([@FirebirdSQL](https://github.com/FirebirdSQL) member, 40+ PRs across the org).

I build and maintain open‑source tooling around Firebird: the desktop admin GUI, export/copy utilities, a web frontend, drivers, and the CI and containers that ship them. Lately I've been pushing Firebird into places it hasn't been before — **the browser (WASM)**, **Kubernetes**, **vector search**, **Rust**, and **LLM assistants over MCP**.

- 🔭 Maintaining [**FlameRobin**](https://github.com/mariuz/flamerobin) — the cross‑platform Firebird admin tool, shipping releases roughly monthly
- 🧪 Building [**fbvector**](https://github.com/mariuz/fbvector) (pgvector‑style similarity search for Firebird) and [**electric‑firebird**](https://github.com/mariuz/electric-firebird) (Firebird embedded in WASM)
- 🎮 Running DOOM and Quake **inside a Firebird database** in the browser: [play the demos](#-games-rendered-by-a-database)
- 🦀 Experimenting with [**fire‑crab**](https://github.com/mariuz/fire-crab) — incremental C++→Rust conversion of the Firebird engine, differential‑tested against the real one
- 💬 Ask me about **Firebird**, SQL, database internals, C++, or FreePascal
- 🏠 [mariuz.github.io](https://mariuz.github.io/) · 🌐 [reea.net](https://reea.net) · ✍️ [mapopa.blogspot.com](https://mapopa.blogspot.com)

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
| [**fbadmin**](https://github.com/mariuz/fbadmin) | pgAdmin‑style web admin for Firebird: object explorer, DDL extraction, query tool with plans, editable grid. → [**project page**](https://mariuz.github.io/fbadmin/) | Web |
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
| [**FirebirdREST**](https://github.com/mariuz/firebirdrest) | Serve a RESTful API from any Firebird database. → [**docs**](https://mariuz.github.io/firebirdrest/) | REST |
| [**firebirdrest‑js**](https://github.com/mariuz/firebirdrest-js) | The supabase‑js query API (`from()`, `select()`, filters, `rpc()`, upserts) for FirebirdREST. | JavaScript |
| [**fire‑crab**](https://github.com/mariuz/fire-crab) 🔥🦀 | Incremental C++→Rust conversion of the engine, bottom‑up from the storage layer, differential‑tested against upstream from the first commit. | Rust |

**Explaining the database**

| Project | What it is |
| --- | --- |
| [**FBSimCity**](https://github.com/mariuz/FBSimCity) | An explorable isometric city that shows how Firebird actually works — Y‑valve, DSQL, MVCC, sweep, backups, replication, and (since v0.9) the real engine in the machine room. → [**live demo**](https://mariuz.github.io/FBSimCity/) |
| [**conceptual‑architecture‑for‑firebird‑paper**](https://github.com/mariuz/conceptual-architecture-for-firebird-paper) | The Waterloo conceptual‑architecture paper on Firebird, updated and re‑diagrammed. |

---

### 🎮 Games, rendered by a database

Classic shooters simulated and rendered **inside Firebird 6 compiled to WebAssembly**, plus engine ports. All run in the browser:

| Game | Running on | Play |
| --- | --- | --- |
| [**firebird-doom**](https://github.com/mariuz/firebird-doom) | Firebird SQL / WASM | [▶ play](https://mariuz.github.io/firebird-doom/) |
| [**firebird-quake**](https://github.com/mariuz/firebird-quake) | Firebird SQL / WASM | [▶ play](https://mariuz.github.io/firebird-quake/) |
| [**firebird-quake2**](https://github.com/mariuz/firebird-quake2) | Firebird SQL / WASM | [▶ play](https://mariuz.github.io/firebird-quake2/) |
| [**firebird-quake3**](https://github.com/mariuz/firebird-quake3) | Firebird SQL / WASM | [▶ play](https://mariuz.github.io/firebird-quake3/) |
| [**castle-doom**](https://github.com/mariuz/castle-doom) | Castle Game Engine (Object Pascal) | [▶ play](https://mariuz.github.io/castle-doom/) |
| [**castle-quake1**](https://github.com/mariuz/castle-quake1) | Castle Game Engine (Object Pascal) | [▶ play](https://mariuz.github.io/castle-quake1/) |
| [**castle-quake2**](https://github.com/mariuz/castle-quake2) | Castle Game Engine (Object Pascal) | [▶ play](https://mariuz.github.io/castle-quake2/) |
| [**castle-doom3**](https://github.com/mariuz/castle-doom3) | Castle Game Engine (Object Pascal) | desktop |
| [**unreal-doom**](https://github.com/mariuz/unreal-doom) | Unreal Engine 5.8 (C++), Lumen, co‑op & deathmatch | desktop |

---

### 📣 Latest announcements

- 2026‑10‑21 · [Firebird can now be built with CMake + Clang on Windows, Linux and macOS](https://mapopa.blogspot.com/2026/10/firebird-can-now-be-built-with-cmake.html)
- 2026‑08‑15 · [FBSimCity v0.9.0: the machine room, with the real Firebird engine inside the city](https://mapopa.blogspot.com/2026/08/fbsimcity-v090-machine-room-real.html)
- 2026‑08‑09 · [Electric Firebird: the Firebird engine compiled to WebAssembly, with a live demo](https://mapopa.blogspot.com/2026/08/electric-firebird-firebird-database.html)
- 2026‑08‑04 · [Firebird adds an optional static fbclient](https://mapopa.blogspot.com/2026/08/firebird-adds-optional-static-fbclient.html)
- 2026‑07‑31 · [node-firebird catches up: roadmap complete, issue tracker at zero](https://mapopa.blogspot.com/2026/07/node-firebird-catches-up-roadmap.html)
- 2026‑07‑31 · [cl-firebird v1.0.0: a pure Common Lisp driver for Firebird](https://mapopa.blogspot.com/2026/07/announcing-cl-firebird-v100-pure-common.html)
- 2026‑07‑13 · [node-firebird v2.6.0: TypeScript 7, query cancellation, Firebird 6.0 support](https://mapopa.blogspot.com/2026/07/announcing-node-firebird-v260.html)

→ [All posts](https://mapopa.blogspot.com) · [mariuz.github.io](https://mariuz.github.io/)

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
- **Games & graphics** — WebAssembly · Castle Game Engine · Unreal Engine 5
- **Build & ship** — GitHub Actions · GitLab CI · Docker · CMake · Meson · wxWidgets

---

### 📫 Elsewhere

[🏠 mariuz.github.io](https://mariuz.github.io/) · [🌐 reea.net](https://reea.net) · [✍️ Blog](https://mapopa.blogspot.com) · [👤 LinkedIn](https://www.linkedin.com/in/mariuz/) · [🐘 Mastodon](https://mastodon.social/@mariuz) · [🦋 Bluesky](https://bsky.app/profile/mapopa.bsky.social) · [🧵 Threads](https://www.threads.com/@popa_adrian_marius) · [✉️ Email](mailto:mapopa@gmail.com)

❤️ If FlameRobin or any of this is useful to you, consider [sponsoring](https://github.com/sponsors/mariuz).
