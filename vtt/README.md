# VTT — rocket-blocks

VTT (Finland) photonic PDK. Domains: photonic.
Upstream PDK: [gdsfactory/vtt](https://github.com/gdsfactory/vtt)

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
