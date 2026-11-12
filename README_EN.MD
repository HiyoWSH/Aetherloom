# Aetherloom

> The loom does not speak. It keeps the threads.

[中文](README.md) | English

What lives here are its weaves: plain-text files that say, stitch by stitch,
*when*, *which motif*, and *how deep the water*.

## A weave

One stitch per line, three things, divided by a bar:

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
- Ticks should climb. Two stitches at the same moment: only the later is heard.
- A whole line beginning with `#` is a margin note. It may not trail a stitch.
- The last stitch returns amplitude to zero, or the loom holds its final state.

## The ten motifs

| No. | Motif | Shape | Suited to |
|---|---|---|---|
| 1 | Still stream | flat and continuous, lightest of three | groundwork, closing, long low passages |
| 2 | Steady stream | same waveform as Still, middle gain | the working body of a weave |
| 3 | Rushing stream | same waveform as Still, full gain | surges, bursts |
| 4 | Sparse rain | short touches, clear gaps | beats, crisp rhythm |
| 5 | Ebb | a run of pulses, each weaker than the last | from fast to slow, gathering up |
| 6 | Reflux | speeds and slows on its own, longest cycle | turns, shifting tempo |
| 7 | Downpour | dense short pulses, merged into one sheet | the chorus of a hard rhythm |
| 8 | Climbing vine | amplitude steps upward, level by level | swells, ascents |
| 9 | Breath | one long, one short, alternating | contrast, held silence |
| 10 | Beads | short hits chained into a single run | dense runs, just before the strike |

Still, Steady and Rushing are one waveform at three built-in depths. To keep the
texture and change only the level, hold the motif and move the amplitude; walking
1 → 2 → 3 stacks depth on depth. Motifs 4 to 10 are where the shapes truly differ.

## Five waters

| Amplitude | Water | Suited to |
|---|---|---|
| `0` | dry | opening, closing a passage, the end |
| `1`–`20` | trickle | groundwork, pauses |
| `21`–`50` | ripple | the working body of a weave |
| `51`–`80` | surge | chorus, approach to the peak |
| `81`–`100` | boil | the peak, the strike |

## The weaves

The weaves are given to the commons. Take them without asking.
