# Repolex Knowledge Graph of zopefoundation/zope.size

RDF knowledge graph data for [zopefoundation/zope.size](https://github.com/zopefoundation/zope.size), parsed by [repolex](https://repolex.ai).

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
rlex download zopefoundation/zope.size
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── a7914d7957e1caf2993fa1217e35472f92ed7844
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── a7914d7957e1caf2993fa1217e35472f92ed7844
│           └── chunk-001.nq.gz
├── blob
│   ├── 034043e1628b277e8c3805e50acd2ac1e6e85255.nq.gz
│   ├── 0ab12fe1e0c8eb6cb0d68fce1b14a2209cdb0def.nq.gz
│   ├── 1f321f52abb7db6f79c285bab56e2852dc575699.nq.gz
│   ├── 407122fe1199f1275fa8b3f88e6c53c72c14f6d1.nq.gz
│   ├── 4edbaee9c7a3876e2a596748ce89df935603d7cf.nq.gz
│   ├── 52f70c8ce883994bd0d988a5c1a65fd67446995a.nq.gz
│   ├── 717bb607f8a664ec726e9216cbe5c07025598268.nq.gz
│   ├── 77c3aece3eaa74e4f1e77d1bf1b205a231e5ee1f.nq.gz
│   ├── 79859e06010bf4967c5b4b044afea6ef39742938.nq.gz
│   ├── 802b1885614585e0cd3228c6c84950b1e818974b.nq.gz
│   ├── 868c40e85dd80671da84952ec46ac65b3fb84c9e.nq.gz
│   ├── 8ce2e05ba90848c004f149e7272e75d9c1833444.nq.gz
│   ├── 9484f8c094119ea0ea6b676cc5e89c09c4be3dda.nq.gz
│   ├── a78ef8e93e20951709df85d0f2b0a72ac7bf9fb7.nq.gz
│   ├── ace150a60ef1c05d7b0247d0ccb92062f9b60753.nq.gz
│   ├── b1b66ea44d8852633e2942b77da6c504852aef85.nq.gz
│   ├── b82edd9f1e05c6b170230b1030be75274f5e5974.nq.gz
│   ├── b8764a8abb1b8b56b23b1c5e8398aac3fd7706c9.nq.gz
│   ├── c100369dc834c4035106c8a942c5b683d1dca995.nq.gz
│   ├── c5508b9f083362a81185d598327e7801d837cb18.nq.gz
│   ├── c6985b7d9ab15d17a022aa3fa5dcc55dddcd608b.nq.gz
│   ├── ccdedc28073a0ba8303c52c91284a4e7e70bb471.nq.gz
│   ├── d9e113ec685b92b018297dd2f200341d1fba01f9.nq.gz
│   ├── e1f9ad7b3b48377bfbfaa1b380c384ddea24060f.nq.gz
│   ├── e235f162f07f7075ca7b9c21da8e1ef766cabbc4.nq.gz
│   ├── e3579011e1a5792ed2adb52fe79f1ac001b9c3bf.nq.gz
│   ├── ec960deb6a27d702e76ceb734ff5f4af858b7fdb.nq.gz
│   ├── f0ed9d001e553f388470f3a0b5eca7e9269311c7.nq.gz
│   └── fa992cbd4cb7d6542795f83a82a9d9147c243c6b.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── a7914d7957e1caf2993fa1217e35472f92ed7844.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 37 files
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

[zopefoundation/zope.size](https://github.com/zopefoundation/zope.size)

---
*Parsed on 2026-11-06 by [repolex](https://repolex.ai)*
