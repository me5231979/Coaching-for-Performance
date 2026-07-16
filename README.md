# Coaching for Performance — Building Managers Who Grow People

An interactive, single-page teaching site for **people managers, team leads,
and HR/talent partners** at Vanderbilt. A **Learning on Demand** program:
the facilitator projects it while learners scan a QR code and work every
exercise on their own devices, or share the link for self-paced review.

Part of the Vanderbilt Learning Series, in the FLH visual system, alongside
[AI Basics](https://me5231979.github.io/AI_Classroom/) and
[Navigating Difficult Conversations](https://me5231979.github.io/Difficult_Conversations/).
Catalog: [Course Library](https://me5231979.github.io/Course_Library/).

- **Learner edition:** https://me5231979.github.io/Coaching-for-Performance/
- **Facilitator edition:** https://me5231979.github.io/Coaching-for-Performance/facilitator/

## Running it

Plain HTML/CSS/JS, no build step:

```bash
python3 -m http.server 8000
```

## What it teaches (7 sections)

1. The case for coaching — Google's Project Oxygen, McKinsey's controller→coach
2. Your telling default — Goleman's styles, why doers over-direct
3. The GROW conversation — Whitmore's model, practiced against a virtual coachee
4. Powerful questions — ICF's three tests, the six-second silence
5. Feedforward — Marshall Goldsmith's future-only exchange
6. Choose your model — GROW vs CLEAR vs OSKAR
7. When NOT to coach — situational judgment (Ibarra & Scoular, HBR)

Ends with a scored recap quiz, a **capstone coaching plan** (model, written
opening question, telling-trap counter-move, and a date within 7 days), a
flip-card glossary, and a commitment close. `worksheet.html` mirrors the
capstone on paper; `cheatsheet.html` is the take-home reference.

## The interactive tools

| Slide | Tool | What learners do |
|---|---|---|
| The case | **Coaching ratio meter** | Rate their last five 1:1s; the readout responds; baseline for the 30-day re-poll |
| Telling default | **Catch the style** | Label five manager lines: directing, pacesetting, or coaching |
| GROW | **Coach Jordan simulator** | Run a full 4-stage GROW conversation; the coachee's replies change with every choice |
| Powerful questions | **The converter** | Pick the rewrite that passes open / clean / theirs |
| Feedforward | **Past, future, or advice?** | Classify five lines against Goldsmith's rules |
| Models | **Match the model** | Fit GROW, CLEAR, or OSKAR to four coachees |
| Recap | **Scored quiz** | 6 questions mapped 1:1 to the objectives |
| Capstone | **My Coaching Plan** | Build and copy a dated plan with a written opening question |

## Instructional design

- **Bloom's ladder:** objectives run Explain → Apply → Analyze/Convert →
  Practice → Create-and-commit.
- **Kirkpatrick:** L1 fist-to-five at close; L2 inline checks + recap mapped
  to objectives; L3 capstone plan + 7-day pulse + the 30-day coaching-ratio
  re-poll (the ratio meter captures the baseline in session).
- **Adult learning (Knowles):** every exercise uses the learner's real
  1:1s, immediate applicability (a conversation this week), self-direction
  (choose your model), and experience as the raw material.

## The facilitator edition

Generated at `/facilitator/` by `python3 tools/build-facilitator.py` from
`facilitator/notes.json` — ATD-scripted rails (Say / Do / Ask with expected
answers / Debrief / Transition), a briefing slide (prep, materials,
contingencies, tough questions, copy-paste templates including the 30-day
ratio re-poll), and Full 90 / Core 60 timing. Its QR encodes the learner URL.

## Editing map

- Copy: `index.html` · Recap: `QUESTIONS` in `assets/js/main.js`
- Trainers: `makeTrainer` configs · Simulator: `STAGES` array
- Runbook: `facilitator/notes.json` (timing must sum Full 90 / Core 60)
- Publish: `git push origin main && git branch -f gh-pages main && git push -f origin gh-pages`
