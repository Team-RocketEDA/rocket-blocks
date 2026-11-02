# GF180MCU — rocket-blocks

GlobalFoundries 180nm MCU CMOS. Domains: digital, analog/mixed-signal, high-voltage.
Upstream PDK: [google/gf180mcu-pdk](https://github.com/google/gf180mcu-pdk) · [open_pdks](https://github.com/RTimothyEdwards/open_pdks) · [gdsfactory/gf180mcu](https://github.com/gdsfactory/gf180mcu)

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

## Install the PDK

- From source: [open_pdks](https://github.com/RTimothyEdwards/open_pdks)
  (builds from [gf180mcu-pdk](https://github.com/google/gf180mcu-pdk)) —
  follow its README.
- Prebuilt: [volare](https://github.com/efabless/volare), the PDK version
  manager used by OpenLane/LibreLane.
- gdsfactory package: [gf180mcu](https://github.com/gdsfactory/gf180mcu)
  ([docs](https://gdsfactory.github.io/gf180mcu/)) — pip-installable per
  its README.
