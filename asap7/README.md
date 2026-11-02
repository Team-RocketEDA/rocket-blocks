# ASAP7 — rocket-blocks

ASAP7 7nm FinFET (academic/predictive, ASU). Domains: digital.
Upstream: [asap7sc7p5t standard cells](https://github.com/The-OpenROAD-Project/asap7sc7p5t) (OpenROAD mirror of the kit)

Status: empty, awaiting seeding.

## What goes here

Self-contained entry folders, one per IP block. Per the repo rule: IP
blocks are prebuilt hierarchical schematic blocks (symbol + footprint
linked), strictly per-PDK. Predictive-kit caveat: entries must record
which kit revision they were built against.

## Entry anatomy (v0 sketch; full standard pending)

```text
<entry>/
├── entry_repo/   # nested upstream checkout, ONLY if wrapping one
└── rocket/       # maintained rocket-compatible adapter
    ├── meta.yaml # name, version, upstream url+rev+license, kind, ports, links
    └── adapt.*   # conversion into engine-consumable artifacts
```

Entry folders are slugs (`lowercase-with-dashes`), unique within this PDK.
