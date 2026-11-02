# Luxtelligence GF (lxt_pdk_gf) — rocket-blocks

Luxtelligence GlobalFoundries photonic PDK. Domains: photonic.
Upstream PDK: [Luxtelligence/lxt_pdk_gf](https://github.com/Luxtelligence/lxt_pdk_gf) · [docs](https://luxtelligence.github.io/lxt_pdk_gf/)

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

## Install the PDK

- Package: [lxt_pdk_gf](https://github.com/Luxtelligence/lxt_pdk_gf)
  ([docs](https://luxtelligence.github.io/lxt_pdk_gf/)) —
  pip-installable per its README.
