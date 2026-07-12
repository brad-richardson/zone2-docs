# Dev calibration sessions — June 2026 (HR + R-R; raw ECG withheld)

A small set of **real indoor-cycling sessions captured during development** of
zone2, kept here to reproduce the DFA-a1 calibration work and as a springboard
for anyone picking this up (see [`research/raw-pmd-fusion.md`](../../research/raw-pmd-fusion.md)).

> **Note:** the analysis scripts referenced below (`scripts/calibration_fusion.py`,
> `scripts/pmd_fusion/`) live with the **application code**, not in this data repo.
> The R-R here is a plain integer-millisecond list per sample, so you can also load
> it with any HRV library. See `research/raw-pmd-fusion.md` for the method.

## 🔒 Raw PMD (ECG + accelerometer) withheld for privacy

The per-ride `<id>.pmd.jsonl` sidecars — raw **single-lead ECG (130 Hz)** + chest
**accelerometer (200 Hz)** — are **deliberately NOT published.** Raw ECG is
biometric/health data and is, in principle, personally identifying
(heartbeat-as-fingerprint); committing it to public git history is effectively
permanent and unrevocable, and that's a one-way door not worth walking through for
a side project. The raw-PMD analysis that used these captures is fully preserved in
**code + figures + writeup** (`scripts/pmd_fusion/`, `docs/img/raw-pmd-*.png`,
`docs/raw-pmd-fusion.md` §4) — just not the underlying biometric. **To re-run the
PMD axes (alignment, ECG→R-R audit, EDR breakpoint), capture your own** with a
Polar H10 (`scripts/decode_pmd.py` / `scripts/pmd_fusion/` work on any session dir
with sidecars).

## What IS here (and why it's safe to publish)

Eight `<id>.json` session records — 1 Hz **HR, power, cadence, and R-R intervals**
(plus plan/band metadata). R-R is inter-beat *timing* (the basis of HRV), which
every HRV app exports and is **not** the identifying ECG waveform. Scanned and
confirmed: **no name, email, tokens, Strava IDs, weight, notes** (all empty/`null`),
and no location (indoor; no GPS). Timestamps reveal workout dates/times only. These
reproduce the **DFA-a1 VT1 calibration** — the part of the analysis that actually
ships.

## ⚠️ Provenance & quirks

Development captures, **not** a curated scientific dataset, and the app's planned
trajectory has since changed — do **not** read `plan_name` / `kind` as current
product behavior:

- The **`"Fitness test"` / `kind: "longevity_ramp"`** rides are from a **maximal
  ramp protocol that was DROPPED** (`calibrate-pivot-2026-06.md`). They're kept
  because the maximal one (`…cbb4f9`) is the ride that exposed the ventilatory
  breakpoint in the (now-withheld) PMD analysis.
- One ride (`…d51e6d`) is a **~2.5-min aborted** attempt.
- Quality varies: `…cd58f7`'s a1 never crossed 0.75; `…5f4e54` is the
  operationally-representative Zone-2 calibration.
- Formats evolved mid-development (5-/7-/8-field positional rows). Use the loaders,
  not hand-parsing.

## Files

| id | plan (as recorded) | dur | PMD captured | notes |
|---|---|---|---|---|
| `20260613-023727-4e50be` | Steady Z2 45 min | 38 m | — | early; HR only, no R-R |
| `20260613-222224-6fda8f` | DFA-a1 step test | 25 m | — | a1 crossing ≈135 |
| `20260614-212743-5c11f4` | Steady · 45 min | 45 m | — | passive crossing ≈134 |
| `20260617-210151-cd58f7` | DFA-a1 step test | 19 m | withheld | a1 never crossed (stayed below VT1) |
| `20260617-213151-4cb065` | Train · 45 min | 25 m | withheld | steady reference |
| `20260619-121050-d51e6d` | Fitness test *(dropped protocol)* | 2.5 m | withheld | aborted |
| `20260619-121348-cbb4f9` | Fitness test *(dropped protocol)* | 21 m | withheld | maximal ramp, HR 97→171 — the EDR/breakpoint ride |
| `20260620-111335-5f4e54` | Zone 2 calibration | 20 m | withheld | operational calibration, a1 crossing ≈133 |

"PMD captured = withheld" means a raw `.pmd.jsonl` sidecar was recorded during the
ride but is not published (see above); `ride.pmd_file` in the JSON still names the
(absent) sidecar.

**Format:** 1 Hz session record, positional sample rows
`[t, hr, power, cadence, target, …, rr_ms(idx 7), src(idx 8), hr_flags(idx 9),
seg(idx 10)]` (older files are shorter). Schema: `src/zone2/session.py`.

## Use

```bash
# DFA-a1 VT1 / Zone-2 band fusion (uses the R-R in the JSONs — works on this set):
uv run python scripts/calibration_fusion.py datasets/dev-calibration-2026-06 --age 40

# The raw-PMD fusion report needs .pmd.jsonl sidecars (withheld here) — point it at
# your OWN capture dir:
uv run --extra analysis python -m scripts.pmd_fusion.report <your-sessions-with-pmd>
```
