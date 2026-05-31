# [Appt] Ch 7: Approach — Design, Development, Testing

## Core Idea
Accessibility is a team effort across disciplines and across the whole lifecycle. Catch issues early ("Shift Left") — discovering them in design is far cheaper than in code. The chapter gives concrete guidance for the three development phases plus an org-maturity lens.

## Frameworks Introduced
- **W3C Accessibility Maturity Model — 7 dimensions** (assess how accessible your *organization* is):
  Communications · Knowledge & Skills · Support · Development Process · Personnel · Procurement · Culture.

- **Design phase ("Shift Left")**:
  - **Contrast**: text ≥ 4.5:1; bold (≥18.5px/700) or large (≥24px) text ≥ 3:1; graphical elements ≥ 3:1.
  - **Text Scaling**: design at 2× and 3× font size; nothing overlaps or truncates; leave room to expand.
  - **Orientation**: usable in portrait and landscape.
  - **Structure**: simple, clear, consistent; group related elements (and annotate groups for devs) — gives bigger touch targets and one-shot screen-reader announcements.
  - **Language**: simple, short; careful heading wording (headings are signposts); labeled inputs with clear instructions and error messages.

- **Development phase**:
  - **Framework**: native offers the best accessibility support; hybrid/cross-platform may lack access to features — native is best for a fully accessible app.
  - **Name, Role, Value**: set on all interactive elements (often overlooked on custom components).
  - **Dynamic Interface**: no fixed width/height — elements grow with text scaling/orientation; avoid sticky top/bottom elements (waste landscape space, clash with keyboard).
  - **Focus Order**: left→right, top→bottom; adjust in code if needed.
  - **Alternative Text**: on all non-decorative images.
  - **Headings**: marked in code so AT users can jump heading-to-heading.

- **Testing phase**:
  - **Conformance**: test against a target (e.g. WCAG AA). W3C's WCAG-EM is web-oriented, so Appt created **Appt-EM** for apps.
  - **Automated testing**: platform-specific, cross-platform, and framework-specific tools (free & paid) — complements manual.
  - **Manual testing (80/20 rule)**: ~80% of issues found with ~20% effort. Quick checks:
    - *Without AT*: captions (1.2.2), transcript/audio desc (1.2.3), rotation (1.3.4), info clear without color (1.4.1), required fields/expected data (3.3.2).
    - *Text scaling*: correct at 200% (1.4.4).
    - *Contrast*: 4.5:1 text / 3:1 large & non-text (1.4.3, 1.4.11).
    - *Screen reader*: alt text (1.1.1), clear layout (1.3.1), full operability (2.1.1), no traps (2.1.2), logical order (2.4.3), correct name/role/value (4.1.2).

## Key Concepts
- **Shift Left** — fixing in design is cheaper than fixing in code.
- **Appt-EM** — the app-specific evaluation methodology (vs web-only WCAG-EM).
- **80/20 manual testing** — a screen reader + external keyboard finds most issues fast.
- **Native > hybrid/cross-platform** for accessibility feature access.

## Mental Models
- **Accessibility is a team effort across the whole lifecycle**, not one role's job.
- **Shift Left** — the earlier you catch it, the cheaper it is.
- **Manual + automated, not either/or** — automation can't find everything; a real screen-reader pass is essential.

## Anti-patterns
- Fixed-size elements that break under text scaling/rotation.
- Sticky headers/footers that eat landscape space and collide with the keyboard.
- Relying on automated tools alone (they miss most nuanced issues).
- Choosing hybrid/cross-platform when full accessibility is required without checking feature support.

## Key Takeaways
1. Shift Left: bake contrast, scaling, orientation, structure, and language into design.
2. Prefer native; set Name/Role/Value; build a dynamic, non-sticky interface; mark headings; logical focus order.
3. Test against a WCAG level with Appt-EM; combine automated tools with manual screen-reader/keyboard passes.
4. Use the 80/20 manual checklist for a fast first impression; bring in an expert for full evaluation.
5. Assess org maturity across the 7 W3C dimensions.

## Connects To
- **appt-ch03–ch06**: the criteria these phases satisfy.
- **[Giving a Damn] bh-ch04**: accessible design systems, release gates, testing with disabled users.
- **[Playbook] esdc-ch07**: the maturity model's "Culture" dimension mirrors Play 7.
