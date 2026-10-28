# Repolex Knowledge Graph of databrickslabs/migrate-ip-acls

RDF knowledge graph data for [databrickslabs/migrate-ip-acls](https://github.com/databrickslabs/migrate-ip-acls), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [rlex](https://github.com/repolex-ai/rlex) query tool:

```bash
cargo install --git https://github.com/repolex-ai/rlex
```

Verify the install:

```bash
rlex --help
```

**rlex is designed to be used primarily by LLMs in a terminal.** Start up your favorite AI assistant and ask it to use rlex. It handles the SPARQL — you just ask questions in plain English.

To load this repo's data:

```bash
rlex download databrickslabs/migrate-ip-acls
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── f07a21a57b5fabda23fa97ab63ea07fefadc2a94
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── f07a21a57b5fabda23fa97ab63ea07fefadc2a94
│           └── chunk-001.nq.gz
├── blob
│   ├── 01da3d9d6f60a92769e4205f71c8dc337d7219db.nq.gz
│   ├── 05cb6a991f75c7fae54b84aaf099875bfd0f17ad.nq.gz
│   ├── 14c428021d3650e43d76f2b38fccc210edbe2853.nq.gz
│   ├── 20f34eb15a3dcea968690850d5d878504a4ec86a.nq.gz
│   ├── 28a7416b84e6737e6dba0d75559f9905e27b5b76.nq.gz
│   ├── 2abc8b38a3bf56c18df426890f4ccdc9f6692118.nq.gz
│   ├── 310a6d6a6e6dfa9553eb880b7ab733a0534d8f7f.nq.gz
│   ├── 352ad8a4416254594fa997f3842af5caa50c2e43.nq.gz
│   ├── 41394c21eeeae358ca94f991e040d5ce069fdf20.nq.gz
│   ├── 45d5574096f79e6422141dd5a5051604f69204b2.nq.gz
│   ├── 4f87d4d752e2f2971179d99c9004944e73cd5f2a.nq.gz
│   ├── 547754381e0deb0de8de75be8c869a0620990ad9.nq.gz
│   ├── 59a5e01e53966d897adde89b0e6266ba81d1b356.nq.gz
│   ├── 6047d689c2b426c8d8276a820628e0ddac580085.nq.gz
│   ├── 68f702d6091df094f478e3edb1f428f52a7d1049.nq.gz
│   ├── 7d8cfc5b64a52f7dc2718bc135df1093048fd58b.nq.gz
│   ├── 7e2ee1e5e2a8e55d4ac5f7f03f0432d9f1a82b24.nq.gz
│   ├── 9b93cc5a54b9b85f76ad1591f2aa598ab639ecb4.nq.gz
│   ├── ab86163c3167d768cb9c729ecd72dc6e7dfc0ed3.nq.gz
│   ├── b4566f0846b1928b242cca7831b0a8e6ee920e0f.nq.gz
│   ├── b5566a648c15ea057bb2674eb8b8330669537c81.nq.gz
│   ├── be8b42ca255cbbf3447f9fcfb791bb48cacd89a0.nq.gz
│   ├── c0f2495bed095d31cd5794ab36f381b6a9e3f6cb.nq.gz
│   ├── cd48ed1810b94b0439fe9badb2b1712ceacf5b0d.nq.gz
│   ├── d71a06a8020b2b809f755e403c1b0de1027bedab.nq.gz
│   ├── d805f4b635de279a02fe68b1a256484fb2d5a3bb.nq.gz
│   ├── ebed8373678d941f55662f79c42ec5d879aa729f.nq.gz
│   ├── f5276185ee9b1c644eae2f4c3a918d848b61c799.nq.gz
│   ├── fefd63a182a326d7e4eb01b2c5d12e6a33f923f1.nq.gz
│   └── ffbcbadc34ff03b405f7b1fe617f668f020137cf.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── f07a21a57b5fabda23fa97ab63ea07fefadc2a94.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

12 directories, 37 files
```

| Directory | What it contains |
|-----------|-----------------|
| `blob/` | Per-file AST graphs, content-addressed by git blob SHA. Each file in the source repo gets its own graph. |
| `aggregate/ast/` | Combined AST graph per parsed commit. Merges all blob graphs for a snapshot of the entire codebase at that point. |
| `aggregate/lsp/` | Language Server Protocol enrichment: resolved symbols, definitions, references, and type information. |
| `aggregate/dataflow/` | Interprocedural data flow edges between functions and modules. |
| `aggregate/repolex/` | Combined graph (AST + LSP + dataflow) per commit. |
| `commit/` | Git commit metadata (author, date, message, parent links). |
| `branch/` | Branch metadata. |
| `tag/` | Tag metadata. |
| `filetree/` | File tree snapshots per commit (which files existed and their blob SHAs). |
| `audit/` | Code architecture and graph audit reports per commit. |

## Source repository

[databrickslabs/migrate-ip-acls](https://github.com/databrickslabs/migrate-ip-acls)

---
*Parsed on 2026-10-28 by [repolex](https://repolex.ai)*
