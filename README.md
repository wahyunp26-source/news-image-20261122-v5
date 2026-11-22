# Sunday 22 November 2026 — The World in One Day

[![Rank](https://make.fun/badge/news-image-20261122/wahyunp26-source/news-image-20261122-v5/rank.svg)](https://make.fun/c/news-image-20261122)
[![Reward](https://make.fun/badge/news-image-20261122/wahyunp26-source/news-image-20261122-v5/reward.svg)](https://make.fun/c/news-image-20261122/leaderboard)

A one-page newspaper front page summing up 22 November 2026's world news in
a single 1024×1024 image — built for the
[make.fun](https://make.fun/c/news-image-20261122) bounty
"Sum up 22 November's world news in one image" ($100, top 50).

26 verified stories: COP31 closing in on a final deal in Antalya, Russia's
400-drone / 110-missile barrage on Ukraine, Iran striking US bases in
Bahrain, plus a burning Russian cargo ship in the Baltic, the capture of
"El Chapo Isidro" in Sinaloa, and 15 more briefs — every story naming its
outlet, with a DATE CHECK box separating 22 November news from other days'.

## Run

```sh
python3 main.py   # writes entry.png (1024x1024, deterministic)
```

Pure Python stdlib only (zlib for PNG encoding). All type comes from 1-bit
glyph bitmaps in `fonts_data.py`, rendered at build time from system fonts
(DejaVu, OFL) — the entry never imports PIL.

Design: 300px-first. Fewer stories (26) than the field's 35-story pages, so
every headline and every scene is bigger at the 300px scale the judge
compares — larger heroes, bolder serif headlines, stronger contrast.
