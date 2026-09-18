---
title: Cost + sizing models
description: Sensor BOM options and powerpack sizing workbook.
---

- `cost model.xlsx` — sensor BOM comparison: Sensor IC / op-amps / resistors /
  PCB + flex / bias magnet / harness+header across architectures
  (end-mount SINCOS, front-mount Sensitec GT / Multi-Dimension GT / NVE GT, MSB variants;
  AS5215 / AL803 / MMGX45 / ABL015 / LMV344; 10K; power FR4 / 2-layer FR4; target material + labor).
- `Powerpack sizing ratio 26jn14.xlsx` — CEPS/REPS ratio sizing: rack/pinion loads (kN),
  stack length, turns, stall + battery current, controller + motor resistance,
  wires-in-hand, rev/rev and rev/mm, standard/premium/optimal + upsized-controller/motor cases
  (100/120/125/155 A battery).

:::note[Models, not gospel]
Workbooks capture June-2014-era assumptions. Use them to understand trades
(ratio vs. current vs. resistance vs. package), then re-run with current inputs.
:::

## Sources

| Original file | Size | Type |
|---|---|---|
| `supporting material/cost model.xlsx` | 15 KB | XLSX |
| `supporting material/Powerpack sizing ratio 26jn14.xlsx` | 36 KB | XLSX |
