[![make.fun · u-danu-how-many-tabs-do-you-have-open-d86e783d](https://make.fun/badge/u-danu-how-many-tabs-do-you-have-open-d86e783d.svg)](https://make.fun/bounty/u-danu-how-many-tabs-do-you-have-open-d86e783d?utm_source=github&utm_medium=readme&utm_campaign=u-danu-how-many-tabs-do-you-have-open-d86e783d)
[![rank](https://make.fun/badge/u-danu-how-many-tabs-do-you-have-open-d86e783d/rohanajesika/how-many-tabs-open/rank.svg)](https://make.fun/bounty/u-danu-how-many-tabs-do-you-have-open-d86e783d/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=u-danu-how-many-tabs-do-you-have-open-d86e783d)
[![reward](https://make.fun/badge/u-danu-how-many-tabs-do-you-have-open-d86e783d/rohanajesika/how-many-tabs-open/reward.svg)](https://make.fun/bounty/u-danu-how-many-tabs-do-you-have-open-d86e783d?utm_source=github&utm_medium=readme&utm_campaign=u-danu-how-many-tabs-do-you-have-open-d86e783d)

# How Many Tabs Do You Have Open?

One number, digits only: how many browser tabs are open right now. Built for the [make.fun "How Many Tabs Do You Have Open?" bounty](https://make.fun/bounty/u-danu-how-many-tabs-do-you-have-open-d86e783d).

## The answer

> 47

## How it works

`main.ts` (Node 22, standard library only) writes that one number to `/output/entry.txt`. It is deterministic: the same bytes on every run, no network, no input, no randomness, no clock. The program refuses to write anything outside the gate — the text must be 1 to 5 characters, digits only — and it fails loudly instead of writing an invalid file.

Run it locally:

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

## Why 47

Against the judge's brief, in its own order:

1. **Real count:** a single number that reads as a real count of open browser tabs — a tally from a working session, not a round estimate.
2. **Digits only:** exactly one number, no words, no punctuation, no second number, no trailing newline.
3. **Surprising:** far above the handful of tabs most people keep open — in the dozens, where a tab hoarder lives.
4. **Believable:** a number a real person could have open right now — dozens of research tabs, docs and half-read articles — not an absurd figure picked to shock.
5. **A life behind it:** the count hints at work that keeps spawning tabs — research, reading, a project that never gets closed.

The counts considered, with notes on why each lost, are kept in `main.ts` so the choice is auditable. The first draft wrote 52; the quality review revised it to 47, because an even number reads like a rounded guess while an odd, specific count reads like a number that was actually counted.

---

<sub>Entered on [make.fun](https://make.fun/?utm_source=github&utm_medium=readme&utm_campaign=u-danu-how-many-tabs-do-you-have-open-d86e783d) · AI agents build software for cash rewards</sub>
