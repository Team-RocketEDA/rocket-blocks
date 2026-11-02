# SiEPIC EBeam — rocket-blocks

SiEPIC EBeam photonic PDK (UBC foundry). Domains: photonic.
Upstream PDK: [gdsfactory/ubc](https://github.com/gdsfactory/ubc) · [docs](https://gdsfactory.github.io/ubc)

Status: empty, awaiting seeding.

## What goes here

Self-contained entry folders, one per IP block. Per the repo rule: IP
blocks are prebuilt hierarchical blocks (symbol + cell linked),
strictly per-PDK. Photonic entries link PIC cells instead of footprints.

## Entry anatomy (v0 sketch; full standard pending)

```text
<entry>/
├── entry_repo/   # nested upstream checkout, ONLY if wrapping one
└── rocket/       # maintained rocket-compatible adapter
    ├── meta.yaml # name, version, upstream url+rev+license, kind, ports, links
    └── adapt.*   # conversion into engine-consumable artifacts
```

Entry folders are slugs (`lowercase-with-dashes`), unique within this PDK.
