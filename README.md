# Electric Power Steering (EPS) — Technical Documentation

> Archive of Nexteer EPS Technology Roadmap work (2014–2016): systems engineering, core mechanical,
> sensors, motor control, electronics, safety, NVH and manufacturing.

[![Docs — Astro Starlight](https://img.shields.io/badge/docs-Astro_Starlight-7c3aed)](./docs)
[![Source formats](https://img.shields.io/badge/sources-pptx_xlsx_pdf_png-blue)](#repository-structure)

## Contents

- [What is this?](#what-is-this)
- [Start here](#start-here)
- [Repository structure](#repository-structure)
- [Content map](#content-map)
- [TRM one-pager index](#trm-one-pager-index)
- [Technology domains](#technology-domains)
- [Docs site (`docs/`)](#docs-site-docs)
- [Working with the original files](#working-with-the-original-files)
- [Contributing](#contributing)

## What is this?

This repo preserves the working documents behind the EPS Technology Roadmap up to **11MY16**
(`Technology Roadmap 11MY16.xlsx`):

- **~120 source files** — mostly `.pptx` one-pagers / deep-dives, plus `.xlsx` models, `.pdf` drawings/timing, one `.png`.
- Organized by subsystem and by **TRM ID** (`TRM-002 … TRM-204`, `CCM-`, `SE-`, `RCM-`, `FE-`, `ES-`).
- Human-readable web version lives in [`docs/`](./docs) as Markdown/MDX.
  Original binaries stay untouched at the repo root.

## Start here

| If you want to… | Go to |
|---|---|
| Understand the program at a glance | [`Technology Roadmap 11MY16.xlsx`](./Technology%20Roadmap%2011MY16.xlsx) + [`docs/src/content/docs/roadmap/`](./docs/src/content/docs/roadmap/) |
| Browse by topic on the web | [`docs/`](./docs) |
| Find a specific technology (e.g. “spring isolators”) | [TRM one-pager index](#trm-one-pager-index), or search in the docs site |
| See LoA / safety classification | [`supporting material/`](./supporting%20material/) → LoA Naming Convention + `Nexteer LoA Types` |
| See cost / sizing models | [`supporting material/cost model.xlsx`](./supporting%20material/cost%20model.xlsx), [`Powerpack sizing ratio 26jn14.xlsx`](./supporting%20material/Powerpack%20sizing%20ratio%2026jn14.xlsx) |
| See presentations for customers / leadership | [`supporting material/Customer presentation/`](./supporting%20material/Customer%20presentation/), [`For Frank/`](./supporting%20material/For%20Frank/), [`Product Team presentation/`](./supporting%20material/Product%20Team%20presentation/) |

## Repository structure

```text
.
├── README.md
├── Technology Roadmap 11MY16.xlsx        # master roadmap to Nov 2016
├── Digital Motor Position/               # 4 pptx — handwheel sensing, probe housing, spur gear
├── DisruptiveTechnology/
│   └── Low Output CEPS/                  # 1 pptx — LO CEPS cost-down stages
├── M.E objectives/                       # 5 pptx + 2016-5-25/ PDF drawing
├── One Pagers/                           # 27 loose files + 39 TRM-xxx folders (~60 files)
│   ├── TRM-002/ … TRM-204/
│   └── *.pptx / *.pdf                    # motor noise, REPS ratio, sensorless, roadmap updates…
├── supporting material/                  # 15 files
│   ├── LoA Naming Convention.png + Nexteer LoA/LoSAS xlsx
│   ├── cost model.xlsx / Powerpack sizing ratio 26jn14.xlsx
│   ├── Customer presentation/ (PSA visit)
│   ├── For Frank/ (EPS TRM updates, NSC review)
│   └── Product Team presentation/
└── docs/                                 # web version — all documentation mirrored in md/mdx
    └── src/content/docs/                 # one section per area above, one page per TRM
```

> Folder names keep their historical spelling (`M.E objectives`, `DisruptiveTechnology`, …)
> so existing links don’t break. The `docs/` site normalizes them
> (`mechanical-engineering-objectives`, `low-output-ceps`, …).

## Content map

| Area | Path | What’s inside |
|---|---|---|
| Digital motor position | [`Digital Motor Position/`](./Digital%20Motor%20Position/) | SGMW digital handwheel sensor sort/reject rate (19MR14, 26MR14), probe-housing signal issue (16AP14), single→dual spur gear |
| Low-output CEPS | [`DisruptiveTechnology/Low Output CEPS/`](./DisruptiveTechnology/Low%20Output%20CEPS/) | Stage I/II cost-down vs baseline CR3005897 (Fiat 319/332): axial sensor, press-press jacket, E/A delete |
| Mechanical engineering | [`M.E objectives/`](./M.E%20objectives/) | VR rack, cut-and-coin BMW rack, hard-turned ball nuts, pinion-skiving simulation (ASME), stop-tooth sensor spline, 29T outer-ball drawing (PDF) |
| One-pagers (loose) | [`One Pagers/`](./One%20Pagers/) | 26× `.pptx` + EA4 timing PDF: 2-step-skew NVH, PMSynRM, REPS ratio, sensorless control, HRLOEPS, ball-nut bearing, torque-sensor dims, Ford CD6, roadmap updates |
| One-pagers (TRM) | [`One Pagers/TRM-*/`](./One%20Pagers/) | One page per technology with Description / Motivation score / Deliverables / Timing / Status / Challenges / Next steps |
| Roadmap master | [`Technology Roadmap 11MY16.xlsx`](./Technology%20Roadmap%2011MY16.xlsx) | 25 sheets — scoring (cost/mass/packaging/performance), timing, applicability |
| Supporting — LoA | [`supporting material/`](./supporting%20material/) | `LoA Naming Convention.png`, `Nexteer LoA Types v1/v2`, `Nexteer LoSAS Types v1` — sensor/current/ECU/inverter redundancy classes |
| Supporting — models | [`supporting material/`](./supporting%20material/) | `cost model.xlsx` (sensor BOM options), `Powerpack sizing ratio 26jn14.xlsx` (CEPS/REPS ratio, stall/battery current) |
| Supporting — decks | [`supporting material/*/`](./supporting%20material/) | PSA customer visit, “For Frank” TRM updates + NSC review, Product-Team tech plans |

## TRM one-pager index

Prefix: **SE** = Systems/Electronics · **CCM** = Core Mechanical · **RCM** = Rack/CEPS Mechanical ·
**FE** = Front-End / sensing · **ES** = Electrical Systems.

| TRM | Topic | TRM | Topic |
|---|---|---|---|
| TRM-002 | SE02 Global Cross Check | TRM-084 | CCM84 Plastic / over-molded pulley |
| TRM-006 | SE06 Arch. modeling tools | TRM-085 | CCM-85 High-output CEPS (>90 Nm) |
| TRM-007 | SE07 Formal safety process | TRM-086 | CCM-86 Plastic CEPS housing |
| TRM-008 | SE08 Arch. + req. traceability | TRM-087 | CCM-87 Short T-bar, no grind (Gen 5) |
| TRM-009 | SE09 Autocoding | TRM-093 | RCM-93 Wrap-up |
| TRM-014 | SE14 Systematic SW protection | TRM-094 | RCM-94 |
| TRM-016 | SE16 Next-gen power management | TRM-109 | CCM-109 Pinion non-delash |
| TRM-019 | SE19 Brush-motor current control (PDF) | TRM-129 | CCM-129 Single isolated-bearing worm |
| TRM-033 | SE33 Motor-sensor tech + cost | TRM-130 | Enhanced FET fault strategy |
| TRM-043 | SE43 Limp-home current sensor | TRM-142 | FE142 Low-cost small-dia. torque sensor |
| TRM-045 | SE45B Limp-home position sensor w/ TC | TRM-143 | RCM-143 updates (×4) |
| TRM-050 | SE50 Torque-steer compensation | TRM-152 | ES152 Reverse-battery FET removal |
| TRM-077 | CCM-77 Eccentric worm | TRM-155 | SE155 Inverter LoA mitigation HW |
| TRM-078 | CCM-78 Spring isolators | TRM-162 | 48 V prototype (FCA request) |
| TRM-081 | CCM-81 Short T-bar, profile grind (Gen 4) | TRM-166 | CCM-166 PSA 2 stop-tooth shafts |
| TRM-082 | CCM-82 Shorter flex coupling | TRM-171 | Axial-sensor stators + sensor cost |
| TRM-083 | CCM-83 15° skew | TRM-174 | CCM-174 Zero-lash spur gear |
| — | — | TRM-175 | Sensor cost info 11MY16 |
| — | — | TRM-177 | Motor friction update |
| — | — | TRM-203 | RCM-203 Boot protection |
| — | — | TRM-204 | Over-molded plastic pulley |

Each TRM folder keeps its original deck(s); the `docs/` mirror gives each TRM its own
searchable page with key points, status/challenges/next steps and a source-file table.

## Technology domains

Covered across the archive: **Manufacturing** (hard-turn, skiving, cut-and-coin, plastic housing/pulley) ·
**Mechanical** (worm/rack/pinion, T-bar, couplings, boots, bearings) ·
**Motor control** (sensorless, PMSynRM, 2-step skew, current control) ·
**NVH** (skew/isolators/eccentric worm, friction) ·
**Electronic** (ECU/inverter, FET faults, reverse battery, power management) ·
**Safety** (ASIL/global cross-check, LoA/LoSAS, limp-home, redundancy, traceability).

## Docs site (`docs/`)

The [`docs/`](./docs) folder mirrors the whole archive as searchable Markdown/MDX:
one section per area above, one page per TRM, topic pages for loose decks,
reference pages (glossary, file index). Each page carries its figures and a
**Sources** table with the exact original filename + size. Originals are
**not** duplicated as binaries except small shared assets.

## Working with the original files

- Formats: PowerPoint (`.pptx`, two legacy `.ppt`), Excel (`.xlsx`), PDF, PNG.
  No special tooling is needed — PowerPoint/LibreOffice + Excel + any PDF viewer.
- File names keep author/date stamps (`… 19MR14`, `…_KleinauV2`, `… 02SE15`) — the `docs/`
  pages normalize titles but always list the exact source filename + size.
- Large decks (e.g. `TRM-130` FET strategy, 44 slides; `REPS Ratio`, 10 slides) are summarized
  per-section in `docs/` so you don’t have to open the binary to get the point.

## Contributing

1. Keep originals immutable — put narrative/edits in `docs/src/content/docs/` (MD/MDX).
2. One TRM = one docs page; loose decks grouped by topic (noise/NVH, sensors, safety, …).
