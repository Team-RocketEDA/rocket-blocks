# SKY130 — rocket-blocks

SkyWater 130nm CMOS. Domains: digital, analog/mixed-signal.
Upstream PDK: [google/skywater-pdk](https://github.com/google/skywater-pdk) · [open_pdks](https://github.com/RTimothyEdwards/open_pdks) (sky130A/B variants) · [gdsfactory/skywater130](https://github.com/gdsfactory/skywater130)

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
  (builds from [skywater-pdk](https://github.com/google/skywater-pdk)) —
  follow its README.
- Prebuilt: [volare](https://github.com/efabless/volare), the PDK version
  manager used by OpenLane/LibreLane.
- gdsfactory package: [skywater130](https://github.com/gdsfactory/skywater130)
  ([docs](https://gdsfactory.github.io/skywater130/)) — pip-installable
  per its README.
