# _superDestroy

A Max for Live audio effect — a faithful port and creative expansion of
Destroy FX's **Polarizer**.

## What it does

The original Polarizer periodically inverts the polarity of one audio
sample, with an optional wavefold ("implode") on top — a simple idea that
produces a surprisingly wide range of digital grit, from subtle buzz to
outright destruction. `_superDestroy` ports that core algorithm
sample-accurately, then builds on it:

- **Width** — extends a single polarized sample into a sustained run of
  polarized samples, opening up rhythmic/glitch-gate territory that
  doesn't exist in the original.
- **Continuous Implosion** — the original's fold was strictly on/off;
  here it's a continuous blend, including negative territory (amplify
  rather than fold) that doesn't exist in the original at all.
- **Asymmetry** — the original produced a small DC offset instead of
  true silence under one specific condition; this device fixes that by
  default, but lets you dial the original's own quirk back in
  deliberately if you want it.
- **Skew** — an independent, new control for asymmetric gain shaping
  between the positive and negative halves of the waveform, with no
  counterpart in the original.
- **Extended ranges** on every parameter, well past what the original
  plugin could reach, while still being able to dial in the original's
  exact sound.
- **Fractional precision** — every control accepts exact decimal values,
  not just whole numbers.
- **A built-in safety limiter** — new, not present in the original.
- **A live oscilloscope** — new, not present in the original.
- **Live readouts** for every control, showing its real, in-use effect
  on the signal, not just its own setting.

If you set every parameter to its original-equivalent value, this device
should sound essentially identical to the original. Turned up, it goes
considerably further.

## Installing

Download `_superDestroy_1.0.amxd` from this repo and drag it onto an
audio track in Ableton Live.

## Documentation

See [`_superDestroy_manual.txt`](./_superDestroy_manual.txt) in this repo
for the full parameter reference, how to exactly match the original
plugin's sound, and a guide to the live readouts.

## Source

In compliance with the GPL-2.0 license this project inherits from the
original Polarizer, the modified source is included in this repo:
[`_superDestroy_1.0_source.json`](./_superDestroy_1.0_source.json) is
the complete Max patcher (rename to `.maxpat` to open directly in Max).

## Credits & license

`_superDestroy` is a derivative of Destroy FX's **Polarizer**, originally
written by Sophia Poirier and Tom Murphy 7. The original source is
available at [destroyfx/destroyfx](https://github.com/sophiapoirier/destroyfx/tree/main/polarizer).

This project is released under the **GNU General Public License v2.0**,
the same license as the original — see [`LICENSE`](./LICENSE) for the
full text.
