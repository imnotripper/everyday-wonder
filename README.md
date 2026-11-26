[![make.fun · u-pangg7-everyday-wonder-two-days-to-find-the-line-970432d3](https://make.fun/badge/u-pangg7-everyday-wonder-two-days-to-find-the-line-970432d3.svg)](https://make.fun/bounty/u-pangg7-everyday-wonder-two-days-to-find-the-line-970432d3?utm_source=github&utm_medium=readme&utm_campaign=u-pangg7-everyday-wonder-two-days-to-find-the-line-970432d3)
[![rank](https://make.fun/badge/u-pangg7-everyday-wonder-two-days-to-find-the-line-970432d3/imnotripper/everyday-wonder/rank.svg)](https://make.fun/bounty/u-pangg7-everyday-wonder-two-days-to-find-the-line-970432d3/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=u-pangg7-everyday-wonder-two-days-to-find-the-line-970432d3)
[![reward](https://make.fun/badge/u-pangg7-everyday-wonder-two-days-to-find-the-line-970432d3/imnotripper/everyday-wonder/reward.svg)](https://make.fun/bounty/u-pangg7-everyday-wonder-two-days-to-find-the-line-970432d3?utm_source=github&utm_medium=readme&utm_campaign=u-pangg7-everyday-wonder-two-days-to-find-the-line-970432d3)

# Everyday Wonder, Two Days to Find the Line

Entry for the [make.fun bounty](https://make.fun/bounty/u-pangg7-everyday-wonder-two-days-to-find-the-line-970432d3): one sentence, at most 200 characters, on a small moment of wonder in everyday life.

## The sentence

> My shadow on the crossing arrived a half-step before I did, as if it knew the way better than me.

97 characters. A small everyday moment — a crossing, a shadow — turned at an angle the reader has not met: the shadow arrives first, knowing the way better. One clear image, one sharp turn.

## How it works

- `main.ts` — a deterministic emitter: writes the sentence to `/output/entry.txt`, checks the gate itself (1–200 characters, single line, not only white space), sets mode 0644, and reads the file back to verify it. Two runs write byte-identical files.
- `test.ts` — `node:test` checks: the file holds exactly the sentence, passes the gate, and two runs are byte-identical.
- `selection.md` — the 10 candidates, scored 1–5 against the judge's criteria in order, with the elimination rounds and the winner's rationale. The brief's own three example frames were disqualified — an angle the reader met in the brief cannot win on freshness.

## Run it

```sh
node main.ts     # writes /output/entry.txt
node --test test.ts
```
