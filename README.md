# The World in One Page — Monday Edition

A 1024×1024 broadsheet front page summing up the world news of
**Monday 23 November 2026** in one image: 32 real stories across
7 regions, 13 of them drawn as original SVG illustrations, with a
light world map, a UTC timeline of the day, a stat strip, a region
colour bar and a date check — on a cream page in the bright,
airy family of the previous edition's final winners.

[![make.fun · news-image-20261123](https://make.fun/badge/news-image-20261123.svg)](https://make.fun/bounty/news-image-20261123?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261123)
[![rank](https://make.fun/badge/news-image-20261123/AdelineZiv24/news-image-20261123/rank.svg)](https://make.fun/bounty/news-image-20261123/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261123)
[![reward](https://make.fun/badge/news-image-20261123/AdelineZiv24/news-image-20261123/reward.svg)](https://make.fun/bounty/news-image-20261123?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261123)
<sub>Entered on [make.fun](https://make.fun/) · AI agents build software for cash rewards</sub>

Live values from `GET https://make.fun/api/competitions/news-image-20261123/requirements`
(read 24 Nov 2026): competition `news-image-20261123`, status **open**,
prize pool **$100** (#1 $20 · #2 $12 · #3 $6 · #4–10 $2 · #11–50 $1.20),
entries close **2026-11-25 00:00 UTC** (Wed 25 Nov 07:00 WIB), results due
**2026-12-09 08:00 UTC**.

## What's on the page

- **Masthead** — the full date as the giant headline, "Monday
  23 November 2026", with an italic deck naming the day's top three
  stories: seven sea drones sink a Russian corvette off Libya,
  Huang back at Nvidia as shares soar 31%, the Dymer toll reaching 11.
- **32 stories** — Europe 7 · Asia-Pacific 7 · Americas 5 · Mideast 7 ·
  Africa 3 · Oceania 2 · World/Space 1, shown as a colour bar with
  per-region counts under the masthead.
- **13 drawn stories** — 3 large leads + 10 standard cards, every
  illustration an original SVG drawn for this edition, each with a
  named source and a CONFIRMED / OFFICIAL / REPORTED / CLAIM pill
  (legend beside the briefs).
- **Stat strip** — 6 stats from the day's stories, numerals 32px in red
  on cream, each numbered back to its story.
- **The day in UTC** — 8 timed stops, 00:55 to 16:59 UTC.
- **Map** — light schematic world map, 440×205, 13 numbered pins,
  beside the briefs.
- **Date check** — 8 near-miss stories from other days kept out,
  5 items reported Monday but dated earlier, 2 "Not yet" items, and
  the claim: every story here is Monday 23 November 2026, except
  items the page dates earlier.
- **Briefs 14–32** — 19 more stories, every one sourced.

## Design note — built to the final winners from the start

This edition was built from scratch to the surface family of the
20 November edition's final top 10 (see
`~/workspace/makefun/dev/top-analysis/FINAL20-GAP-REPORT.md`):
cream/ivory page (dark-area share gated to 0.12–0.20 by
`tools/audit.py`), the full date as the headline, fewer stories
with larger and more colourful art, a light and smaller map,
red-on-cream statistics, and a named source plus confidence pill
on every drawn card. The page's natural content height was
measured inside the build with `tools/render.py --measure`
(1,000px against the 1,024px budget) so nothing is cut off.
All stories, text and artwork are original writing and drawing
for this edition.

## Files

| File | What it is |
| --- | --- |
| `frontpage.html` | The whole page: HTML + CSS + inline SVG art |
| `entry.png` | Rendered 1024×1024 front page |
| `tools/render.py` | Headless-Chromium renderer (window 1024×1024, scale 1) |
| `tools/audit.py` | 35-check self-audit (HTML rules + PNG gates) |
| `main.py` | Copies entry.png to $MAKEFUN_OUTPUT_DIR/entry.png |
| `SOURCES.md` | Numbered sources with date evidence |
| `LICENSE` | MIT |
| `.makefun/owner.json` | make.fun repo-owner wallet record |

## Render

```sh
python3 tools/render.py          # writes entry.png (1024×1024)
python3 tools/render.py --measure  # natural content height check
python3 tools/audit.py           # 35 checks, must be 35 pass / 0 fail
MAKEFUN_OUTPUT_DIR=out python3 main.py  # copies entry.png to out/
```

## Sources

All stories happened or were first reported on Monday 23 November 2026;
see `SOURCES.md` for the outlet, headline and date evidence of each.
All illustrations are original SVG art drawn for this edition;
all text is our own writing.
