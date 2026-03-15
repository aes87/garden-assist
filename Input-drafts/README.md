# Garden Project — Warren County NJ 2026

## Project Overview

Home vegetable garden plan for two 4×12 raised beds (12" depth) in Warren County, NJ (Zone 6b). Part shade conditions (~5-6 hours midday sun). Last frost ~May 10-15.

This repo contains planning documents, an interactive HTML planner, and build guides. The primary deliverable is `garden-hq.html` — a self-contained single-page app with bed layouts, planting timeline, persistent shopping checklist, and groundhog fence build instructions.

## Site Conditions

- **Location:** Warren County, NJ. Zone 6b. Last frost ~May 12.
- **Beds:** Two 4'×12' raised beds, ~12" depth, oriented roughly east-west (±15°)
- **Sun:** ~5-6 hours direct midday sun (11am-3pm window). House blocks morning sun from the east. Dense evergreen tree wall blocks late afternoon sun from west/northwest. Shade is year-round (evergreens, not deciduous).
- **Soil:** 2+ year aged compost available. Standard raised bed soil.
- **Wildlife:** Active groundhog population. Exclusion fencing required before any outdoor planting.

## Layout Strategy

### Bed 1 — "Tomato Bed"
- South 2/3: 6 tomato plants at 24" spacing (2 cherry + 4 heirloom), staked/pruned to 1-2 leaders
- North 1/3: shade-tolerant understory (basil, parsley, chard, lettuce as living mulch)
- Middle flex zone: usable early season, goes fallow under tomato canopy shade by July
- **Cross-shade note:** Tomatoes on south edge will shade everything behind them by midsummer. This is intentional — north side is planned for shade-tolerant companions.

### Bed 2 — "Everything Else"
- North edge: tall crops (kale ×3, pea trellis) — won't shade anything behind them
- Middle: brassicas (broccoli ×2, cabbage ×1, cauliflower ×2, kohlrabi ×4) at 18-24" spacing
- South edge: low-growing greens and roots (lettuce, spinach, arugula, beets, carrots, radishes, scallions)
- Bush beans: 6 sq ft, one main sowing + optional second

### Plant Count (~35 transplants + direct-sown seed)
- 6 tomatoes: Sungold, Black Cherry, Juliet, Black Krim, Stupice, Cherokee Purple
- 12 brassicas: 2 broccoli, 1 cabbage, 2 cauliflower, 3 kale, 4 kohlrabi
- 2 chard, 4 basil, 2 parsley
- ~40 peas (spring only), ~54 bush beans
- Direct-sown: lettuce, spinach, arugula, radishes, beets, carrots, scallions, cilantro

## Key Timing

| When | Action |
|------|--------|
| Mar 14-16 | Start brassicas + lettuce indoors (soil blocks) |
| Mar 28-Apr 1 | Start tomatoes, chard, parsley indoors |
| Apr 1-15 | BUILD GROUNDHOG FENCE |
| Apr 10-20 | Direct sow cool-season crops outdoors |
| Apr 15-20 | Start basil indoors |
| Late Apr | Transplant brassicas outdoors |
| Early May | Direct sow bush beans |
| May 20-25 | Transplant tomatoes + basil |
| Early Jun | Resow #2: greens, radishes |
| Mid Jul | Pull peas, optional resow #3 |

## Groundhog Fence Spec

- Single enclosure around both beds, ~64' perimeter
- 2"×4" welded wire fencing, 4' tall above grade
- 12" deep trench with L-apron (hardware cloth or bent welded wire) extending 12" outward
- 12" wobble top (unattached, bends outward) to defeat climbers
- 14 T-posts, gate on house side
- **Recommended:** Rent walk-behind trencher (~$175/day) vs manual dig
- Must be complete before outdoor planting begins (mid-April)

## File Structure

```
garden-2026/
├── README.md              ← This file
├── garden-hq.html         ← All-in-one interactive planner (open in browser)
│                             Tabs: Bed Layout, Timeline, Shopping Checklist, Fence Build
│                             Shopping list has persistent checkboxes (localStorage)
├── garden-shopping-v2.xlsx ← Spreadsheet version of shopping list (3 tabs)
├── groundhog-fencing-guide.md ← Standalone fence build guide (detailed)
└── garden-plan.md          ← Original text-based garden plan (reference)
```

## Development Notes

- `garden-hq.html` is fully self-contained — no build step, no dependencies, no framework. Opens in any browser. Uses Google Fonts (DM Sans + DM Mono) loaded via CDN.
- Shopping checklist state is persisted via `localStorage` under key `gardenChecklist2026`. Survives browser refresh. Reset button clears all checks.
- Bed layout grid uses CSS Grid with `span` classes for zone sizing. Each zone represents a planting area (NOT one plant per cell). Click any zone for variety, spacing, and timing details.
- Color scheme: dark green/earth tones. Category colors: tomatoes (red), brassicas (blue), greens (green), roots (brown), herbs (purple), legumes (yellow), alliums (pink).

## Maintenance / Future Work

- [ ] Add actual bed spacing dimensions once measured
- [ ] Update fence enclosure footprint with real measurements
- [ ] Track seed germination dates and actual transplant dates
- [ ] Add fall planting schedule (August starts)
- [ ] Photo documentation of build progress
- [ ] End-of-season yield notes for shade-performance data
- [ ] Consider adding a soaker hose / drip irrigation plan
