# Gantt Chart

Interactive Gantt chart for project planning, hosted on GitHub Pages.

## View

**[Open Gantt Chart](https://wybezwa.github.io/gantt-chart/)**

## Update

1. Edit `gantt_data.json` (task data)
2. Push to `main`
3. GitHub Actions auto-regenerates `index.html`
4. The page updates within ~30 seconds

## Local preview

```bash
python generate_gantt_html.py
# Open index.html in browser
```

## Features

- Color-coded bars by category
- Inline editing (click any cell)
- Person, Effort, Confidence dropdowns
- Milestone and today lines
- Export JSON button for saving edits
- Hardware delivery waiting period visualization
