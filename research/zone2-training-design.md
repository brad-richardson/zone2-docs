# Zone 2 Workout Design — Research Notes (June 2026)

Findings that shaped zone2's presets. Full sourcing inline.

## The HR-clamp design is endorsed, not a compromise
When HR and power diverge (cardiac drift), HR is the more honest signal of
physiological state. San Millán (the coach behind the Zone 2 boom) uses HR as
the primary metric and accepts declining power — staying under the first
lactate threshold matters more than holding watts. TrainerDay's HR+ mode
implements exactly this. Friel-school "power leads, HR informs" reconciles:
for the Z2 fat-oxidation goal specifically, clamp HR and let power fall.
(highnorth.co.uk, trainerday.com, podcastnotes.org Attia #201)

## Steady beats undulating for pure Z2
San Millán: the benefit requires the *entire* duration in zone — surges spike
lactate, which suppresses fat oxidation for up to ~30 minutes after each
surge. Zwift's "Zone 2" workouts (60–75% undulations, 10–15s bursts, tempo
bumps) optimize engagement, not the Z2 stimulus. zone2's pure presets hold
one HR band, flat.

## Duration & frequency
- Minimum effective session: ~45 min (beginners adapt to 30–45)
- Standard: 60 min (TrainerRoad Pettit archetype)
- Ideal for trained athletes: 90 min; long ride 2 h+
- One continuous session > the same time split in two (PMC11319183: 1x60
  produced greater adaptive stress than 2x30)
- Frequency (San Millán): 2 d/wk maintains, 3+ improves, 4 ideal;
  ~300–400 min/wk
- Setting the target: the DFA-a1 step test (VT1 = a1 crossing 0.75) minus a small
  margin, or roughly 67–73% max HR (centre ~70%) / 80–87% threshold (LTHR) — the
  figures zone2 actually ships. *(Superseded: the old "talk test breaks" landmark
  is dropped — VT1 is validated by its own DFA-a1 crossing instead.)*

## Cadence drills: the legitimate variety
Power/HR-neutral, so they don't violate continuity:
- Spin-ups: 45–60 s at 110–125 rpm every 5 min, starting after 15 min
  (TrainingPeaks high-cadence template), 1–2 sessions/wk
- Blocks: 6 min alternating 70/85/100 rpm at constant power
  (Zwift FTP Builder "Foundation" model)

## Warmup / cooldown
Pure Z2 needs little: 5–10 min ramp in (lets HR rise into band before the
clamp engages), 3–5 min spin down. (FasCat, Zwift, TrainerDay all agree.)

## Rest-break presets (3x15 etc.)
Kept for saddle relief, honestly labeled: breaks don't spike lactate like
surges do, but continuity research says steady accumulates more stimulus.
Use when the alternative is a shorter ride.

## Realistic weekly targets (added after a sanity check)
The 300-400 min/wk figure is San Millán's prescription for trained athletes.
More realistic tiers for a working adult:
- ~135-180 min (3 x 45-60): San Millán's own time-crunched answer — "very
  important mitochondrial adaptations" at 1hr, 3-4 days/wk
- 180-240 min (3-4 hrs): Attia's longevity prescription; the knee of the
  diminishing-returns curve
- 300-400 min: performance tier
The stats view defaults its goal line to 120 weekly minutes (configurable in
Settings).

These presets live in the app's shared, portable core, so one definition drives
every client.
