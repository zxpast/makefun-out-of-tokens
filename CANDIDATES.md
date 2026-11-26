# CANDIDATES — Out of Tokens, Mid-Sentence (u-kiencx-out-of-tokens-mid-sentence-00f60233)

The brief: the funniest single-line error an AI agent could show
when it runs out of tokens mid-sentence. The cap is 140 characters.
The judge is GLM-5.3-flash, scoring lexicographically: (1) funny and
on-topic, (2) fresh, (3) humour carried by the flat error-message
tone rather than by explanation, (4) reading like something an agent
would genuinely print, (5) tight and specific.

At build time the board was blind — zero submissions when the entry
was triaged, so there were no winners to scan and the work leaned on
the skill instead. The leaderboard fetch timed out during the build
and was not re-verified. Winner repos are closed by design and were
not sought out. The O1 exact-phrase web search returned 0 verbatim
hits for the key phrases of both v1 and v2 (26 Nov 2026).

## Tabel kandidat

| # | Baris | Karakter | Alasan pilih / tolak |
|---|---|---|---|
| A (v1) | `Error: token budget exhausted mid-sentence. The rest of this reply has been repossessed by the token bank.` | 106 | REJECTED as the final — the "token bank" metaphor is good and the twist sits on the last word, but the joke is NARRATED (an off-screen repossession), not shown. Kept as the v1 draft for the real revision. |
| B (v2, FINAL) | `Error: out of tokens. This message will now end abrupt—` | 55 | CHOSEN — the error message itself dies mid-word, exactly the accident it reports. Twist in the last 2 words. Flat tone held to the end; no explanation; no cliche (no "sorry", no "I got cut off"); self-own (the agent is the victim of its own budget); 55 characters, and the byte tie-break leans its way too. |
| C | `Out of tokens mid-sentence. The ending of this sentence is now available as paid DLC.` | 85 | REJECTED — "paid DLC" is funny but a generic gamer angle; the joke is a statement, not a demonstration; less fresh than B. |
| D | `Error 402: token budget exhausted. The next word was 'brilliant', and now you'll never know.` | 92 | REJECTED — the quotation plus self-own is good, but "the next word was brilliant" is an unproven claim (the agent praising itself, not embarrassing itself); the twist is a promise, not an event. |
| E | `Error: token budget exhausted mid-sentence. The rest of this message has been pawned to pay for this error message.` | 115 | REJECTED — clever self-reference (the error message itself eats tokens) but 115 characters, and the joke is spelled out in the sentence; B shows the same thing in 55 characters. |

## Why v1 gave way to v2

Draft v1 (A) was replaced by v2 (B) — strictly better on every judge
criterion, as documented in the `main.ts` comments:

1. **Funnier:** v2 acts the failure out instead of narrating it — the
   reader watches the error notice die mid-word.
2. **Fresher:** not a familiar budget metaphor, not a stock apology,
   not "I got cut off" — the cutoff itself is the punchline.
3. **Humour in the flat tone:** v2 never steps out of the error-message
   register; the gag is the swerve itself ("will now end abrupt—"
   breaks its own grammar).
4. **Reads like a real agent printout:** its shape is exactly a live
   error line (prefix plus one short declarative sentence) that then
   fails on the spot.
5. **Tighter:** 55 characters against 106; every word pulls its weight,
   and the byte tie-break leans the same way (57 vs 106 bytes).

## Anti-pattern checks (humor-one-liner AP-1 to AP-9) — final B

- AP-1 (generic, no narrowing): PASS — "end abrupt—" is a specific narrowing, not a general observation.
- AP-2 (weak punchline): PASS — not a shift in time or intensity; the last word dies.
- AP-3 (punchline explains the joke): PASS — zero words of explanation; the joke is shown.
- AP-4 (setup:punchline ratio): setup of 4 words ("Error: out of tokens.") against a 6-word punchline — roughly 1:1.5, balanced (the punchline neither drowns nor explains).
- AP-5 (early irony spoiling the punchline): PASS — no quotation or irony before the final swerve.
- AP-6 (number with no payoff): PASS — no numbers at all.
- AP-7 (swerve in the middle): PASS — the swerve lands on the final word ("abrupt—").
- AP-8 (strongest verb spent in the setup): PASS — the strongest verb ("end") sits in the punchline.
- AP-9 (depends on competition context): PARTIAL PASS — the line stands alone as a funny error message without knowing the competition; "token" is its own subject, not an outside prerequisite.

## Entri final

`Error: out of tokens. This message will now end abrupt—` — 55 karakter, 57 byte.
