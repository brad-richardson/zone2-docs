# zone2-docs

Public pages, build notes, and sample data for **Zone2** — an HR-clamped Zone 2
training app for smart trainers (iPhone & iPad).

This repository serves the app's website via GitHub Pages and hosts the
shareable research and sample data. **It does not contain the application source
code** — that lives in a separate repository.

## Live site

Once GitHub Pages is enabled (Settings → Pages → deploy from `main`, root):

- **Home** — https://brad-richardson.github.io/zone2-docs/
- **Build notes & science** — https://brad-richardson.github.io/zone2-docs/notes.html
- **Support** — https://brad-richardson.github.io/zone2-docs/support.html
- **Privacy Policy** — https://brad-richardson.github.io/zone2-docs/privacy.html

## What's here

```
index.html          Landing page
notes.html          "How it works & what I learned" — the open build/science writeup
support.html        Support page (App Store support URL)
privacy.html        Privacy policy (App Store privacy URL)
style.css           Shared "Calm Instrument" styling (matches the app)
research/           Deeper source notes behind the writeup
  zone2-training-design.md   Zone 2 preset research (steady vs undulating, dose)
  cadence.md                 Cadence under an HR clamp (personal metrics redacted)
  raw-pmd-fusion.md          The raw ECG/ACC respiration study — a recorded negative result
  img/                       Figures for the PMD study
datasets/
  dev-calibration-2026-06/   8 real, scrubbed indoor sessions (HR, power, cadence, R-R)
  real_rr_nsr2db.txt         PhysioNet R-R fixture the DFA-a1 math is validated against
```

## Sample data & privacy

The sessions in `datasets/dev-calibration-2026-06/` are **real rides, scrubbed**:
no name, email, tokens, Strava IDs, body metrics, notes, or location — see that
folder's README. They contain beat-to-beat (R-R) *timing*, which every HRV app
exports, and reproduce the DFA-a1 calibration baseline.

**Deliberately withheld:** the raw single-lead ECG / accelerometer sidecars behind
the respiration study. Raw ECG is biometric and effectively unrevocable once in
public git history, so it is not published. The study is fully preserved in the
writeup, figures, and (in the app repo) the analysis code.

## License

Documentation and data in this repository are licensed **CC BY 4.0** — see
[`LICENSE`](LICENSE). The PhysioNet fixture (`datasets/real_rr_nsr2db.txt`) is
third-party data under its own [PhysioNet license](https://physionet.org/content/nsr2db/1.0.0/);
keep its attribution header intact.
