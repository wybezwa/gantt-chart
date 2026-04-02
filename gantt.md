# Sander Roadmap — Next 2 Months (W14–W22)

> Auto-generated from `gantt_data.json` on 2026-04-02 09:57
> Calendar range: 2026-03-30 to 2026-05-31

## Milestones

- **Go/No-Go Gate** — 2026-04-19

## Design & Planning

| ID | Task | Person(s) | Start | Days | Effort | Difficulty | Status | Depends On |
|:---|:-----|:----------|:------|-----:|:------:|:----------:|:------:|:-----------|
| T1 | Confirmed controller path (decision) | Sander | 2026-04-06 | 5 | M | H | ✅ | — |
| T2 | Initial controller architecture | Sander | 2026-04-13 | 5 | L | M | ✅ | — |
| T3 | Spark basic system design | Sander | 2026-04-20 | 5 | L | M | ✅ | — |
| T4 | Spark mechanical design decisions | Sander | 2026-04-20 | 5 | M | H | ✅ | — |
| T5 | Spark critical parts finalised | Sander | 2026-04-27 | 5 | M | M | ✅ | — |
| T6 | EWS dashboard requirements defined | Sander | 2026-04-27 | 5 | S | H | ✅ | — |
| T7 | Total system validation planning | Sander | 2026-05-11 | 5 | M | H | ✅ | — |

## Hardware Deliveries

| ID | Task | Person(s) | Start | Days | Effort | Difficulty | Status | Depends On |
|:---|:-----|:----------|:------|-----:|:------:|:----------:|:------:|:-----------|
| T8 | MBD board (ordered → delivered) | Camilo, Ernst, Nathan | 2026-03-25 | 10 | S | H | ✅ | — |
| T9 | MB board (ordered → delivered) | Sander | 2026-03-28 | 14 | S | M | ✅ | — |
| T10 | EEC board (ordered → delivered) | Sander | 2026-04-13 | 15 | S | M | ✅ | — |
| T11 | Spark parts (ordered → delivered) | Sander | 2026-04-29 | 17 | S | M | ✅ | — |

## Firmware & Software

| ID | Task | Person(s) | Start | Days | Effort | Difficulty | Status | Depends On |
|:---|:-----|:----------|:------|-----:|:------:|:----------:|:------:|:-----------|
| T12 | BB improvement list & quick studies | Sander | 2026-04-06 | 5 | M | H | ✅ | — |
| T13 | First firmware for MB validation | Sander | 2026-04-13 | 5 | L | M | ✅ | — |
| T14 | More firmware ready | Sander | 2026-04-27 | 5 | M | M | ✅ | — |

## Assembly & Build

| ID | Task | Person(s) | Start | Days | Effort | Difficulty | Status | Depends On |
|:---|:-----|:----------|:------|-----:|:------:|:----------:|:------:|:-----------|
| T15 | BB-1V2 assembly (DC motor) | Sander, Wybe | 2026-03-30 | 5 | M | H | ✅ | — |
| T16 | Spark assembly | Sander | 2026-05-18 | 5 | L | M | ✅ | T11 |

## Testing & Validation

| ID | Task | Person(s) | Start | Days | Effort | Difficulty | Status | Depends On |
|:---|:-----|:----------|:------|-----:|:------:|:----------:|:------:|:-----------|
| T17 | BB-1V2 full system validation (EH+EEC) | Sander | 2026-03-30 | 5 | M | H | ✅ | — |
| T18 | MBD actuator testing | Sander, Wybe | 2026-03-30 | 5 | M | H | ✅ | — |
| T19 | EEC upgrade results evaluated | Sander | 2026-04-06 | 5 | S | H | ✅ | — |
| T20 | MB validation | Sander | 2026-04-13 | 5 | M | M | ✅ | T9, T13 |
| T21 | EEC validated | Sander, Thijs | 2026-05-04 | 5 | M | M | ✅ | T10 |
| T22 | First integrated test (ctrl+fw+EEC) | Sander | 2026-05-04 | 5 | L | M | ✅ | T21, T14 |
| T23 | First EWS-BEH power measurement test | Sander | 2026-05-04 | 5 | M | M | ✅ | — |
| T24 | Controller continued testing | Sander, Wybe | 2026-05-11 | 5 | M | H | ✅ | T22 |
| T25 | First data dashboard testing | Sander | 2026-05-11 | 5 | M | M | ✅ | T6 |
| T26 | Delay buffer (controller) | Sander, Thijs | 2026-05-11 | 5 | S | H | ✅ | — |
| T27 | Spark first mechanical testing | Sander, Thijs | 2026-05-18 | 5 | M | M | ✅ | T16 |
| T28 | First Spark + Controller system test | Sander | 2026-05-18 | 5 | L | L | ✅ | T27, T24 |
| T29 | Further Spark mechanical testing | Sander | 2026-05-25 | 5 | M | M | ✅ | T27 |
| T30 | Full integrated test (Mech+EEC+Ctrl) | Sander | 2026-05-25 | 5 | L | L | ✅ | T28 |
| T31 | Final total system test + endurance | Sander | 2026-05-25 | 5 | L | L | ✅ | T30 |
| T32 | Full system test with EWS-B + server | Sander | 2026-05-25 | 5 | L | L | ✅ | T30, T25 |

---

*This file is auto-generated. Edit `gantt_data.json` and push to update.*
