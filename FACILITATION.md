# Facilitation Guide — Coaching for Performance

Every activity carries a learner-visible **"Why this matters"** line, and
every teaching section has (1) an **interactive tool or practice moment**,
(2) a **labeled, timed activity** — *As a group* or *On your own* — and
(3) a **validation point**.

The full runbook lives in [`facilitator/notes.json`](facilitator/notes.json)
on the **ATD facilitator-guide framework**: per section a verbatim **Say**
script, **Do** choreography, an **Ask** with anticipated responses, a
**Debrief** line, and a scripted **Transition**, plus front matter
(materials, prep checklists, contingencies, tough questions, and copy-paste
templates: pre-work invite, 7-day pulse, 30-day ratio re-poll).

The **facilitator edition is live at `/facilitator/`** — regenerate after
any change to `index.html` or `notes.json`:

```bash
python3 tools/build-facilitator.py
```

## Run of show — two paths

| Slide | Full (90 min) | Core (60 min) |
|---|---|---|
| Welcome / QR | 3 | 2 |
| Objectives | 2 | 1 |
| Agenda | 1 | — |
| 01 The case for coaching | 9 | 5 |
| Manifesto | 1 | — |
| 02 Your telling default | 8 | 5 |
| 03 The GROW conversation | 16 | 12 |
| 04 Powerful questions | 9 | 6 |
| 05 Feedforward | 12 | 8 |
| 06 Choose your model | 7 | 3 |
| 07 When NOT to coach | 6 | 4 |
| Recap quiz | 4 | 4 |
| My coaching plan (capstone) | 8 | 7 |
| Glossary | 1 | — |
| Closing / commitment | 3 | 3 |
| **Total** | **90** | **60** |

**Core-path rules:** the ratio poll, every trainer, the GROW simulator,
ONE direction of the pair roleplay, one Feedforward rotation, the recap,
and the capstone stay. Skip the agenda, manifesto, glossary, and the GROW
and Goleman videos. Per-section cuts live in each `coreNote`.

**Timing discipline:** GROW (16) and Feedforward (12) are the stretchy
blocks; talkative rooms will eat both. Protect the last 15 minutes (recap,
capstone, commitment) by trimming rotations and debriefs first, never the
capstone.

**Pre-work and follow-up:** send the pre-work invite with the calendar
invite (a primed room saves the roleplay five minutes of topic-hunting);
the 7-day pulse and the 30-day ratio re-poll templates live on the
facilitator briefing slide. `worksheet.html` is the no-device fallback.

**Practice norms (load-bearing):** real but low-stakes topics; roles, not
names; coaching practice is not therapy, and heavy disclosures route to
EAP/HR per the contingency table.

## Validation model

- **In the moment:** inline checks (01, 07), trainer scores (02, 04, 05,
  06), the GROW simulator outcome tier (03), the pair-roleplay coachee
  verdict ("you coached me" / "you managed me"), and triad rule-keeping
  in Feedforward.
- **End of session:** the 6-question recap maps 1:1 to the objectives
  (Level 2); the closing fist-to-five is the Level 1 check; the capstone
  plan and the model-and-day commitment round are the transfer artifacts.
- **After:** the 7-day pulse (Level 3), and the **30-day coaching-ratio
  re-poll** measured against the in-session baseline — the program's
  headline behavioral metric.
- **Deliberately not validated:** the ratio meter score and the plan's
  contents are private — facilitators must not collect them.
