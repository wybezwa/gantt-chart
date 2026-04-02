# Gantt Chart – How to Use

## Quick Start

**[Open the Gantt Chart](https://wybezwa.github.io/gantt-chart/)** in your browser.

All editing happens inline — click any cell to modify it.

## Columns

| Column | How to edit | Description |
|--------|------------|-------------|
| **ID** | Read-only | Auto-assigned task identifier (T1, T2, ...) |
| **Task** | Click to type | Task name or description |
| **Person(s)** | Click → checkboxes | Assign one or more people to a task |
| **Start** | Click to type | Start date in `YYYY-MM-DD` format |
| **Days** | Click to type | Duration in calendar days |
| **Effort** | Dropdown | S = Small (½ day), M = Medium (1–3 days), L = Large (week+) |
| **Diff.** | Dropdown | Difficulty: H = Hard (red), M = Medium (yellow), L = Easy (green) |
| **Deps** | Click → checkboxes | Select predecessor tasks by ID. Arrows show dependencies on the chart |
| **Status** | Dropdown | On Track (green), Delayed (red), Done (blue), Not Needed (grey) |

## Status Effects

| Status | Bar effect | Text effect |
|--------|-----------|-------------|
| **On Track** | Full opacity | Normal |
| **Delayed** | 50% opacity | Normal |
| **Done** | 60% opacity | Blue text |
| **Not Needed** | 20% opacity | Strikethrough, grey |

## Saving Your Changes

### Option 1: Save to File (recommended)
Click **💾 Save to File**. The first time, you'll be asked to pick a location — navigate to your local clone of the `gantt-chart` repo and save as `gantt_data.json`. Subsequent saves in the same browser session write to the same file instantly.

### Option 2: Download JSON
Click **⬇ Download JSON** to download the file. Then manually replace `gantt_data.json` in the repo.

### After saving
1. `git add gantt_data.json`
2. `git commit -m "Update Gantt chart"`
3. `git push`

GitHub Actions will auto-regenerate `index.html` and `gantt.md` from the updated JSON.

## Workload Summary

Below the chart you'll find a **Workload Summary** showing each person's load:
- Score = `days × difficulty weight` (L=1, M=2, H=3)
- For multi-person tasks, the load is split equally
- Bars colored from green (low load) to red (high load)
- Shows task count and total days per person

## Dependency Arrows

When tasks have dependencies set (via the **Deps** column), arrows are drawn on the chart from the end of the predecessor bar to the start of the dependent bar.

- Arrows update automatically when you change start dates, durations, or dependencies
- Arrows redraw on scroll and window resize

## Local Preview

To preview changes locally without pushing:

```bash
python generate_gantt_html.py
# Open index.html in your browser
```

This also generates `gantt.md` — a markdown companion file with the same data as a readable table.

## Markdown Companion

The file `gantt.md` is auto-generated alongside `index.html`. It contains all tasks in markdown tables, grouped by category. Colleagues who prefer reading markdown (or viewing in Git) can use this file instead of the interactive chart.

## Files

| File | Purpose |
|------|---------|
| `gantt_data.json` | Source data — edit this (or use the web UI) |
| `generate_gantt_html.py` | Generator script — produces `index.html` + `gantt.md` |
| `index.html` | Interactive Gantt chart (auto-generated) |
| `gantt.md` | Markdown table view (auto-generated) |
| `.github/workflows/gantt.yml` | GitHub Actions — auto-regenerates on push |

## Browser Storage

Changes made in the browser are auto-saved to `localStorage`. This means:
- Your edits persist across page reloads
- Click **↺ Reset** to discard browser edits and reload the original data
- Browser edits are local only — use **Save to File** or **Download JSON** to commit them
