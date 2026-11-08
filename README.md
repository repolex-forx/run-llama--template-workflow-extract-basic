# Repolex Knowledge Graph of run-llama/template-workflow-extract-basic

RDF knowledge graph data for [run-llama/template-workflow-extract-basic](https://github.com/run-llama/template-workflow-extract-basic), parsed by [repolex](https://repolex.ai).

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
rlex download run-llama/template-workflow-extract-basic
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── b4aad4f8e851bbab8c08407590f12ee5049cf916
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── b4aad4f8e851bbab8c08407590f12ee5049cf916
│           └── chunk-001.nq.gz
├── blob
│   ├── 095df0581b16ad0fbaa09210181082355c6a8852.nq.gz
│   ├── 0f48d31b8e28a6cbf797a405e8cc3c70bbbd184a.nq.gz
│   ├── 1bd7e75eb30d851dfcb2a0735b070e4b5a9a0c31.nq.gz
│   ├── 25ad5bcbea25ab78a63bd3f3f84a66693ffa7f2f.nq.gz
│   ├── 28421e9a2d828368600a96569397363add486aa2.nq.gz
│   ├── 35fca6eac9cae2583c8c1de898b60f793a1ec092.nq.gz
│   ├── 3cdee003bf488e12d3a4fa4953119126da830f87.nq.gz
│   ├── 3ef840615d4640601ef02d130ad64520554f45ce.nq.gz
│   ├── 453877564ffaa7b88a1f0ee26a55af5ab35e4cd4.nq.gz
│   ├── 45b37fc91442a293c8805c74bf853e259bab8ed1.nq.gz
│   ├── 4da33406e72b559c03d608dd6285862cf3587d83.nq.gz
│   ├── 5e13111b909c292f8edc2f6499d5d8bfba3214f2.nq.gz
│   ├── 696289b8290d83f707343b10b1f653eedadf3a92.nq.gz
│   ├── 6fa106702b614ba5fa6b97a24ff2b6c53c7f9f81.nq.gz
│   ├── 800bc6ad052fd0f8c6b71ae928ab138a3f6e430a.nq.gz
│   ├── 85c9a64cc53f6202cf5a66bcb8da2b80d60a1090.nq.gz
│   ├── 88acac8845cf45be2f401aa449d0fcf2f5b786c3.nq.gz
│   ├── 8a857cbbcc6194e4d5d2c58936ca687608f550e4.nq.gz
│   ├── 8fcca685f1148e88ba8445310c5609531bd0856f.nq.gz
│   ├── 97856e842efe3cace2180a4d1171b10594a84831.nq.gz
│   ├── 9d5c91e6b3db527b85409c39b9351e2482ba41e9.nq.gz
│   ├── b1f3492860feb8fe54d06551703182c6259ca77e.nq.gz
│   ├── b56bed7e80ac87ea7ce50913ef870f0db71980f1.nq.gz
│   ├── b65d27068dfb8847c52ad54237962a20b8b44243.nq.gz
│   ├── c01805e89c1684e79130151abc23bb80401583a9.nq.gz
│   ├── c01c299d6c5cef6521434d725677af1b65ff5cd4.nq.gz
│   ├── c5da6423128173b14442dc855c06a1d535726117.nq.gz
│   ├── d2958545a684467a2967c02a58b2d91ebd5031eb.nq.gz
│   ├── d8e401fe8f32fff3f18b4763baf4bb4fd63725b4.nq.gz
│   ├── dab92719d5e87d21d9c78afb909733288cb1c331.nq.gz
│   ├── db2f45ed1dc9a9e85d343908b48d330999619824.nq.gz
│   ├── df2e02be1f9bc925b7449501b03336c524564c69.nq.gz
│   ├── e5439b09bd058b9bbf5e3dc61d7f5eae6eb306eb.nq.gz
│   ├── e5a1fa50e315bbcf29a37b6cfa7e30437e705958.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── e8eb53be53aebf6345306a04536b5d2567a9d2ca.nq.gz
│   └── f900b7ec6513a252686e4363d6232bd846bb3b59.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── b4aad4f8e851bbab8c08407590f12ee5049cf916.nq.gz
└── tag
    └── tag.nq.gz

11 directories, 43 files
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

[run-llama/template-workflow-extract-basic](https://github.com/run-llama/template-workflow-extract-basic)

---
*Parsed on 2026-11-08 by [repolex](https://repolex.ai)*
