# Garden Assist

## Overview
Home vegetable garden planning project for Warren County, NJ (Zone 6b, 2026 season). Two 4x12 raised beds in part shade (~5-6 hrs sun). Covers bed layouts, planting timelines, shopping lists, and groundhog exclusion fencing.

## Tech Stack
- Language: HTML/CSS/JS (self-contained single-page app)
- No build step, no framework, no dependencies
- Google Fonts (DM Sans + DM Mono) loaded via CDN
- Shopping list persistence via localStorage

## Project Structure
```
garden-assist/
├── CLAUDE.md              ← This file
├── README.md              ← Project overview and quick reference
├── app/
│   └── garden-hq.html     ← Interactive planner SPA (open in browser)
│                             Tabs: Bed Layout, Timeline, Shopping Checklist, Fence Build
├── planning/
│   ├── garden-plan.md      ← Full text garden plan (varieties, timing, soil, care)
│   └── garden-shopping-v2.xlsx ← Spreadsheet shopping list (3 tabs)
├── guides/
│   └── groundhog-fencing-guide.md ← Detailed fence build guide
├── docs/                   ← Future: photos, measurements, yield tracking
└── Input-drafts/           ← Original source files (reference only, do not edit)
```

## Key Details
- **Location:** Warren County, NJ. Zone 6b. Last frost ~May 12.
- **Beds:** Two 4'x12' raised beds, 12" depth, east-west orientation
- **Sun:** ~5-6 hours direct midday sun. Evergreen shade from west, house shade from east.
- **Wildlife:** Groundhog exclusion fence required before any outdoor planting (mid-April deadline)
- **localStorage key:** `gardenChecklist2026` (shopping checklist state)

## Conventions
- garden-hq.html is the primary deliverable — keep it self-contained (no external JS/CSS deps beyond fonts)
- Markdown files in planning/ and guides/ are reference docs, not generated from the app
- Input-drafts/ is read-only archive of original Claude session outputs
- Plant spacing, timing, and variety data should stay consistent across all files

## When Working Here
1. Open `app/garden-hq.html` in a browser to see the interactive planner
2. Reference `planning/garden-plan.md` for detailed variety/timing info
3. If updating plant data, ensure consistency across the HTML app and markdown docs
4. Keep the HTML self-contained — no build tools or npm
