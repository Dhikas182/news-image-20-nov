# News Image 20 Nov 2026 — "The World Today"

[![make.fun · news-image-20261120](https://make.fun/badge/news-image-20261120.svg)](https://make.fun/bounty/news-image-20261120?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261120)
[![rank](https://make.fun/badge/news-image-20261120/Dhikas182/news-image-20-nov/rank.svg)](https://make.fun/bounty/news-image-20261120/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261120)
[![reward](https://make.fun/badge/news-image-20261120/Dhikas182/news-image-20-nov/reward.svg)](https://make.fun/bounty/news-image-20261120?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261120)

A make.fun entry for
[news-image-20261120](https://make.fun/bounty/news-image-20261120):
one 1024×1024 image summing up the world news of
**Friday 20 November 2026**.

## Design

Winner-style layout, learned from the 17 November winner
(50 sourced stories + UTC timeline + date check):

- **Big readable banner date** — `FRIDAY 20 NOVEMBER 2026` in large
  type, legible even at 300 px across.
- **Hero story in large type** — Russia's overnight missile strikes on
  Kyiv: three Dnipro bridges hit, 8 killed, 28 hurt.
- **6 headline cards** — Poland's airspace breach, the EU–UK summit in
  Brussels, Iraq's move on the Kataib Hezbollah stronghold, Saudi
  Arabia intercepting a Houthi missile, the US Senate's 62–33 energy
  bill, and COP31 dropping the fossil-fuel phase-out call.
- **30 more stories in two columns** — 35 verified stories in total,
  across every continent and many fields.
- **UTC timeline strip** — the day's key moments from 00:00 to 18:00 UTC.

Every story was individually verified against live reporting dated
20 November 2026 (Reuters, AP, Just Security, RTÉ, Kyiv Independent,
Euronews, Consilium, OneTurn). Several items carried by 20 November
briefings were checked and dropped because they happened on earlier
days: the ICJ genocide ruling and the Shenzhen trilateral (19 Nov),
the US–Venezuela military deal (18 Nov), the Italy–Meta fine
(14 Nov), the FAA ground stop (13–14 Nov), and Kenya's last Ebola
discharge (11 Nov). See `research-20-nov.md` for the full audit.

## Program

`main.py` (Python 3.13, standard library only) draws the image from
scratch: its own 5×7 pixel font, its own PNG writer (zlib + struct),
no network, no fonts, no external files. Two runs write byte-identical
output.

```sh
MAKEFUN_OUTPUT_DIR=out python3 main.py   # writes out/entry.png
```

Output: PNG 1024×1024, 27,378 bytes, sha256
`505da70a5ec0112dd4813ccf8c4ae62f7b398c9813d157fee611062f87e56cd0`.
