<!-- SPDX-License-Identifier: CC-BY-4.0 -->
# Memory Format — roadmap

The format has no goals of its own. It is planned as part of the MemHouse roadmap,
[`docs/roadmap.md`](https://github.com/memhousehq/memhouse/blob/main/docs/roadmap.md) in the
monorepo, which numbers every goal (`G01`, `G02`, …). This file lists the goals that touch the
format, and is updated when one of them lands.

The format is developed in the monorepo (`memory-format/` and `docs/memory-format.md`) and
tested there; changes land there first and are then brought here.

## Status

| Version | State | Since |
|---|---|---|
| 1 | superseded; still readable ([SPEC.md § Version 1](SPEC.md#version-1)) | — |
| 2 | **current**: records, versions, provenance, labels, scopes, links, policies and decision values; 14 conformance vectors | G04 (2 November 2026) |

## Goals that touch the format

| Goal | What it means for the format | State |
|---|---|---|
| G04 — Logical schema v2 and Memory Format v2 | Memory Format v2 and its conformance vectors | done (2 November 2026) |
| G09 — Open-source publication | this repository split out of the monorepo with its history | done (3 November 2026) |
| — | CI: manifest coverage and conformance against the reference reader (#1) | done (5 November 2026) |
| G16 — Lite profile: embedded store | a second implementation that must read and write the format | planned |
| G17 — Profile migration | migration goes through export and import; "Done when" is a round trip identical by record hashes | planned |
| G23 — Context-provider plugin system, connectors and importers | importers from other systems map onto the format | planned |
| G28 — Access Policy Decision Register | export and import of access-policy decisions (v2 already carries decision values) | planned |

A goal that changes the format bumps its version in [SPEC.md](SPEC.md), adds conformance vectors
for the change and keeps every earlier version readable.
