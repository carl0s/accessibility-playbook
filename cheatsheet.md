# Cheatsheet — Accessibility Knowledge Base

**[P]** Playbook · **[GD]** Giving a Damn · **[Appt]** Appt Handbook

## Which book for what?
| Need | Book |
|------|------|
| Accessible **government / client service**, org culture | **[P]** Playbook |
| **Mindset, advocacy, good→great**, vendor vetting | **[GD]** Giving a Damn |
| **Mobile app** build, WCAG criteria, testing | **[Appt]** Appt Handbook |

## WCAG 2.2 at a glance [Appt]
4 principles · 13 guidelines · 86 success criteria · levels A / AA / AAA (target A + AA).
**POUR**: **P**erceivable · **O**perable · **U**nderstandable · **R**obust.

### Most-cited criteria
| SC | Level | Rule |
|----|-------|------|
| 1.1.1 | A | Alt text for non-text content |
| 1.2.2 | A | Captions for prerecorded video |
| 1.3.1 | A | Info/relationships marked in code |
| 1.4.1 | A | Color never the only cue |
| 1.4.3 | AA | Contrast 4.5:1 text / 3:1 large-bold |
| 1.4.4 | AA | Text scales (200%) no truncation |
| 1.4.11 | AA | Non-text contrast 3:1 |
| 2.1.1 | A | Full keyboard operability |
| 2.1.2 | A | No keyboard trap |
| 2.4.7 | AA | Focus visible |
| 2.5.8 | AA | Target size ≥ 24×24 px |
| 3.1.1 | A | Language set |
| 3.3.1 | A | Errors identified in text |
| 4.1.2 | A | Name, Role, Value on all elements |
| 4.1.3 | AA | Status messages announced to AT |

## Contrast ratios [Appt]
Text **4.5:1** · large (≥24px) or bold (≥18.5px/700) **3:1** · icons/inputs/focus **3:1**.

## 6 disability categories [P][Appt]
Hearing · Cognitive · Mobility · Visual · Speech · Age-related (states: permanent / temporary / situational).

## 6 core mobile features [Appt]
Text scaling (≥200%) · Dark mode · Screen reader · Voice control · Switch control · External keyboard.

## 7 Universal Design principles [P]
Equitable use · Flexibility · Simple & intuitive · Perceptible info · Tolerance for error · Low physical effort · Size & space.

## The 6 resistance archetypes [GD]
Allergic to change · "Show me the business case" · Demands detailed proof · New-features-over-old · "Only a few users" · "Not our audience." → all countered by: civil rights need no ROI; substitution test; WCAG is non-prescriptive.

## Good → Great [GD]
Compliance→empathy · product→whole experience · research→test *with* disabled users · accessible design systems · release gates · speak at *design* events.

## App lifecycle (Shift Left) [Appt]
**Design**: contrast, 2×–3× text, portrait+landscape, grouped/annotated, simple language.
**Dev**: native > hybrid; Name/Role/Value; dynamic non-sticky; focus order; alt text; coded headings.
**Test**: WCAG level via Appt-EM; automated + manual; 80/20 screen-reader + keyboard pass.

## Always-on defaults (all books)
"Press 0" on phone trees [P] · no-time-limit save-and-resume forms [P][Appt] · single-pointer alternative for every gesture [Appt] · errors in text + fix suggestion [Appt] · test with disabled users, never simulate [GD] · WCAG is a floor, not a ceiling (all).

## Load-bearing truths
- "Technically accessible ≠ accessible" [P] — can the client *actually* use it?
- "Inaccessible products are broken products" [GD]
- "Accessibility is not a feature you toggle on/off" [Appt]
- "A rising accessibility tide raises all disabled users' boats" [GD]
- Curb-cut effect — features help more than the intended group [P][Appt]

## Key laws
ADA + Section 508 (US) · EAA + WAD → EN 301 549 (EU) · CRPD (UN) · Accessible Canada Act 2019 (CA) — all point to **WCAG**.
