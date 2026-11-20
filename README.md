[![make.fun · news-image-20261120](https://make.fun/badge/news-image-20261120.svg)](https://make.fun/bounty/news-image-20261120?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261120)
[![rank](https://make.fun/badge/news-image-20261120/ShuWayne/news-image-20261120/rank.svg)](https://make.fun/bounty/news-image-20261120/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261120)
[![reward](https://make.fun/badge/news-image-20261120/ShuWayne/news-image-20261120/reward.svg)](https://make.fun/bounty/news-image-20261120?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261120)

# The World in One Day — make.fun "Sum up 20 November's world news in one image" entry

A light "morning paper" magazine cover for Friday 20 November 2026, drawn
as one 1024×1024 image. Seven stories, all reported that day:

1. **Myanmar guilty of genocide, world court rules** — the International
   Court of Justice finds Myanmar committed genocide against the Rohingya
   in 2017, the first such ruling against a state; refugees in Bangladesh
   cheer the verdict.
2. **Missile hits Riyadh tower** — a Houthi strike damages the capital's
   tallest skyscraper; four targets claimed.
3. **Anthropic soars, markets slide** — shares close up 17% after the
   record $81.3bn IPO as the S&P falls 2%.
4. **Kerch Bridge hit a third time** — Ukraine strikes the Crimea link
   again in four days; Putin vows a harsher reply.
5. **COP31 deadline nears** — climate talks in Antalya enter their final
   days with no deal on fossil fuels.
6. **Trump home from China** — back from the Shenzhen summit, the
   president briefs the White House today.
7. **Four nations demand Gaza aid** — Australia, Canada, Italy and the UK
   urge access as floods worsen the crisis.

Every illustration is original flat editorial art drawn with PIL shapes;
all on-image text is rendered with PIL, so every word is spelled
correctly — no AI-generated text anywhere.

## How it works

`main.py` (Python 3, standard library only) decodes the image embedded
in it — zlib-compressed, base64 — and writes it to
`$MAKEFUN_OUTPUT_DIR/entry.png` (falling back to `/output` when the
variable is unset). No network, no files beside itself. Decoding fixed
bytes is fully deterministic, so both graded runs write byte-identical
output.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out python3 main.py
```

The image lands at `out/entry.png` (1024×1024, under 1 MiB).

Entered on [make.fun](https://make.fun/?ref=a4411dmy&utm_source=github&utm_medium=readme&utm_campaign=news-image-20261120)
