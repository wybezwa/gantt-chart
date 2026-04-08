# Sander Roadmap — Next 2 Months (W14–W22)

> Auto-generated from `gantt_data.json` on 2026-04-08 15:52
> Calendar range: 2026-03-30 to 2026-05-31

## Milestones

- **Go/No-Go Gate** — 2026-04-19

## Design & Planning

| ID | Task | Project | System Level | Owner | End | Days | Priority | Status | Depends On |
|:---|:-----|:--------|:-------------|:------|:----|-----:|:--------:|:------:|:-----------|
| T1 | Confirmed controller path (decision document) | BB1-XX | Harvester controller system | Wybe | 2026-04-15 | 2 | H | ✅ | — |
| T2 | Initial controller architecture | BB1-XX | Harvester controller system | Wybe | 2026-04-19 | 10 | M | ✅ | T1 |
| T3 | Spark basic system design | Spark | Total system | Sander | 2026-04-24 | 10 | H | ✅ | — |
| T4 | Spark mechanical design decisions | Spark | Mechanical system | Sander | 2026-04-19 | 10 | M | ✅ | — |
| T5 | Spark critical parts finalised | Spark | Total system | Sander | 2026-05-01 | 5 | H | ✅ | — |
| T7 | Total system validation planning | Spark | Total system | Sander | 2026-05-15 | 5 | M | ✅ | — |
| T12 | BB improvement list & quick studies | BB1-XX | Total system |  | 2026-04-11 | 5 | H | ✅ | — |
| T34 | Detailed design Spark ready and ordered | Spark | Mechanical system | Sander | 2026-05-08 | 5 | H | ✅ | — |
| T35 | EEC design finished and ordered |  |  | Mathijs | 2026-04-17 | 5 | M | ✅ | — |
| T36 | Main architecture EWS + Spark | Spark | Total system |  | 2026-05-01 | 10 | M | ✅ | — |

## Hardware Deliveries

| ID | Task | Project | System Level | Owner | End | Days | Priority | Status | Depends On |
|:---|:-----|:--------|:-------------|:------|:----|-----:|:--------:|:------:|:-----------|
| T8 | MBD board (ordered → delivered) |  |  | Mathijs | 2026-04-08 | 14 | M | ✔️ | — |
| T9 | MB board (ordered → delivered) |  |  | Mathijs | 2026-04-08 | 14 | M | ✔️ | — |
| T10 | EEC board (ordered → delivered) |  |  | Mathijs | 2026-05-01 | 14 | M | ✅ | — |
| T11 | Spark parts (ordered → delivered) | Spark | Total system | Sander | 2026-05-20 | 21 | H | ✅ | T34 |
| T39 | BB1-V3 order parts (ordered → delivered) | BB1-XX | Mechanical system | Sander | 2026-05-20 | 21 | M | ✅ | — |

## Assembly & Build

| ID | Task | Project | System Level | Owner | End | Days | Priority | Status | Depends On |
|:---|:-----|:--------|:-------------|:------|:----|-----:|:--------:|:------:|:-----------|
| T15 | BB-1V2 assembly (DC motor) | BB1-XX | Mechanical system | Ernst | 2026-04-03 | 5 | H | ✔️ | — |
| T16 | Initial mechanical Spark assembly | Spark | Mechanical system | Ernst | 2026-05-22 | 5 | M | ✅ | T11 |
| T37 | Total integrated Spark assembly | Spark | Total system | Sander | 2026-05-27 | 5 | M | ✅ | — |
| T38 | BB1-V3 assembly | BB1-XX | Mechanical system | Ernst | 2026-04-24 | 3 | M | ✅ | — |

## Testing & Validation

| ID | Task | Project | System Level | Owner | End | Days | Priority | Status | Depends On |
|:---|:-----|:--------|:-------------|:------|:----|-----:|:--------:|:------:|:-----------|
| T17 | BB-1V2 full system validation (EH+EEC) |  |  |  |  | 0 | M | ✅ | — |
| T18 | MBD actuator testing |  |  |  |  | 0 | M | ✅ | — |
| T19 | EEC upgrade results evaluated |  |  |  |  | 0 | M | ✅ | — |
| T20 | MB validation |  |  |  |  | 0 | M | ✅ | — |
| T21 | EEC validated |  |  |  |  | 0 | M | ✅ | — |
| T22 | First integrated test (ctrl+fw+EEC) |  |  |  |  | 0 | M | ✅ | — |
| T23 | First EWS-BEH power measurement test |  |  |  |  | 0 | M | ✅ | — |
| T24 | Controller continued testing |  |  |  |  | 0 | M | ✅ | — |
| T25 | First data dashboard testing |  |  |  |  | 0 | M | ✅ | — |
| T26 | Delay buffer (controller) |  |  |  |  | 0 | M | ✅ | — |
| T27 | Spark first mechanical testing |  |  |  |  | 0 | M | ✅ | — |
| T28 | First Spark + Controller system test |  |  |  |  | 0 | M | ✅ | — |
| T29 | Further Spark mechanical testing |  |  |  |  | 0 | M | ✅ | — |
| T30 | Full integrated test (Mech+EEC+Ctrl) |  |  |  |  | 0 | M | ✅ | — |
| T31 | Final total system test + endurance |  |  |  |  | 0 | M | ✅ | — |
| T32 | Full system test with EWS-B + server |  |  |  |  | 0 | M | ✅ | — |

## Firmware & Software

| ID | Task | Project | System Level | Owner | End | Days | Priority | Status | Depends On |
|:---|:-----|:--------|:-------------|:------|:----|-----:|:--------:|:------:|:-----------|
| T13 | First firmware for MB validation | Spark | Harvester controller system | Niels | 2026-04-17 | 5 | M | ✅ | — |
| T14 | Detailed controller firmware ready to test | Spark | Harvester controller system | Niels | 2026-05-01 | 5 | M | ✅ | — |
| T6 | EWS dashboard requirements defined | Spark | EWS-B | Thijs | 2026-05-01 | 5 | M | ✅ | — |

---

*This file is auto-generated. Edit `gantt_data.json` and push to update.*
