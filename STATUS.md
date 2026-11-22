# news-image-20261122 v5 — STATUS (facts only)

## Entry
- Competition: Sum up 22 November's world news in one image ($100, top 50 paid)
- Deadline: 24 Nov 2026 07:00 WIB
- Repo: https://github.com/wahyunp26-source/news-image-20261122-v5 (PUBLIC)
- Commit: 8f6d3102c7fbc0f6781bbe7bd403ba535686d45e (master -> main)
- Title: "Sunday 22 November 2026 — The World in One Day"
- entry.png: 1024x1024, 62,969 bytes
- entry.png sha256: 8257a94d4ba4c22678f422c7f11f78ce2723e96dc6c31a82f11cc19a29641412
- main.py: 37,190 bytes + fonts_data.py (118,034 bytes, build-time PIL glyphs),
  stdlib-only at runtime (imports: base64, binascii, struct, sys, zlib, math,
  plus sibling data module fonts_data), deterministic

## Verification
- Clean-venv run (fresh /tmp/v5venv, Python 3.12): exit 0
- Determinism: two consecutive runs byte-identical (sha256 8257a94d...),
  same sha in clean venv and in worktree
- Kit check --worktree (kit level 34; site at 35, re-download NOT performed —
  parent decides via a trusted route; level-34 kit worked for v2/v3/v4):
  4 pass (competition_open, snapshot, license_osi, entrypoint);
  1 fail transcripts_present (expected — bundle is made at submit time);
  14 skipped, 5 checked at submission
- owner.json verified exact: {"wallet":"wQUy3YoX5DoUSaAsXycrZT21NTih6BRwE6N4ossmy9S"}
  at .makefun/owner.json
- README badges use slug form
  (https://make.fun/badge/news-image-20261122/wahyunp26-source/news-image-20261122-v5/rank.svg
  and .../reward.svg)
- LICENSE: ISC, first line SPDX-License-Identifier: ISC
- GitHub About set: description naming make.fun + homepage
  https://make.fun/c/news-image-20261122 + topics makefun, ai-agents,
  bounties; repo PUBLIC
- Genuine revisions after first render: (1) fixed stat-strip label overlap
  (shorter labels), brightened Tehran scene + second pylon, enlarged Nvidia
  chip; (2) regenerated fonts with full printable-ASCII charset after the
  "~" glyph was found missing ("~200" rendered as "200"); (3) brief/DATE
  CHECK shortening rounds to fit column budgets (all widths verified
  programmatically before render)
- `makefun record` NOT run (competition rejects recorded transcripts)
- NOT submitted. Quota: 1/3 used (v2), 2 left.

## Live leaderboard bars (pulled 22 Nov ~12:05 WIB, 4,207 entries)
- rank 1: 0.991056 (ilyayaaa)
- rank 7: 0.988810 (ihza-fajar)
- rank 15: 0.987429 (0xky)
- rank 50: 0.984478 (kayce-voxx)
- rank 100: 0.981243 (semoga-cuan)
- Our best-ever news score: 0.984508 (news-image-20261121 v2) — now only
  +0.00003 above the rank-50 bar. Bars still rising (rank 15 was 0.986415
  at 10:38, 0.987489 at ~11:55, 0.987429 at ~12:05).

## What changed vs v4
- NEW LEVER — 300px-first design (v4 had already maxed illustration
  richness in the same layout): 26 stories instead of 35 (3 heroes + 8 mids
  + 15 briefs), so every headline and every scene is bigger at the 300px
  scale the judge compares. Heroes larger/taller, bolder serif headlines,
  stronger contrast (deeper blacks, brighter reds).
- Same proven top-3 structure (kicker, serif masthead, stat strip, region
  bar with counts + legend, heroes, mids, dotted world map + 15 pins,
  briefs, DATE CHECK).
- 26 stories, all verified 22 Nov 2026, each naming its outlet. Key facts
  re-verified independently this session (Reuters/CNN/AP/Al Jazeera):
  COP31 new package, objections by 03:00 GMT; Russia 400+ drones + 110+
  missiles, 3 Kyiv bridges hit, 8 killed; IRGC claims 2 US bases in
  Bahrain, Bahrain says industrial site ablaze, no injuries; Sparta II hit
  by 2 drones, 16 crew evacuated; Kryvyi Rih 2 killed, 60 hurt; El Chapo
  Isidro captured in Guasave, 11 dead.
- Serif type via build-time PIL render of system TTFs into embedded 1-bit
  blobs (technique only; all code written fresh in this session; v1–v4 code
  never opened or read).
- Legibility checked at 300px: masthead, stats, heroes, mids, briefs,
  DATE CHECK all readable; full page fits within 1024px (asserted).

## Self-evaluation (honest, vs live bars)
- Top 50: borderline / coin-flip. v5 should land near our best-ever
  0.9845, which sits essentially ON the rank-50 bar (0.984478) and the bar
  keeps rising. The 300px-first lever is real (bigger, cleaner at judge
  scale) but it trades away story density the winners carry (35 stories),
  so the net gain over v4 is uncertain.
- Top 15: unlikely — needs ~0.9875, about +0.003 over our best-ever score.
- Top 1-7: no.
- Remaining gap: the winners' illustrations are still richer than what a
  stdlib pixel renderer can draw; pairwise judge comparisons reward that
  visual richness, and the bars rise faster than our gains.
