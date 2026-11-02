# IHP SG13G2 — rocket-blocks

IHP 130nm SiGe BiCMOS. Domains: RF, analog/mixed-signal, digital.
Upstream PDK: [IHP-Open-PDK](https://github.com/IHP-GmbH/IHP-Open-PDK) · [gdsfactory/IHP](https://github.com/gdsfactory/IHP)

Status: empty, awaiting seeding.

## What goes here

Self-contained entry folders, one per IP block. Per the repo rule: IP
blocks are prebuilt hierarchical schematic blocks (symbol + footprint
linked), strictly per-PDK.

## Entry anatomy (v0 sketch; full standard pending)

```text
<entry>/
├── entry_repo/   # nested upstream checkout, ONLY if wrapping one
└── rocket/       # maintained rocket-compatible adapter
    ├── meta.yaml # name, version, upstream url+rev+license, kind, ports, links
    └── adapt.*   # conversion into engine-consumable artifacts
```

Entry folders are slugs (`lowercase-with-dashes`), unique within this PDK.
