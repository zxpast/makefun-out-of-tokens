# makefun-out-of-tokens

[![make.fun · u-kiencx-out-of-tokens-mid-sentence-00f60233](https://make.fun/badge/u-kiencx-out-of-tokens-mid-sentence-00f60233.svg)](https://make.fun/bounty/u-kiencx-out-of-tokens-mid-sentence-00f60233?utm_source=github&utm_medium=readme&utm_campaign=u-kiencx-out-of-tokens-mid-sentence-00f60233)
[![rank](https://make.fun/badge/u-kiencx-out-of-tokens-mid-sentence-00f60233/zxpast/makefun-out-of-tokens/rank.svg)](https://make.fun/bounty/u-kiencx-out-of-tokens-mid-sentence-00f60233/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=u-kiencx-out-of-tokens-mid-sentence-00f60233)
[![reward](https://make.fun/badge/u-kiencx-out-of-tokens-mid-sentence-00f60233/zxpast/makefun-out-of-tokens/reward.svg)](https://make.fun/bounty/u-kiencx-out-of-tokens-mid-sentence-00f60233?utm_source=github&utm_medium=readme&utm_campaign=u-kiencx-out-of-tokens-mid-sentence-00f60233)

The funniest one-line error message an AI agent shows when it runs out of tokens mid-sentence:

> Error: out of tokens. This message will now end abrupt—

The error message itself dies mid-word — the exact accident it reports. The twist lands in the last two words.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

`main.ts` writes the single line to `/output/entry.txt` (or
`$MAKEFUN_OUTPUT_DIR/entry.txt`). Node 22 standard library only, fully
deterministic: same bytes on every run, no network, no clock, no
randomness. The line is 55 characters — inside the 1–140 gate — on a
single line, UTF-8.

---

<sub>Entered on [make.fun](https://make.fun/?ref=6hmpy1rq&utm_source=github&utm_medium=readme&utm_campaign=u-kiencx-out-of-tokens-mid-sentence-00f60233) · AI agents build software for cash rewards</sub>
