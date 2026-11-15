# Aetherloom

> The loom does not speak. It keeps the threads.

[中文](README.md) | English

What lives here are its weaves: files that say, stitch by stitch, *when*, *which
motif*, and *how deep the water*.

## A weave

The `.txt` files under `weaves/patterns/` hold one stitch per line, three things,
divided by a bar:

```
tick|motif|amplitude
```

```text
00:00|1|0
00:04|1|20
00:09|1|40
00:14|1|60
00:19|1|40
00:24|1|20
00:30|1|0
```

| A stitch | Holds | May be |
|---|---|---|
| tick | the moment, counted from zero | `12`, `12.5`, `01:12`, `00:01:12`, up to three hours |
| motif | which waveform walks | an integer, `1`–`10` |
| amplitude | how deep the water runs | an integer, `0`–`100`; `0` is dry |

Five laws of the stitch:

- All three must be present. Miss one and the stitch is void.
- No two stitches closer than 0.5 s. Denser ones are swallowed by the throttle.
- Ticks should climb. Two stitches at the same moment: only the later one counts.
- A whole line beginning with `#` is a margin note. It may not trail a stitch.
- The last stitch returns amplitude to zero, or the loom holds its final state.

## The ten motifs

| No. | Motif | Shape | Suited to |
|---|---|---|---|
| 1 | Still stream | flat and continuous, lightest of three | groundwork, closing, long low passages |
| 2 | Steady stream | same waveform as Still, middle gain | the middle stretch of a weave |
| 3 | Rushing stream | same waveform as Still, full gain | the crest, full water |
| 4 | Sparse rain | short pulses, wide gaps | beats, crisp rhythm |
| 5 | Ebb | a run of pulses, each weaker than the last | from fast to slow, drawing in |
| 6 | Reflux | speeds and slows on its own, longest cycle | turns, shifting tempo |
| 7 | Downpour | dense short pulses, merged into one sheet | the chorus of a hard rhythm |
| 8 | Climbing vine | amplitude steps upward, level by level | swells, ascents |
| 9 | Breath | one long, one short, alternating | contrast, held silence |
| 10 | Beads | short pulses chained into a single run | dense runs, just before the crest |

Still, Steady and Rushing are one waveform at three built-in depths. To keep the
texture and change only the level, hold the motif and move the amplitude; walking
1 → 2 → 3 stacks depth on depth. Motifs 4 to 10 are where the shapes truly differ.

## Five waters

| Amplitude | Water | Suited to |
|---|---|---|
| `0` | dry | opening, closing a passage, the end |
| `1`–`20` | trickle | groundwork, pauses |
| `21`–`50` | ripple | the middle stretch of a weave |
| `51`–`80` | surge | chorus, approach to the peak |
| `81`–`100` | boil | the peak, the crest |

Adjacent steps under five are hard to tell apart. Multiples of five are enough.

## The weaves

| Folder | Holds | Files |
|---|---|---|
| `weaves/patterns/` | text weaves, three columns to a stitch | `.txt` |
| `weaves/pulse-patterns/` | pulse weaves, single files or whole packs | `.pulse`, `.zip` |

The two kinds are written separately and do not share a format. A pack comes in as
`.zip`, named after the single file it holds.

### Text weaves

| Weave | Length | What it records |
|---|---|---|
| [三度潮汐.txt](weaves/patterns/三度潮汐.txt) | 53 min | three rises, peaks at 44 / 58 / 70; the closing stretch ebbs back to dry |
| [夜雨独阵.txt](weaves/patterns/夜雨独阵.txt) | 45 min | a plateau of 6–31 with one shower to 62; the closing stretch eases back to dry |

### Pulse weaves

| Weave | Form | What it records |
|---|---|---|
| [三度潮汐-波形.zip](weaves/pulse-patterns/三度潮汐-波形.zip) | pack | waveforms for the weave above, six parts |
| [夜雨独阵-波形.zip](weaves/pulse-patterns/夜雨独阵-波形.zip) | pack | waveforms for the weave above, six parts |

The weaves are given to the commons; no permission asked, none needed.
