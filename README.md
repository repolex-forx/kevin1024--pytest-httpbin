# Repolex Knowledge Graph of kevin1024/pytest-httpbin

RDF knowledge graph data for [kevin1024/pytest-httpbin](https://github.com/kevin1024/pytest-httpbin), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [lexq](https://github.com/repolex-ai/lexq) query tool using [uv](https://docs.astral.sh/uv/getting-started/installation/).

If you have uv installed, just copy/paste this into your terminal:

```bash
uv tool install git+https://github.com/repolex-ai/lexq
```

This installs lexq onto your system, in your user context. Verify the install:

```bash
lexq --help
```

**lexq is designed to be used primarily by LLMs in a terminal.** Start up your favorite LLM and ask it to use the lexq tool. It's that easy!

To load this repo's data:

```bash
lexq download kevin1024/pytest-httpbin
```

This will automatically download essential data files from the last parsed commit. Consult `lexq --moreinfo` for other options, including downloading multiple commits, blobs, etc.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 5cee134e732506bf190b0a043c554247e1b83785
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   └── 5cee134e732506bf190b0a043c554247e1b83785.nq.gz
│   └── repolex
│       └── 5cee134e732506bf190b0a043c554247e1b83785
│           └── chunk-001.nq.gz
├── blob
│   ├── 03623e121e3104366f01ae908cf14d30b12cc31d.nq.gz
│   ├── 03a78fc64b0b65bc320f97c9adeb5d632eea63b1.nq.gz
│   ├── 066bc629204e30f2a202c4e95e9fa5d972d88bce.nq.gz
│   ├── 12541cc5b1fb95d90b2778a1e8a55dd9eb9be20f.nq.gz
│   ├── 17ddfd4db4c77bcddb0101ccf0bb300ff1708f06.nq.gz
│   ├── 1de1a0d19e806a6c2eb0a2360f55d061e6169245.nq.gz
│   ├── 230f41bbb26608846348cc2b7fe8879b4e48dc64.nq.gz
│   ├── 46c2ff56b8712baf167dcd7c5341f8a3c85649f0.nq.gz
│   ├── 4d77de2cde4cd6add4e4f64e654a75316d24febf.nq.gz
│   ├── 4e0cba87c0d179977296a2079b559f3f52b22826.nq.gz
│   ├── 5d4402a1cdf4af1f35dbea610ce728f7a8860ffa.nq.gz
│   ├── 6115f03c65cae5c5d59f5710dbe711d6fdcd118c.nq.gz
│   ├── 741846848fef34887429fe88b545d5b8761a9d9d.nq.gz
│   ├── 7572aebe510f8c7a7bfb242b1a0baadfee49d74b.nq.gz
│   ├── 794613724aa05c9bc3fa734e38e8c3ff47e16c40.nq.gz
│   ├── 7c70f6460d713e21a41c8c868e807c3e10a3a599.nq.gz
│   ├── 7d9dc337cb976be91b359b6765eb3410754e98a8.nq.gz
│   ├── 98133238bb4db0a4aa4c5c5224bb77b14d60e9f9.nq.gz
│   ├── 9aa3f90365fde8f020d7d8d42193f97c3d0660e1.nq.gz
│   ├── 9f2e4aaa7a566be9ff5694a12d9f5f1d06011e55.nq.gz
│   ├── c06475ed14ee0e5a39d31fd23a2bad734c5de9e2.nq.gz
│   ├── ca73058dda4f9c380668eab72514c78b5ab34a85.nq.gz
│   ├── edba2746747f07bf0706085b42190a7255f91e71.nq.gz
│   └── fd9fd8296760ea8d01197050253af171c8909b55.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── dep
│   └── 5cee134e732506bf190b0a043c554247e1b83785.nq.gz
├── filetree
│   └── 5cee134e732506bf190b0a043c554247e1b83785.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

15 directories, 34 files
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

## Source repository

[kevin1024/pytest-httpbin](https://github.com/kevin1024/pytest-httpbin)

---
*Parsed on 2026-04-09 by [repolex](https://repolex.ai)*
