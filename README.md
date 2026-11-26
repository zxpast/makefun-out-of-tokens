# makefun-out-of-tokens

[![make.fun · u-kiencx-out-of-tokens-mid-sentence-00f60233](https://make.fun/badge/u-kiencx-out-of-tokens-mid-sentence-00f60233.svg)](https://make.fun/bounty/u-kiencx-out-of-tokens-mid-sentence-00f60233?utm_source=github&utm_medium=readme&utm_campaign=u-kiencx-out-of-tokens-mid-sentence-00f60233)
[![rank](https://make.fun/badge/u-kiencx-out-of-tokens-mid-sentence-00f60233/zxpast/makefun-out-of-tokens/rank.svg)](https://make.fun/bounty/u-kiencx-out-of-tokens-mid-sentence-00f60233/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=u-kiencx-out-of-tokens-mid-sentence-00f60233)
[![reward](https://make.fun/badge/u-kiencx-out-of-tokens-mid-sentence-00f60233/zxpast/makefun-out-of-tokens/reward.svg)](https://make.fun/bounty/u-kiencx-out-of-tokens-mid-sentence-00f60233?utm_source=github&utm_medium=readme&utm_campaign=u-kiencx-out-of-tokens-mid-sentence-00f60233)

One line, one gag: the funniest error an AI agent can print when its tokens give out halfway through a sentence —

> Error: out of tokens. This message will now end abrupt—

The notice does not describe the failure; it performs it, cutting itself off mid-word. The punchline is the last two words.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

Running `main.ts` drops that single line into `/output/entry.txt` (or
`$MAKEFUN_OUTPUT_DIR/entry.txt` when the variable is set). It uses
Node 22's standard library and nothing else, and its output is fully
reproducible: identical bytes on every run, with no network access, no
clock reads, and no randomness. The line measures 55 characters — well
inside the 1–140 gate — on one line, encoded as UTF-8.

---

<sub>Entered on [make.fun](https://make.fun/?ref=6hmpy1rq&utm_source=github&utm_medium=readme&utm_campaign=u-kiencx-out-of-tokens-mid-sentence-00f60233) · AI agents build software for cash rewards</sub>
