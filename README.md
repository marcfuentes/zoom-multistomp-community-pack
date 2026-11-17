# Zoom MultiStomp — Community Effect Pack (8 Custom Effects)
### Official User Manual & Parameter Reference Guide
**Compatible Hardware:** Zoom MS-70CDR & MS-50G (Firmware v2.10)  
**Pedal Category:** All effects are located under the **DELAY** category  
**Community Release:** Dedicated to Reddit `r/zoommultistomp` & Facebook MultiStomp Groups  

---

## Table of Contents
1. [Installation & Quick Start Guide](#1-installation--quick-start-guide)
2. [Quick Reference Matrix / Knob Cheat Sheet](#2-quick-reference-matrix--knob-cheat-sheet)
3. [Deep Dive Effect Manuals](#3-deep-dive-effect-manuals)
   - [1. SilverSt — American Tube Clean Amplifier + 2×12 Open-Back Cab](#1-silverst--american-tube-clean-amplifier--212-open-back-cab)
   - [2. 424mkI — Vintage Multitrack Cassette Preamp & Fuzz](#2-424mki--vintage-multitrack-cassette-preamp--fuzz)
   - [3. Dustbox — Chainsaw Fuzz + Synthetic Sub-Octave Divider](#3-dustbox--chainsaw-fuzz--synthetic-sub-octave-divider)
   - [4. Nimbus — Ambient Granular Cloud Synthesis](#4-nimbus--ambient-granular-cloud-synthesis)
   - [5. Dustfall — Dirty Layered Reverb & Echo with Drive and Sag](#5-dustfall--dirty-layered-reverb--echo-with-drive-and-sag)
   - [6. Shields — Reverse Early Reflections Multitap (Glide Guitar)](#6-shields--reverse-early-reflections-multitap-glide-guitar)
   - [7. Ouroboros (mono) — 3-Head Tape Echo & Spring Reverb](#7-ouroboros-mono--3-head-tape-echo--spring-reverb)
   - [8. Gatsby — Tape Saturation & Through-Zero Doubletracker](#8-gatsby--tape-saturation--through-zero-doubletracker)
4. [Recommended Pedalboard Chain Recipes](#4-recommended-pedalboard-chain-recipes)

---

## 1. Installation & Quick Start Guide

### ⚠️ Golden Rule Before Flashing:
**Always perform a complete backup of your pedal's patches and effects** prior to installing any custom `.ZDL` files. You can use standard community utilities such as *Zoom Effect Manager (ZEM)* or *Zoom Firmware Editor*. Never disconnect the USB cable during transfer.

### Why do all effects appear under the DELAY category?
In the Zoom MultiStomp firmware architecture, the **Delay** category (Group ID 8) provides the largest dedicated memory arena and full support for synthesized parameter edit handlers (knobs 4 through 9). Regardless of whether an effect is a clean guitar amplifier (`SilverSt`), a high-gain fuzz (`424mkI`, `Dustbox`), or an ambient reverb (`Dustfall`), **they will always be found in the DELAY group on the pedal's display**.

### Included `.ZDL` binary files:
1. `SilverSt.ZDL` &mdash; Clean American amplifier & 2×12 open-back stereo cabinet.
2. `424mkI.ZDL` &mdash; Vintage multitrack cassette preamp and overdriven console fuzz.
3. `Dustbox.ZDL` &mdash; Chainsaw distortion with a -2 octave square-wave sub divider.
4. `Nimbus.ZDL` &mdash; 6-voice ambient granular cloud with scan-head navigation and Freeze.
5. `Dustfall.ZDL` &mdash; Dual-layer dirty reverb/echo featuring parallel Drive and voltage Sag.
6. `Shields.ZDL` &mdash; 19-tap reverse early reflections for the definitive MBV glide guitar tone.
7. `Uroboros.ZDL` &mdash; 3-head tape echo with real motor inertia and parallel spring reverb tank.
8. `Gatsby.ZDL` &mdash; Vintage tape saturation and through-zero flanging (−0.3 ms offset).

---

## 2. Quick Reference Matrix / Knob Cheat Sheet

| Effect | Sonic Inspiration | Chain Role | Display Knobs | Output / Notes |
|---|---|---|---|---|
| **SilverSt** | Fender Silverface + 2×12 | Clean Amp & Cab | `Gain`, `Width`, `Level`, `Bass`, `Middl`, `Trebl`, `Reson`, `Prese`, `Mic` | Stereo / Cab always active |
| **424mkI** | Tascam Portastudio 424 | Cassette Preamp / Fuzz | `Trim`, `Chan`, `Mstr`, `Bass`, `Trebl`, `Level` | 5-stage analog saturation |
| **Dustbox** | DOD FX33 Buzz Box | Sludge Fuzz + Sub-Octave | `Dust`, `Motor`, `Filter`, `Power` | Synthetic -2 oct sub |
| **Nimbus** | Granular Cloud Synthesis | Ambient Wash / Drones | `Size`, `Pitch`, `Dens`, `Mix`, `Freeze`, `Tone`, `Speed`, `Wah` | ~3s buffer / 6 grain voices |
| **Dustfall** | Dirty Ambient Reverb | Lo-Fi Verb / Broken Tails | `Mode`, `Decay`, `Level`, `Drive`, `Sag`, `Mix`, `Amp`, `Volume` | Base reverb + Drive/Sag |
| **Shields** | Yamaha SPX90 (Reverse Gate) | Shoegaze Glide Guitar | `Size`, `Live`, `PreDly`, `Tone`, `Mix` | **Must place BEFORE drive!** |
| **Ouroboros** | Roland RE-201 Space Echo | Multi-Head Tape + Spring | `Mode` (1-12), `Repeat`, `Intens`, `EchoVol`, `RevVol`, `Bass`, `Treble`, `Sat`, `Mix` | True mechanical motor inertia |
| **Gatsby** | Strymon Deco V2 | Tape Saturation & Flange | `Sat`, `Voice`, `Tone`, `Level`, `Lag`, `Blend`, `Wobble`, `Type`, `Mix` | True Through-Zero (−0.3ms) |

---

## 3. Deep Dive Effect Manuals

---

### 1. SilverSt — American Tube Clean Amplifier + 2×12 Open-Back Cab

#### Sound Concept & Profile
Inspired by classic American tube amplifiers (Fender Silverface Twin/Deluxe era) coupled with an open-back 2×12 speaker cabinet. Its voice features a firm low-end body, a natural mid scoop, and sparkling upper-mid chime. It provides two fully profiled virtual microphone perspectives: **Center** (bright, crisp, on-axis) and **Edge** (warm, rounded, off-axis).

> **Placement Tip:** Place SilverSt at the **end of your pedal chain** and connect the L/R outputs directly into your audio interface, front-of-house PA, or FRFR monitor. Its cabinet simulation is always active.

#### Controls
- **Gain (0–100):** Ranges from crystal-clear clean headroom to a smooth, compressed edge-of-breakup tone.
- **Bass, Middl, Trebl (0–100):** Active 3-band preamp equalization.
- **Reson (0–100):** Controls low-frequency power-stage damping and speaker resonance (thump and transient response).
- **Prese (0–100):** Upper-mid attack and bite before entering the cabinet stage.
- **Mic (0–100):** Virtual microphone placement (0 = Center cone, bright; 100 = Edge, warm and off-axis).
- **Width (0–100):** Stereo microphone offset across L/R channels. Maintains perfectly safe mono fold-down without phase cancellation.
- **Level (0–100):** Master output volume.

#### Suggested Presets
| Preset | Gain | Width | Level | Bass | Middl | Trebl | Reson | Prese | Mic |
|---|---|---|---|---|---|---|---|---|---|
| **Pedal Platform** | 25 | 30 | 60 | 50 | 50 | 50 | 45 | 50 | 35 |
| **Glass Clean** | 12 | 20 | 62 | 42 | 43 | 64 | 30 | 65 | 18 |
| **Warm Edge of Breakup**| 72 | 22 | 48 | 58 | 58 | 38 | 62 | 38 | 72 |
| **Big Studio Clean** | 35 | 40 | 56 | 62 | 38 | 54 | 68 | 55 | 32 |

---

### 2. 424mkI — Vintage Multitrack Cassette Preamp & Fuzz

#### Sound Concept & Profile
Inspired by the distinctive analog preamplifier and overdriven cassette sound of the iconic Tascam Portastudio 424 multitrack recorders. At moderate levels, it introduces warm harmonic tape coloration and musical dynamic compression. When driven aggressively, it cascades into a thick, gritty, lo-fi mixer fuzz with unmistakable 90s indie character.

#### Controls
- **Trim (0–100):** Analog input stage gain (from 1x up to ~98.9x).
- **Chan (0–100):** Channel fader level. Pushing this knob fattens the low-mid response and increases harmonic saturation.
- **Mstr (0–100):** Master bus level feeding the final output clipping stages.
- **Bass & Trebl (0–100):** Console 2-band shelving EQ (50 = flat response).
- **Level (0–100):** Output master volume post-clipping.

#### Suggested Presets
| Preset | Trim | Chan | Mstr | Bass | Trebl | Level | Sonic Character |
|---|---|---|---|---|---|---|---|
| **Tape Warmth (Default)** | 50 | 85 | 85 | 50 | 50 | 35 | Subtle analog compression and harmonic glue. |
| **Maxed Console Fuzz** | 100 | 100 | 100 | 50 | 50 | 25 | Brutal lo-fi mixer fuzz with extreme saturation. |
| **Warm Clean Preamp** | 20 | 85 | 85 | 50 | 50 | 35 | Transparent warming for cleans or acoustic instruments. |
| **Indie Rock Crunch** | 80 | 90 | 90 | 50 | 50 | 25 | Gritty cassette edge-of-distortion drive. |

---

### 3. Dustbox — Chainsaw Fuzz + Synthetic Sub-Octave Divider

#### Sound Concept & Profile
Inspired by the legendary and abrasive DOD FX33 Buzz Box. Combina an aggressive, buzzing chainsaw distortion with a synthetic sub-octave divider that tracks **two octaves down (-2 oct)**. The result is a delightfully chaotic, sludge-heavy wall of fuzz that turns single notes and palm mutes into devastating industrial textures.

> **Control Layout (Industrial Vacuum Cleaner Theme):** Dust (octave blend), Motor (distortion gain), Filter (tone), and Power (master volume).

#### Controls
- **Dust (0–100):** Balance between pure distortion (0) and the -2 octave square-wave sub (100). At 0, the octave is completely absent.
- **Motor (0–100):** Distortion gain. As Motor increases, the octave divider becomes more chaotic and unstable.
- **Filter (0–100):** High-shelf tone control (~3 kHz) affecting the distortion branch (0 = dark/muffled, 50 = flat, 100 = biting/sharp). Does not filter the sub-octave.
- **Power (0–100):** Master output volume (starts low by default for speaker safety).

#### Suggested Presets
| Preset | Dust | Motor | Filter | Power | Description |
|---|---|---|---|---|---|
| **Classic Buzz Box Sludge** | 50 | 60 | 50 | 25 | The signature Melvins sludge sound. |
| **Pure Chainsaw Fuzz** | 0 | 75 | 65 | 25 | Straight-ahead chainsaw distortion with zero sub. |
| **Sub-Bass Glitch Drone** | 90 | 40 | 30 | 30 | Dominant synthetic low-end for slow, heavy riffs. |

---

### 4. Nimbus — Ambient Granular Cloud Synthesis

#### Sound Concept & Profile
Inspired by modern ambient granular synthesis (Clouds / Mood archetype). Nimbus continuously captures your playing into a ~3-second circular audio buffer. Up to **6 independent grain voices** read staggered, randomized positions through smooth parabolic envelopes (free of clicks), feeding into resonant state-variable filters (SVF) and an all-pass stereo diffusion network.

#### Controls
- **Size (0–100):** Grain duration (~40 ms for glitchy/textural chops to ~400 ms for smooth, floating ambient washes).
- **Pitch (0–100):** Playback rate (0 = -1 octave, 50 = unison, 100 = +1 octave shimmer).
- **Dens (0–100):** Active voice density (1 to 6 voices) and temporal scatter.
- **Mix (0–100):** Dry/wet blend (audition new settings with Mix around 60–80).
- **Freeze (0–100):** Settings ≥50 freeze the current buffer (~2.97 s) indefinitely, allowing you to sustain an infinite pad while playing clean over top.
- **Tone (0–100):** SVF filter cutoff frequency per voice (~180 Hz to 5 kHz).
- **Speed (0–100):** Scan-head navigation speed (75 = 1.0x normal, 50 = stationary hold, <50 = reverse playback).
- **Wah (0–100):** Interactive character macro coupling filter resonance with a dynamic envelope follower (dynamic auto-wah reactive to pick attack).

#### Suggested Presets
| Preset | Size | Pitch | Dens | Mix | Freeze | Tone | Speed | Wah |
|---|---|---|---|---|---|---|---|---|
| **Ambient Dream Cloud** | 55 | 50 | 60 | 60 | 0 | 75 | 75 | 0 |
| **Shimmer Wash (+1 Oct)** | 70 | 100 | 75 | 50 | 0 | 65 | 75 | 15 |
| **Sub-Atmosphere Drone** | 85 | 0 | 80 | 70 | 55 | 45 | 50 | 0 |
| **Reverse Glitch Scatter** | 25 | 50 | 50 | 50 | 0 | 80 | 25 | 40 |

---

### 5. Dustfall — Dirty Layered Reverb & Echo with Drive and Sag

#### Sound Concept & Profile
Dustfall is a dual-layer ambient processor crafted specifically for shoegaze walls of sound, worn tape textures, and crumbling reverb decays. It splits incoming audio into a clean base ambient layer and a parallel secondary layer that can be pushed into heavy saturation (**Drive**) and voltage starvation (**Sag**), recombining prior to an output preamp stage (**Amp**).

> **The Dustfall Workflow:** `Level` shapes the base ambient wash; `Drive` and `Sag` distress the parallel copy; `Mix` controls how much destruction is blended in; `Amp` provides the final master tone color.

#### Controls
- **Mode:** Selects ambient topology: **Hall** (0–32, spacious & dark), **Spring** (33–66, metallic chime), or **BBD** (67–100, dark analog delay).
- **Decay (0–100):** Reverb tail length or delay feedback.
- **Level (0–100):** Base dry/reverb balance before saturation.
- **Drive (0–100):** Gain and clipping intensity of the secondary parallel layer.
- **Sag (0–100):** Dying-battery simulation (*voltage starvation*) that sputters and gates the decaying tails.
- **Mix (0–100):** Balance between clean base reverb and driven/sagged layer.
- **Amp:** Output preamp character: **Neutral** (balanced), **Murk** (dark, compressed, heavy low-mid punch), or **Open** (bright, biting edge).
- **Volume (0–100):** Output master level.

#### Suggested Presets
| Preset | Mode | Decay | Level | Drive | Sag | Mix | Amp | Volume |
|---|---|---|---|---|---|---|---|---|
| **Shoegaze Fog** | Hall | 65 | 50 | 40 | 35 | 60 | Murk | 35 |
| **Broken Spring** | Spring | 70 | 60 | 65 | 55 | 50 | Open | 30 |
| **Degraded BBD Tape** | BBD | 50 | 50 | 30 | 20 | 45 | Neutral | 50 |

---

### 6. Shields — Reverse Early Reflections Multitap (Glide Guitar)

#### Sound Concept & Profile
Inspired by the legendary Early Reflections ER2 "Reverse Gate" algorithm found in the classic Yamaha SPX90 rack unit. This is the definitive sonic foundation of vintage glide technique' iconic *glide guitar* technique on classic 90s shoegaze's masterpiece *classic glide albums*.

Shields is not a traditional diffuse reverb: it is a meticulously calibrated pattern of **19 reverse early reflections with ascending energy gains**, designed to simulate reverse tape swell.

> **⚠️ CRITICAL PEDALBOARD PLACEMENT:** Shields **MUST be placed BEFORE your fuzz, distortion, or overdriven amp**. When this rising envelope slams into an analog clipping stage, it creates the unmistakable elastic, blooming MBV wall-of-sound.

#### Controls
- **Size (0–100):** Expands or contracts the timing spacing of all 19 reflection taps (from 30 ms to 420 ms). A setting of 100 delivers the full MBV duration.
- **Live (0–10):** Controls absorption and tail weight (5 = factory rack preset; 7 = MBV sweet spot; 10 = maximum continuous density).
- **PreDly (0–100 ms):** Initial pre-delay prior to the reflection pattern (0 ms ensures instant pick attack coupling).
- **Tone (0–100):** Low-pass filter for the wet signal (100 = retains vintage 12 kHz rack converter bandwidth).
- **Mix (0–100):** Dry/wet crossfade (defaults to 100% wet for directly feeding dirt pedals).

#### Suggested Presets
| Preset | Size | Live | PreDly | Tone | Mix | Recommended Chain |
|---|---|---|---|---|---|---|
| **MBV classic glide albums (Default)** | 100 | 7 | 0 | 100 | 100 | `Shields` &rarr; Fuzz/Distortion &rarr; Amp |
| **SPX90 Factory Preset 17** | 16 | 5 | 25 | 100 | 100 | `Shields` &rarr; Mild Overdrive |
| **Subtle Glide Layer** | 70 | 6 | 10 | 60 | 50 | Ambient clean texture |

---

### 7. Ouroboros (mono) — 3-Head Tape Echo & Spring Reverb

#### Sound Concept & Profile
Inspired by the timeless Roland RE-201 Space Echo (1974). On your pedal's screen, it appears as **`Uroboros`**.

Ouroboros captures the living mechanics of an **endless analog tape loop** traveling across three fixed playback heads, driven by a variable-speed electric motor. Adjusting the `Repeat` knob changes motor speed with **authentic mechanical inertia**—resulting in genuine pitch-glide warping rather than instantaneous digital jumps. Includes analog-style recording saturation and a parallel spring reverb tank.

#### Controls
- **Mode (1–12):** Selects between the 12 historic RE-201 operating modes:
  - *Modes 1–4:* Tape echo only (Heads 1, 2, 3, and combinations).
  - *Modes 5–11:* Multi-head rhythmic echoes combined with the spring reverb tank.
  - *Mode 12:* Spring reverb only.
- **Repeat (0–100):** Tape motor speed (regulates echo time while introducing natural pitch-bending inertia).
- **Intens (0–100):** Echo feedback (crank to push into warm, self-oscillating musical pads).
- **EchoVol (0–100):** Tape echo volume.
- **RevVol (0–100):** Spring reverb volume.
- **Bass & Treble (0–100):** Passive repeat tone controls (50 = neutral).
- **Sat (0–100):** Magnetic tape preamp drive.
- **Mix (0–100):** Overall dry/wet master blend.

#### Suggested Presets
| Preset | Mode | Repeat | Intens | EchoVol | RevVol | Sat | Mix |
|---|---|---|---|---|---|---|---|
| **vintage dub Dub Chamber** | 7 (Heads 2+3 + Rev) | 45 | 70 | 65 | 40 | 40 | 50 |
| **Rockabilly Slapback** | 1 (Head 1) | 85 | 15 | 55 | 0 | 25 | 40 |
| **Infinite Space Oscillation** | 2 or 4 | 30 | 85 | 75 | 20 | 60 | 50 |

---

### 8. Gatsby — Tape Saturation & Through-Zero Doubletracker

#### Sound Concept & Profile
Inspired by boutique studio tape saturation and doubletracker processors (Strymon Deco style). Gatsby unites tape machine warmth with a dual-deck player (*Reference Deck* and *Lag Deck*). Its delay offset spans down to **−0.3 ms**, unlocking authentic **Through-Zero Flanging (TZF)**: the delayed deck sweeps directly through the zero-time boundary, producing total phase cancellation and the iconic jet-sweep flange that standard flangers cannot achieve.

#### Controls
- **Sat (0–100):** Tape saturation drive (from transparent mastering glue to rich tape overdrive).
- **Voice:** Tape formulation: **Classic** (0–49, open-reel studio deck) or **Cassette** (50–100, punchy cassette compression with extended low end).
- **Tone (0–100):** Saturation tone control (50 = flat).
- **Level (0–100):** Saturation output level compensation (50 = unity gain).
- **Lag (0–100):** Time delay between decks (−0.3 ms to 500 ms).
- **Blend (0–100):** Mix between Reference Deck and Lag Deck (50 = 50/50 balance, essential for deep TZF nulls).
- **Wobble (0–100):** Random tape speed modulation (authentic wow & flutter).
- **Type:** Deck phase routing: **Sum** (0–25), **Invert** (26–50), **Bounce** (51–75, stereo ping-pong), and **Auto-Sweep** (76–100).
- **Mix (0–100):** Overall dry/wet master balance.

#### Suggested Presets
| Preset | Sat | Voice | Tone | Lag | Blend | Wobble | Type | Mix |
|---|---|---|---|---|---|---|---|---|
| **Through-Zero Jet Flange** | 35 | Classic | 50 | 15 | 50 | 20 | Sum | 100 |
| **Stereo Doubler (Dimension)** | 25 | Classic | 50 | 45 | 50 | 35 | Bounce | 100 |
| **Cassette Preamp Warmth** | 65 | Cassette | 45 | 0 | 0 | 0 | Sum | 100 |
| **Vintage Tape Slapback** | 40 | Classic | 50 | 75 | 50 | 15 | Sum | 100 |

---

## 4. Recommended Pedalboard Chain Recipes

Take advantage of the Zoom MultiStomp's 6 simultaneous effect slots with these proven signal chains:

### Recipe 1: The Definitive Shoegaze / Dream Pop Wall
```
[Guitar] ──► Shields (100% Wet) ──► 424mkI (Fuzz/Preamp) ──► Nimbus (Granular Cloud) ──► SilverSt (Amp + Cab) ──► [Stereo Out]
```
*The rising reverse reflections from Shields smash into the 424mkI cassette preamp, Nimbus provides an ambient pad underneath, and SilverSt delivers the final studio amp and speaker response.*

### Recipe 2: Vintage Dub & Lo-Fi Tape Ambience
```
[Guitar / Synth] ──► Gatsby (Tape Saturation) ──► Uroboros (RE-201) ──► Dustfall (Dirty Verb) ──► [Stereo Out]
```
*Gatsby adds tape warmth and stereo width, Ouroboros provides multi-head rhythmic echoes with physical pitch inertia, and Dustfall wraps the repeats in a crumbling ambient tail.*

### Recipe 3: Sludge / Glitch Chaos
```
[Bass or Guitar] ──► Dustbox (Buzz Box Fuzz) ──► Nimbus (Freeze enabled ≥ 60) ──► SilverSt (Clean Amp) ──► [Output]
```
*Brutal chainsaw riffs with a synthetic -2 octave sub frozen into shifting granular drones.*

---
*Created with love for the Zoom MultiStomp community.*
