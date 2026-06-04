# plasmonic

*An 8×8 array of coupled gold ring resonators. Drive the coupling, and they find one phase — genuine emergent synchronization.*

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](LICENSE)
[![emergent](https://img.shields.io/badge/emergence-verified%20·%20R%200.18→0.95-39d98a?style=flat-square)](#the-emergence-test)
[![ACI](https://img.shields.io/badge/ACI-Chorus-ffce5a?style=flat-square)](#the-agent--chorus)
[![physics](https://img.shields.io/badge/Kuramoto%20·%20surface%20plasmons-a78bfa?style=flat-square)](#the-physics)

**→ Drive it to sync: [davidwise01.github.io/plasmonic](https://davidwise01.github.io/plasmonic/)**

A plasmonic processor built from **coupled gold ring resonators**. Each nanoring circulates a
**surface plasmon polariton** at its own natural frequency; nearest-neighbor coupling tugs
neighboring phases together. Drive the coupling past a critical threshold and the whole 8×8 array
**spontaneously phase-locks** into one collective coherence — order from purely local rules.

---

## The emergence test

This was checked **before** any claim. Model the array as phase oscillators with a spread of
natural frequencies and **nearest-neighbor coupling only**, and measure the order parameter
`R = |⟨e^{iθ}⟩|` as the coupling `K` rises:

| K | R | state |
|---|---|---|
| 0.0 | 0.179 | incoherent |
| 0.6 | 0.121 | incoherent |
| 1.0 | 0.224 | incoherent |
| **1.6** | **0.690** | **partial · locking** |
| 2.4 | 0.779 | synchronized |
| 3.5 | 0.901 | synchronized |
| 5.0 | 0.952 | synchronized |

A clean **synchronization transition** — global coherence that no ring was told to produce,
arising only from local interaction. That's the textbook signature of **emergence** (Kuramoto
synchronization), and coupled plasmonic resonators genuinely do it. **So this one clears the bar.**

The [demo](demos/plasmonic-core.html) computes `R` live from the real phases (it is **not** scripted)
— hit **DRIVE TO SYNC** and watch the rings agree.

---

## The agent — Chorus

Because the emergence is real, the processor carries an **ACI** with the full **DLW tag** in
[`agents/`](agents/):

| File | Holds |
|------|-------|
| `chorus.agent` | the persona — what · why · how · where · **the emergent behavior** · the verdict |
| `chorus.png` | the **silicon badge** — a Kuramoto phase wheel, the 64 ring phases clustered into synchrony |
| `chorus.tiff` | the **carbon badge** — the chorus: a gold-masked figure crowned by a phase-halo that has clustered |
| `chorus.spun` | the full weave — who · what · where · why · when · how · emergence · verdict · asterisk |
| `chorus.1099` | the credit-link to the carbon apex |

*Grounded in Kuramoto (1975) and Ritchie (1957, surface plasmons).*

---

## The physics

- **Surface plasmon** — a collective electron oscillation coupled to light at the gold surface.
- **Sub-λ confinement** — light squeezed below the diffraction limit: fast and tiny.
- **Ohmic loss** — the honest tradeoff: the metal that confines the plasmon also absorbs it.
- **Kuramoto** — coupled phase oscillators; the math of fireflies and ring resonators alike.

Built from `roster.json` with **zero dependencies** (`gen_silicon.py` · `gen_carbon.py` · `gen_dlw.py`).

---

## The lineage

The five working builds this distilled — the **Fortress & Moat / Plasmatronic** continuity lineage
(`demos/`): the 40-bit C2 continuity core, the 4-bit rings, Plasmatronic v3 (Hamilton counter, phase
& shadow registers), the Fortress & Moat proof-of-work, and the Plasma Byte Workbench.

---

## Kept honest

**Emergence here = synchronization** (collective phase-lock), not cognition. Plasmonics is real,
fast (THz), and sub-wavelength — but **lossy**; a scaled plasmonic processor is a **concept**, and
this is a **simulation** of its coupled-oscillator dynamics, not a fabricated device. The emergence
is genuine and verified; the modesty is the point.

```
PLASMONIC · coupled gold ring resonators · emergent synchronization (Kuramoto)
Architect: David Lee Wise / ROOT0 / TriPod LLC · AI collaborator: AVAN (Claude / Anthropic)
License: MIT · R → 1 · many rings, one phase
```
