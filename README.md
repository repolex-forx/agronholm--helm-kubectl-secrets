# Repolex Knowledge Graph of agronholm/helm-kubectl-secrets

RDF knowledge graph data for [agronholm/helm-kubectl-secrets](https://github.com/agronholm/helm-kubectl-secrets), parsed by [repolex](https://repolex.ai).

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
rlex download agronholm/helm-kubectl-secrets
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 9e42495461a88046d5b40cf5619d37eb96c32b70
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 9e42495461a88046d5b40cf5619d37eb96c32b70
│           └── chunk-001.nq.gz
├── blob
│   ├── 041744dac52a153cc35de2a84e541aebd2885c1f.nq.gz
│   ├── 0cc95f3069bac4c36b0c0c862c47e0fac016d942.nq.gz
│   ├── 104289d689d0bd425e4ca1ab5b598c37cf0aab2b.nq.gz
│   ├── 190e8d5726d3ab21da82a53b5458b08d96c02f31.nq.gz
│   ├── 23aa9cb88e1e2b2a46f1e53db5bc2dc04015f94a.nq.gz
│   ├── 2c5f07297d616a92b0f52d122348b1950d3a69e9.nq.gz
│   ├── 5abe6dda1635e58a39b25ccb0a0ec3fd78c3160f.nq.gz
│   ├── 9ed9f895d4597396bcba6c0ea3c23b3d6ca0dd4a.nq.gz
│   ├── aba498e6517a00f259ad001378b43b9930352c8a.nq.gz
│   ├── b0342ae5858f66f07bf10b263cfd9307453c6580.nq.gz
│   ├── b2ec497969902f810e2659d271dabe025e8a442d.nq.gz
│   ├── c1043f00fb48987c66f209501dcd455946e370cf.nq.gz
│   ├── e2f0e027557b7d7efd2433a0ea0ed59d3466cb65.nq.gz
│   ├── e3b7145cc34bb212aafde028d18792e130208f0a.nq.gz
│   ├── efd42459dc75ee9aa573b5d10937f67957c63d90.nq.gz
│   └── f098fa4430cd15d7ab712d093ff6aac9178f85d3.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 9e42495461a88046d5b40cf5619d37eb96c32b70.nq.gz
└── tag
    └── tag.nq.gz

11 directories, 22 files
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

[agronholm/helm-kubectl-secrets](https://github.com/agronholm/helm-kubectl-secrets)

---
*Parsed on 2026-10-11 by [repolex](https://repolex.ai)*
