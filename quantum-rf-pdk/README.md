# Quantum RF PDK — rocket-blocks

Superconducting quantum / RF PDK. Domains: quantum, RF.
Upstream PDK: [gdsfactory/quantum-rf-pdk](https://github.com/gdsfactory/quantum-rf-pdk) · [docs](https://gdsfactory.github.io/quantum-rf-pdk/)

Status: empty, awaiting seeding.

## What goes here

Self-contained entry folders, one per IP block. Per the repo rule: IP
blocks are prebuilt hierarchical blocks (symbol + cell linked),
strictly per-PDK.

## Entry anatomy (v0 sketch; full standard pending)

```text
<entry>/
├── entry_repo/   # nested upstream checkout, ONLY if wrapping one
└── rocket/       # maintained rocket-compatible adapter
    ├── meta.yaml # name, version, upstream url+rev+license, kind, ports, links
    └── adapt.*   # conversion into engine-consumable artifacts
```

Entry folders are slugs (`lowercase-with-dashes`), unique within this PDK.

## Install the PDK

- gdsfactory package: [quantum-rf-pdk](https://github.com/gdsfactory/quantum-rf-pdk)
  ([docs](https://gdsfactory.github.io/quantum-rf-pdk/)) —
  pip-installable per its README.
