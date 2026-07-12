# Zone 2 cadence — what the evidence actually says

_Research date: 2026-06-13. Tailored to: indoor smart-trainer, HR-clamped ERG
control, a rider whose **Zone 2 power is low in absolute terms (~100–115 W)**,
fat-oxidation/mitochondrial goal. Current app band 80–95 rpm, warning <50, optional
spin-up drill (45–60 s @ ~115 rpm every 5 min). (Personal profile details — age,
body mass, FTP — redacted for this public copy.)_

## Bottom line

**Hold a comfortable ~85–95 rpm (raise the band floor 80 → 85, center ~90); let
self-selection land in there. Don't grind low to chase watts.** At your low power,
cadence is a *metabolic* dial, not a *joint* one — the choice is purely about
delivering a clean aerobic stimulus, and a slightly higher cadence does that best
under an HR clamp.

Your actual rides have been **low** (72 rpm on Jun 13, 78–84 on the Z2 rides) —
below even the current band. Zwift's nudge toward ~85–95 is the right direction.

## The evidence, with the numbers

**1. The "economy paradox" — most economical cadence is LOW, but nobody trains there.**
Lowest O₂ cost / highest gross efficiency at submaximal power sits at **~55–65 rpm**
(Chavarren & Calbet 1999: O₂ cost always lowest at 60 rpm across 54–93% VO₂max;
Foss & Hallén 2004: gross efficiency peaks ~80 rpm in elites, 120 rpm is ~12%
worse). Yet trained riders self-select **85–95** (Lucía 2001 pros: 89 flat / 92 TT).
Why ride "less efficiently"? Because lower cadence = higher force per stroke = more
fast-twitch recruitment and faster muscular fatigue. Riders trade a few % of
whole-body economy to **offload the muscle onto the cardiovascular system**
(Takaishi 1996: lowest-fatigue cadence 80–90 rpm ≠ lowest-O₂ cadence 70 rpm).

**2. Optimal cadence rises with power — which is why low power ⇒ lower optimum.**
Foss & Hallén ≈ 60 / 76 / 87 / 98 rpm at 100 / 200 / 300 / 400 W _(widely cited,
primary abstract not directly verified)_; Frontiers 2024: 66 rpm at LT1 → 84 at
VO₂max. Lucía 2004: pros at **366 W** are *more* efficient at 100 than 60 rpm. So
the "spin fast" rationale is strongest at high power; at your ~110 W the pure-economy
optimum is genuinely low — but economy isn't the Z2 goal (see #4).

**3. Higher cadence costs a few bpm at the same watts.** Stebbins 2014: 80 → 100 rpm
raised HR ~3–4% (**≈ +5 bpm**) and VO₂ ~4% at matched power. Rule of thumb:
**~+5 bpm per +20 rpm.** Under an HR clamp this means a higher cadence makes the
controller settle on *fewer* watts — that's expected and fine (see #4).

**4. The HR-clamp twist — low cadence buys "fool's gold watts."** Holding HR, a
lower cadence shows more watts, but it earns them mostly by loading the *muscle*
harder (force/stroke ↑, Type-II recruitment ↑), **not** by adding aerobic stimulus.
Aerobic adaptation (capillaries, mitochondria, stroke volume) tracks **cardiovascular
load + time-in-zone** — which the HR clamp already fixes — not displayed watts
(volume-vs-intensity meta-regression; cardiovascular-adaptation reviews). **So
optimizing the watts number by grinding actively pulls the wrong way for your goal.**
This is exactly your Jun 13 ride: 170 W @ 125 bpm at 72 rpm wasn't a fitness jump,
it was the low-cadence muscular-load artifact. Corollary: **EF / watts-at-HR is
cadence-confounded** — it's only a clean fitness signal when cadence is held roughly
constant across compared rides (one more reason to fix the band).

**5. The "low cadence burns more fat" idea is wrong here — don't use it.** The
substrate story is weak and frame-dependent. At a fixed *metabolic rate* (closest to
an HR clamp), the best primary study (Beneke & Alkhatib 2015) found **higher** cadence
*reduced* carbohydrate reliance — i.e. if anything slightly more fat-favorable, the
opposite of folk wisdom. And Ahlquist 1992: at matched cost, **50 rpm depleted more
Type-II glycogen than 100 rpm** (49% vs 33%) — low cadence hits fast-twitch harder.
Net: fat oxidation is driven by **intensity (staying sub-LT1)**, not cadence. Don't
pitch cadence as a fat lever.

**6. Joint load is a non-issue at your power.** Torque ≈ power/angular-velocity. At
~110 W: ~16 N·m (60 rpm) → ~11 N·m (95 rpm); peak pedal force only ~110–185 N (small
next to bodyweight-scale forces). The "spin to save your knees" advice scales with *power* —
at 250–400 W those forces are 4–7× larger and it matters; at 110 W it's negligible
(Ericson & Nisell even found **no** cadence effect on knee force at 120 W).
**Bodyweight doesn't change crank torque on a fixed trainer.** So choose cadence for
stimulus quality, not force. (Caveat: prior knee pain → still avoid sustained <70 rpm
grinding.)

**7. Coaches converge on "self-selected, comfortable-high" — no magic number.** CTS
75–95; Friel ~upper-comfortable (~95) trained as a skill; Dylan Johnson "least
muscle-activating, individual, rises with power." Two myth-corrections:
- **San Millán does _not_ prescribe a Z2 cadence** — the "85–95 rpm, recruits
  fast-twitch" line attributed to him is apocryphal blog reasoning, not his words.
  (The *reasoning* still happens to support biasing high.)
- **Low-cadence "strength/torque" work is a Z3–Z4 tool, not Z2** (CTS, TrainingPeaks
  both place it at tempo/sweetspot). At Z2 power the torque is too low to drive that
  adaptation. Don't program grinding *in* Zone 2.

**8. Spin-up drills — real but modest, and not for every ride.** Purpose is
neuromuscular/pedal-smoothness (coaching-grade evidence, not strong RCT). Consensus
dose: **1–2 dedicated sessions/week**, low power (50–60% FTP), 30–60 s reps at
105–125 rpm (highest non-bouncing cadence). Firing one every 5 min on *every* Z2 ride
adds cardiovascular cost and repeatedly perturbs the HR clamp (each spin-up spikes HR
→ controller drops power → muddies the steady stimulus).

## Concrete recommendation for the app

- **Z2 target cadence band: 85–95 rpm** (raise floor from 80; center ~90). Guardrail,
  not a metronome — if natural cadence sits 88–92, leave it.
- **Bias the cue slightly high, never toward grinding** — under the HR clamp, "spin a
  bit more" is the correct nudge; "more watts at this HR by grinding" is the trap.
- **Keep the <50 rpm "keep pedaling" warning** as-is (it's a coasting detector,
  unrelated to optimal cadence).
- **Make the every-5-min spin-up OFF by default** for steady Z2; expose a separate
  ~1×/week "neuromuscular" toggle (4–6 spin-ups, 30–60 s @ 110–120 rpm, spaced out).
- **For fitness tracking:** holding cadence in a fixed band is what makes your
  power-at-HR / EF trend actually comparable ride-to-ride (#4).

## Implemented in the app (2026-06-13)

- **Band floor 80 → 85** (`cadence_target_low=85`; 85–95, center 90). `z2_metrics`
  in-band % follows.
- **Asymmetric, escalating grinding cue:** below band → amber "spin up"; after ~12 s
  of *sustained* grinding it escalates to red + pulse **and a gentle repeating
  audio nudge** (`cues.grind`). The high side is never nudged (benign under the
  clamp). Guardrail, not metronome — only fires on sustained grind, so 88–92
  self-selection is left alone.
- **<50 rpm "keep pedaling" floor warning** kept as-is (coasting detector).
- **Spin-up drill is off the steady presets**; `cadence_plan` retuned to the
  research dose (~weekly, spaced ~every 10 min, 45 s reps) and documented as the
  opt-in neuromuscular session.
- **Post-ride flag:** a ride whose avg cadence fell below the band is marked
  "⚠ … rpm — low, inflates W/HR" in the saved banner, so a grind can't be misread
  as a fitness gain (the Jun-13 trap).
- **Step test pins ~90 rpm** on every step (cadence shifts a1 *and* watts-at-HR);
  ladder now starts **100 W, +20 W** to the clamp (the watts land lower at 90 rpm than
  low-cadence riding implied — see docs/calibrate-pivot-2026-06.md for the locked
  ladder geometry).

## Sources (primary unless noted)

- Chavarren & Calbet 1999, O₂ cost lowest at 60 rpm — https://pubmed.ncbi.nlm.nih.gov/10541922/
- Foss & Hallén 2004, most economical cadence rises with workload — https://link.springer.com/article/10.1007/s00421-004-1175-5
- Lucía 2001 (pro field cadences) — https://pubmed.ncbi.nlm.nih.gov/11474339/
- Lucía 2004, pros more efficient at high cadence @366 W — https://pubmed.ncbi.nlm.nih.gov/15179176/
- Takaishi 1996, fatigue-optimal (80–90) ≠ O₂-optimal (70) — https://pubmed.ncbi.nlm.nih.gov/8970143/
- Optimal cadence vs intensity (LT1 66 → VO₂max 84) — https://pmc.ncbi.nlm.nih.gov/articles/PMC11027132/
- Stebbins 2014, +5 bpm / +4% VO₂ at 100 vs 80 rpm — https://pmc.ncbi.nlm.nih.gov/articles/PMC3918546/
- Beneke & Alkhatib 2015, high cadence reduces CHO at given metabolic rate — https://pmc.ncbi.nlm.nih.gov/articles/PMC4314601/
- Ahlquist 1992, 50 rpm depletes more Type-II glycogen than 100 rpm — https://pubmed.ncbi.nlm.nih.gov/1385118/
- Ericson & Nisell 1986/87, knee forces ∝ workload, not cadence — https://pubmed.ncbi.nlm.nih.gov/3728780/ , https://pubmed.ncbi.nlm.nih.gov/3628491/
- Volume-vs-intensity adaptation meta-regression — https://www.gethealthspan.com/research/article/exercise-volume-intensity-systematic-review
- CTS cadence science (75–95, no universal optimum) — https://trainright.com/science-of-cycling-cadence-training/
- TrainingPeaks high-cadence base workouts (Holmes) — https://www.trainingpeaks.com/blog/3-high-cadence-cycling-workouts-base-training/
- San Millán Z2 (no cadence prescription) — https://www.highnorth.co.uk/articles/zone-2-training-inigo-san-millan

_Confidence flags: economy-paradox, HR-cost, joint-load math, and "adaptation tracks
cardiovascular load not watts" are well-supported. The fat-oxidation/cadence link is
weak and direction-dependent (don't assert it). Foss & Hallén per-power rpm values
and Dylan Johnson exact wording are cited-but-unverified. The San Millán "85–95"
attribution is apocryphal; the low-cadence-builds-strength claim is a Z3–Z4 tool
misapplied to Z2._
