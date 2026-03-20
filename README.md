# Garden Assist

Everything you need to run two raised beds in Zone 6b — bed layouts, planting timelines, germination protocols, a persistent shopping checklist, and a groundhog exclusion fence that actually works. All in one HTML file, no dependencies.

This is a personal garden planning toolkit for Warren County, NJ (2026 season). Two 4×12-foot beds, 12 inches deep, part shade — about 5–6 hours of midday sun. The beds sit in a mixed-shade zone between evergreens and the house, so crop selection leans hard on shade-tolerant varieties.

**[Open the planner →](https://aes87.github.io/garden-assist/app/garden-hq.html)**

## What It Does

- **Interactive bed layouts** — visual grid for both beds with clickable plant details, color-coded by crop family. Bed 1 is tomatoes + shade-tolerant understory; Bed 2 is everything else.
- **Planting timeline** — chronological schedule from March seed starts through fall harvest, tagged by action type (indoor, outdoor, transplant, resow)
- **Germination guide** — 3-wave indoor seed start system with block counts, heat mat rotation, tray cross-sections, and a troubleshooting section for when things go sideways
- **Persistent shopping checklist** — checkboxes saved to localStorage, progress bar, organized by category, cross-referenced against seed packs already on hand
- **Groundhog exclusion fence** — step-by-step build with buried L-apron, wobble top, and gated entry. Call 811 first.
- **Season-long growing guide** — month-by-month maintenance from May through October, plus a "lazy minimum" section for when life gets busy

## Quick Start

Open `app/garden-hq.html` in any browser. That's it — self-contained HTML, no build step, no install.

## How It Works

A single 880-line HTML file with six tabs. All styling and logic inline. Shopping checklist state persists via `localStorage` (`gardenChecklist2026` key). Dark theme, responsive down to mobile, Google Fonts via CDN.

The supporting Markdown docs — garden plan, fencing guide — are the research and reference material that fed the app. The `Input-drafts/` directory is a read-only archive of the original source files.

## Key Dates

| When | Action |
|:-----|:-------|
| Mar 14–16 | Start brassicas + lettuce indoors (Wave 1 — 27 soil blocks) |
| Mar 28–Apr 1 | Start tomatoes, chard, parsley (Wave 2 — 19 blocks) |
| Apr 1–15 | Build groundhog fence |
| Apr 10–20 | Direct sow cool-season crops outdoors |
| Apr 15–20 | Start basil indoors (Wave 3 — 6 blocks) |
| May 20–25 | Transplant tomatoes + basil after last frost |

## Project Structure

```
app/                  Interactive HTML planner (primary deliverable)
planning/             Garden plan details, shopping spreadsheet
guides/               Groundhog fencing build guide
docs/                 Photos, measurements, yield tracking (future)
Input-drafts/         Original source files (read-only archive)
```

## Site Conditions

- **Zone 6b** — last frost ~May 12
- **Part shade** — 5–6 hours direct midday sun, evergreen + house shade on north side
- **Groundhog pressure** — exclusion fence required before any outdoor planting
- **Soil** — 2-year aged compost available for top-dressing

## License

MIT
