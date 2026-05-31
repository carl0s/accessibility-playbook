# [Appt] Ch 4: WCAG Principle 2 — Operable

## Core Idea
Users must be able to **operate** the app with whatever technology they use — not only touch. Screen reader, voice control, switch control, and external keyboard users must all be able to drive every function.

## Frameworks Introduced
- **Guideline 2.1 Keyboard Accessible**
  - **2.1.1 Keyboard (A)** — all functionality usable via the keyboard interface (covers screen reader / switch / voice control).
  - **2.1.2 No Keyboard Trap (A)** — never get stuck; pop-ups/menus need an AT-activatable close button.
  - **2.1.4 Character Key Shortcuts (A)** — single-key shortcuts can be remapped/disabled (AT emulates keystrokes).
- **Guideline 2.2 Enough Time**
  - **2.2.1 Timing Adjustable (A)** — time limits adjustable; best to avoid time limits.
  - **2.2.2 Pause, Stop, Hide (A)** — moving/flashing content can be paused/stopped/hidden.
- **Guideline 2.3 Seizures**
  - **2.3.1 Three Flashes or Below Threshold (A)** — no more than 3 flashes per second.
- **Guideline 2.4 Navigable**
  - **2.4.1 Bypass Blocks (A)** — skip repeated content (menus).
  - **2.4.2 Page Titled (A)** — each screen has a clear title.
  - **2.4.3 Focus Order (A)** — logical focus order (left→right, top→bottom).
  - **2.4.4 Link Purpose in Context (A)** — link purpose clear from link + surrounding text.
  - **2.4.5 Multiple Ways (AA)** — reach screens via more than one path (search, re-viewable onboarding).
  - **2.4.6 Headings and Labels (AA)** — descriptive headings and labels.
  - **2.4.7 Focus Visible (AA)** — focused element clearly indicated (e.g. focus background color).
  - **2.4.11 Focus Not Obscured, minimum (AA)** — focused element stays at least partially visible.
- **Guideline 2.5 Input Modalities**
  - **2.5.1 Pointer Gestures (A)** — alternative (e.g. button) for multi-point/path gestures.
  - **2.5.2 Pointer Cancellation (A)** — activate on up-event, not down — allow cancel.
  - **2.5.3 Label in Name (A)** — the accessible name includes the visible text label.
  - **2.5.4 Motion Actuation (A)** — alternative for motion-triggered actions; allow disabling.
  - **2.5.7 Dragging Movements (AA)** — single-pointer alternative to drag (tap/long-press).
  - **2.5.8 Target Size minimum (AA)** — targets at least **24×24 px** with spacing.

## Key Concepts
- **Keyboard interface** — the umbrella covering screen reader, switch control, voice control, external keyboard.
- **Keyboard trap** — being unable to escape a component without a mouse/touch.
- **Target size** — 24×24 px minimum for reliable activation.
- **Gesture/motion alternatives** — every gesture or shake needs a simple-pointer fallback.

## Mental Models
- **"If you can't do it with a keyboard, it isn't operable."**
- **Every gesture needs a button** — pinch, swipe, drag, shake all need single-pointer alternatives.
- **Activate on release, not on touch** — so users can cancel.

## Anti-patterns
- Keyboard traps in modals/overlays with no AT-reachable close.
- Drag-and-drop with no tap alternative.
- Tiny touch targets (<24×24 px).
- Actions triggered only by shaking/tilting.
- Time limits that can't be extended.

## Key Takeaways
1. Make everything keyboard-operable; eliminate keyboard traps.
2. Provide single-pointer alternatives for gestures, drag, and motion.
3. Targets ≥24×24 px; logical, visible focus order.
4. Avoid time limits; allow pause/stop/hide of motion; ≤3 flashes/sec.
5. Descriptive titles, headings, labels; visible accessible name in the technical name.

## Connects To
- **appt-ch01**: the AT (screen reader, switch, voice, keyboard) these criteria serve.
- **appt-ch07**: focus order and dynamic-interface dev guidance.
- **[Playbook] esdc-ch05**: "build for keyboard use only; don't demand precision."
