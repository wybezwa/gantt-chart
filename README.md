# Gantt Chart

Interactive Gantt chart for project planning, hosted on GitHub Pages.

## View

**[Open Gantt Chart](https://wybezwa.github.io/gantt-chart/)**

## Quick Start

**Setup (one time):**

```bash
git clone https://github.com/wybezwa/gantt-chart.git
```

**Edit the roadmap:**

1. Open the [Gantt Chart](https://wybezwa.github.io/gantt-chart/) in Chrome or Edge
2. Click any cell to edit — tasks, dates, days, priority, status are all inline-editable
3. Use dropdowns for Project, Owner, Priority, Status, and Dependencies

**Save your changes:**

1. Click **💾 Save to File** (top-right)
2. First time: navigate to your cloned `gantt-chart` folder and select `gantt_data.json`
3. Next saves in the same session are instant (one click)

**Deploy:**

```bash
cd gantt-chart
git add gantt_data.json
git commit -m "Update roadmap"
git push
```

The page updates automatically within ~30 seconds.

**Tips:**

- **↺ Reset** clears browser-cached edits and reloads the latest deployed data
- Bars are drawn backwards from the **End date** by the number of **Days**
- The **Deps** column lets you pick predecessor tasks — arrows show on the chart

## Local preview

```bash
python generate_gantt_html.py
# Open index.html in browser
```

## Features

- Color-coded bars by category
- Inline editing (click any cell)
- Owner, Priority, Status, Dependencies dropdowns
- Milestone and today lines
- Save to File button for persisting edits
- Hardware delivery waiting period visualization
- Workload summary and current priorities view
- Project filtering
