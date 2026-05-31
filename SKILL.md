---
name: accessability-playbook
description: "Accessibility knowledge base from three books: the AccessAbility Playbook (ESDC, accessible client service), Giving a Damn About Accessibility (Sheri Byrne-Haber, design/advocacy mindset), and the Appt Accessibility Handbook (Appt Foundation, mobile apps + WCAG). Use when applying frameworks for accessible service, inclusive/Universal Design, WCAG criteria, mobile app accessibility, plain language, accessibility culture/advocacy, or referencing these books' concepts."
allowed-tools:
  - Read
  - Grep
argument-hint: [topic, framework, WCAG criterion, or chapter id e.g. appt-ch03]
---

# Accessibility Knowledge Base (3 books)
**Generated**: 2026-05-31 · A unified KB across service delivery, design/advocacy, and mobile/WCAG.

| Tag | Book | Author | Lens |
|-----|------|--------|------|
| **[P]** | AccessAbility Playbook | ESDC (Gov. of Canada) | Accessible client service / org |
| **[GD]** | Giving a Damn About Accessibility | Sheri Byrne-Haber | Design, advocacy, mindset |
| **[Appt]** | Appt Accessibility Handbook | Appt Foundation | Mobile apps + WCAG criteria |

## How to Use This Skill

- **Without arguments** — load the cross-book core frameworks below.
- **With a topic** — ask about `WCAG contrast`, `Universal Design`, `personas`, `ableism`, `Name Role Value`, `release gate`, `plain language`; I read the relevant chapter.
- **With a chapter id** — `esdc-ch04`, `bh-ch01`, `appt-ch03`.
- **By book** — "what does Giving a Damn say about overlays?" → I scope to `bh-*`.

When a topic isn't in Core Frameworks below, I read the relevant chapter file before answering.

---

## Core Frameworks & Mental Models

### Mindset & advocacy [GD]
- **Root cause is people, not tech.** Name the **6 resistance archetypes** (allergic to change · wants a business case · demands proof · new-over-old · "only a few users" · "not our audience") and counter each.
- **Ableism + substitution test** — swap "disability" for another group; if unacceptable, it's ableist. Civil rights need no ROI.
- **Ship awful, then iterate** — first attempt beats the inaccessible 98%; run the **accessibility flywheel**, not a project. Not zero-sum.
- **Good → Great** — compliance→empathy, product→whole experience, research→testing *with* disabled users, accessible design systems, release gates, evangelize at *design* events.
- **Avoid overlays/plugins** — "pants on fire" claims that invite lawsuits.

### Service & organization [P]
- **5 Barrier Areas** audit: Physical Space · Policies & Processes · Language & Information · Awareness & Attitude · Technology.
- **Channel × Disability matrix** + **3-Lens checklist** (Service Design / Assistive Tech / Training & Culture) for in-person/phone/online. Six personas ("Billy's friends").
- **Person-first service**: ask "How may I help you?"; speak to the client, not the companion; service-animal & TTY/VRS etiquette.
- **Culture change**: Values → Governance → Awareness ("culture eats strategy for breakfast").

### Inclusive design [P]
- **7 Universal Design principles**: Equitable use · Flexibility · Simple & intuitive · Perceptible info · Tolerance for error · Low physical effort · Size & space.
- **Curb-cut effect**; **intersectionality**; "**technically accessible ≠ accessible**."

### WCAG & mobile build [Appt]
- **WCAG 2.2 = POUR**: **P**erceivable · **O**perable · **U**nderstandable · **R**obust (4 principles, 13 guidelines, 86 criteria; target A + AA).
- **Contrast**: 4.5:1 text, 3:1 large/bold & non-text. **Target size** ≥ 24×24 px. **Text scaling** ≥ 200%.
- **Name, Role, Value** on every interactive element (esp. custom components); announce **status messages** to AT.
- **Keyboard-first**: full operability, no traps, single-pointer alternative for every gesture/drag/motion.
- **Shift Left** lifecycle: Design → Development → Testing (manual screen-reader + keyboard 80/20 pass; Appt-EM); native > hybrid.
- **6 disability categories** (Hearing/Cognitive/Mobility/Visual/Speech/Age) × **6 features** (text scaling, dark mode, screen reader, voice control, switch control, external keyboard).

### Shared across all three
WCAG is a **floor, not a ceiling** · accessibility is **not a toggle** · always-on defaults: "press 0", no-time-limit save-and-resume forms, errors in text + fix suggestion, test *with* disabled users. Laws (ADA/508, EAA/WAD→EN 301 549, CRPD, Accessible Canada Act) all point to WCAG.

---

## Chapter Index

### [P] AccessAbility Playbook (ESDC) — service delivery
| id | Title | Key frameworks |
|----|-------|----------------|
| [esdc-ch01](chapters/esdc-ch01-learn-about-accessibility.md) | Learn about accessibility | 5 Barrier Areas, 6 disability types |
| [esdc-ch02](chapters/esdc-ch02-barriers-by-disability.md) | Understand barriers | Channel × Disability matrix, 6 personas |
| [esdc-ch03](chapters/esdc-ch03-involve-persons-from-the-start.md) | Involve from the start | 3 Engagement Pillars |
| [esdc-ch04](chapters/esdc-ch04-design-inclusive-experiences.md) | Design inclusively | 7 Universal Design principles, 3-Lens checklist, curb-cut |
| [esdc-ch05](chapters/esdc-ch05-accessible-communications.md) | Accessible communications | Plain language, print/signage/online specs |
| [esdc-ch06](chapters/esdc-ch06-develop-service-skills.md) | Develop service skills | Person-first language, TTY/VRS & service-animal etiquette |
| [esdc-ch07](chapters/esdc-ch07-accessible-culture.md) | Accessible culture | Role responsibilities, 3 culture steps |
| [esdc-ch08](chapters/esdc-ch08-inspiring-tools.md) | Inspiring tools | CX model, journey maps, assessment checklist |

### [GD] Giving a Damn About Accessibility (Byrne-Haber) — mindset
| id | Title | Key frameworks |
|----|-------|----------------|
| [bh-ch01](chapters/bh-ch01-give-a-damn.md) | People who don't give a damn | 6 resistance archetypes, ableism, substitution test |
| [bh-ch02](chapters/bh-ch02-first-attempt-awful.md) | Your first attempt will be awful | 5 learning truths, accessibility flywheel |
| [bh-ch03](chapters/bh-ch03-not-an-add-on.md) | Not an add-on service | Consultant red flags, specialization analogy |
| [bh-ch04](chapters/bh-ch04-good-to-great.md) | Good → great accessibility | 6 good-vs-great differentiators |

### [Appt] Appt Accessibility Handbook — mobile + WCAG
| id | Title | Key frameworks |
|----|-------|----------------|
| [appt-ch01](chapters/appt-ch01-disabilities-features.md) | Disabilities & features | 6 categories, 6 core features |
| [appt-ch02](chapters/appt-ch02-legislation.md) | Legislation | CRPD, EAA/WAD/EN 301 549, ADA/508 |
| [appt-ch03](chapters/appt-ch03-wcag-perceivable.md) | WCAG: Perceivable | Guidelines 1.1–1.4, contrast |
| [appt-ch04](chapters/appt-ch04-wcag-operable.md) | WCAG: Operable | Keyboard, gestures, target size |
| [appt-ch05](chapters/appt-ch05-wcag-understandable.md) | WCAG: Understandable | Language, predictable, input assistance |
| [appt-ch06](chapters/appt-ch06-wcag-robust.md) | WCAG: Robust | Name/Role/Value, status messages |
| [appt-ch07](chapters/appt-ch07-approach.md) | Approach | Maturity model, Shift Left, testing |

## Topic Index

- **Ableism / resistance / advocacy** → bh-ch01
- **Alt text** → appt-ch03, esdc-ch05
- **Assessment / audit** → esdc-ch08, appt-ch07
- **Barriers** → esdc-ch01, esdc-ch02
- **Channels (in-person/phone/online)** → esdc-ch02, esdc-ch04
- **Contrast** → appt-ch03, appt-ch07
- **Culture / governance / maturity** → esdc-ch07, appt-ch07
- **Curb-cut effect** → esdc-ch04, appt-ch01
- **Design systems / release gates** → bh-ch04, appt-ch07
- **Disability types** → esdc-ch01, esdc-ch02, appt-ch01
- **Forms (time limits, errors, auth)** → esdc-ch04, appt-ch05
- **Good vs great** → bh-ch04
- **Keyboard / gestures / target size** → appt-ch04
- **Legislation (ADA/508/EAA/CRPD)** → appt-ch02, bh-ch01
- **Name, Role, Value / status messages** → appt-ch06
- **Overlays / plugins / widgets** → bh-ch01
- **Perfectionism / first attempt / flywheel** → bh-ch02
- **Personas** → esdc-ch02
- **Person-first language** → esdc-ch06
- **Plain language** → esdc-ch05, appt-ch05
- **Predictable behavior / language set** → appt-ch05
- **Screen reader / voice / switch control** → appt-ch01, appt-ch04
- **Testing (manual/automated/Appt-EM)** → appt-ch07
- **Universal Design (7 principles)** → esdc-ch04
- **Vendor / consultant evaluation** → bh-ch03
- **WCAG (POUR, criteria)** → appt-ch03–ch06
- **Text scaling / dark mode** → appt-ch01, appt-ch03

## Supporting Files

- [glossary.md](glossary.md) — all key terms, source-tagged
- [patterns.md](patterns.md) — techniques across strategy, org, design, build
- [cheatsheet.md](cheatsheet.md) — WCAG table, contrast, "which book for what", quick rules

---

## Scope & Limits

Covers three accessibility books spanning **service delivery [P]**, **design/advocacy mindset [GD]**, and **mobile apps + WCAG [Appt]**. The Appt WCAG summaries are condensed (level A/AA only, paraphrased) — for exact, normative WCAG text consult the W3C spec; for app implementation specifics see appt.org. [GD] reflects a US-centric legal/2021 snapshot. Pair with project tooling and a real screen-reader pass for hands-on work.
