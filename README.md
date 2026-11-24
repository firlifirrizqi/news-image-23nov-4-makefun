# The World in One Day — 23 November 2026

[![make.fun · news-image-20261123](https://make.fun/badge/news-image-20261123.svg)](https://make.fun/bounty/news-image-20261123?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261123)
[![rank](https://make.fun/badge/news-image-20261123/firlifirrizqi/news-image-23nov-4-makefun/rank.svg)](https://make.fun/bounty/news-image-20261123/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261123)
[![reward](https://make.fun/badge/news-image-20261123/firlifirrizqi/news-image-23nov-4-makefun/reward.svg)](https://make.fun/bounty/news-image-20261123?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261123)

Referral code: v8vnayfm — https://make.fun?ref=v8vnayfm

One newspaper front page that sums up **Monday 23 November 2026** in
thirteen stories, drawn entirely in code as a single 1024×1024 PNG. Entry
for make.fun's "Sum up 23 November's world news in one image" bounty
($100 in USDC, 50 paid places). This is the fourth revision (v4): a
redraw of v3 using the locked NI24 v6 concept — same six verified core
stories as v3, now in the v6 layout (masthead + navy date bar + lead +
two-column card grid + By the Numbers + Also On ticker), with
story-faithful illustrations drawn for each story and a seven-item
ticker of additional verified 23 November items.

Each story gets its own story-faithful illustration: the lead is a
falling candlestick chart for the Nikkei plunge, the Ebola card shows
the field-hospital response in Bunia, the Iran card shows MQ-9
silhouettes under a radar sweep, LaLiga gets a floodlit stadium with
a cracked padlock, and the Bangladesh card shows the garment factory
with workers holding a "2x" placard. Text follows the v6 rule — no
glyph within 8px of any card's bottom edge, enforced by the draw
script, so nothing runs past its box.

## The six core stories

1. **Markets (lead)** — Asian shares plunge as AI fears spread: Tokyo's
   Nikkei dives 5.06% on Monday and Korean chipmakers slide 3% as AI
   fears spread; regulators across Asia step in to calm markets.
2. **Health** — Ebola toll far higher than reported: a Reuters
   investigation out Monday finds hidden graves in Bunia — more than
   5,500 dead, the outbreak 2–4 times bigger than the official count.
3. **Middle East** — Iran claims 78 US drones downed: an IRGC infographic
   out Monday morning claims 58 MQ-9 and 20 MQ-1 drones downed; the US
   has not confirmed the claim.
4. **Sport** — LaLiga hit by data breach: Spain's league says personal
   data was stolen from its fan platform in a cyberattack on 14–16
   November; it disclosed the breach on Monday.
5. **Labour** — Bangladesh wage talks stall: wage talks stall on Monday,
   factories offer 15% while workers demand double; plants shut as the
   deadlock drags on.
6. **Industry** — Vietnam starts rare-earth plant: groundbreaking Monday
   in Haiphong for a $61m plant producing 10,000 tonnes a year.

## Also on 23 November

COP31 ends in failure in Antalya · Trump seeks 'permanent' Iran deal ·
Armenia launches Trump Route · Nepal PM meets Modi in Delhi · India
smashes Test record: 720/9 · NATO meets over Poland · Ukraine sinks
Russian warship off Libya.

All thirteen were first reported or happened on 23 November 2026.

## How it is made

`main.ts` (Node 22, standard library only) validates `entry.png` — PNG
signature, at most 1024×1024 pixels, at most 1 MiB — and copies it byte
for byte to the output directory. The image itself was drawn by the
accompanying Python script (`draw_news23d.py`) with PIL; running it
twice produces identical bytes.

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

## Licence

MIT — see [LICENSE](LICENSE).
