# Coaching for Performance — Vanderbilt Learning Series

Single-page interactive classroom experience (Learning on Demand). Live at
https://me5231979.github.io/Coaching-for-Performance/ (GitHub Pages, served
from `gh-pages` — publish with
`git branch -f gh-pages main && git push -f origin gh-pages`).

Sister programs: AI Basics (me5231979/AI_Classroom), Navigating Difficult
Conversations (me5231979/Difficult_Conversations), catalog at
me5231979/Course_Library. Same engine, same standing principles.

## Standing design principles (do not regress these)

1. **Simulators, practice, and play throughout.** Every teaching section
   has an interaction; the GROW simulator (Coach Jordan) is the centerpiece.
2. **A reason and facilitation behind every activity.** Learner-visible
   "Why this matters" lines; activities labeled As a group / On your own
   with numbered steps and timings; solo variants everywhere.
3. **Every section facilitatable, learning validatable.** ATD runbook in
   `facilitator/notes.json` (Say / Do / Ask with anticipated responses /
   Debrief / Transition + briefing front matter + templates). Kirkpatrick:
   L1 fist-to-five, L2 recap mapped to objectives, L3 capstone + 7-day
   pulse + 30-day ratio re-poll (the Section 01 ratio meter is the baseline).
4. **Facilitator edition is generated, never hand-edited** — run
   `python3 tools/build-facilitator.py` after ANY change to index.html or
   notes.json. Its QR encodes the LEARNER url.
5. **Privacy by design.** Ratio meter and coaching plan are private; roles
   not names; practice topics low-stakes; coaching-vs-therapy line routed
   to EAP/HR in the runbook.
6. **Brand: Vanderbilt FLH system.** Black #1C1C1C / white / flat gold
   #CFAE70; Libre Caslon Display headlines (one italic word), Inter body,
   Antonio eyebrows; motion ≤400ms; real VU lockups (authorized use only).
7. **No frameworks.** One CSS file, one JS file, vendored QR lib,
   self-hosted fonts; hero montage streams from Higgsfield CDN with the
   particle canvas as fallback.

## Layout (15 slides)

Welcome/QR → Hero (objectives + montage) → Agenda →
01 Case for coaching (ratio meter + Project Oxygen video) → manifesto →
02 Telling default (style trainer) →
03 GROW (cards + video + Coach Jordan simulator) →
04 Powerful questions (converter + six-second rule) →
05 Feedforward (rules + Goldsmith video + classifier) →
06 Choose your model (cards + matcher) → 07 When not to coach →
Recap quiz → Capstone coaching plan → Glossary → Closing (commitment).

## Editing map

- Copy: `index.html` · Recap questions: `QUESTIONS` in `assets/js/main.js`
- Trainers: `makeTrainer` configs · GROW simulator: `STAGES` array
- Capstone maps: `MODEL` / `TRAP` in main.js
- Runbook: `facilitator/notes.json` (timing must sum: Full 90 / Core 60)
- Keep citations honest: Project Oxygen (Google re:Work), GROW (Whitmore /
  Performance Consultants), ICF competencies, Goldsmith Feedforward,
  Goleman styles, McKinsey controller→coach, Ibarra & Scoular (HBR),
  CLEAR (Hawkins), OSKAR (Jackson & McKergow).
