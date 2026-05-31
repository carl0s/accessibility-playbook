# [Appt] Ch 1: Disabilities & Features (mobile context)

## Core Idea
A disability occurs when a task isn't suited to someone's abilities — caused by personal traits *or* environment. ~1.3 billion people (16% of the world) have a permanent disability; nearly half of people over 60 have one or more. Accessibility is not a toggle; it must be woven into every stage of design, development, and testing.

## Frameworks Introduced
- **The 6 Disability Categories (app context)** — each maps to features and WCAG criteria:
  - **Hearing** (deaf/hard of hearing) — 430M, 70M deaf; depend on subtitles.
  - **Cognitive** (dyslexia, ADHD, memory loss) — 240M with dyslexia; trouble remembering/concentrating/reading.
  - **Mobility** (amputation, paralysis, spasm, rheumatism) — touch not always possible; need button/keyboard input.
  - **Visual** (blind/visually impaired) — 295M severely impaired, 43M blind.
  - **Speech** (stuttering, lisping, mutism) — 19M; voice commands hard.
  - **Age-related** — 442M; combined hearing/cognitive/mobility/visual/speech decline; fast-growing.

- **The 6 Core Accessibility Features** — design and test against all of them:
  1. **Text Scaling** — support ≥200% scaling; every screen needs a ScrollView; 1 in 4 users pick larger text.
  2. **Dark Mode** — ~30% prefer it; helps light-sensitive users and concussion recovery.
  3. **Screen Reader** — reads the screen aloud; gestures: swipe left/right = prev/next element, double-tap = activate. Essential for finding most issues.
  4. **Voice Control** — operate by voice ("Tap back", "Show labels"); vital for mobility impairments.
  5. **Switch Control** — internal (camera, blink) or external (button, joystick) switches for severe motor impairment.
  6. **External Keyboard** — full operability via keyboard; the key testing tool — if keyboard works, switch/voice control work better too.

## Key Concepts
- **Situational disability** — environment-induced (can't play sound in a quiet zone).
- **Permanent / temporary / situational** — the full disability spectrum.
- **"Accessibility is not a feature which can be toggled on or off."**
- **Curb-cut parallel** — good contrast also helps in sunlight; captions help when sound is off.

## Mental Models
- **"I'm not disabled, the world disables me."** (Darice de Cuba) — disability is a mismatch between task and ability/environment.
- **Build for your future self** — you're likely to have a disability one day.
- **The external keyboard is the master test** — pass it and other AT improves.

## Key Takeaways
1. Design for all six disability categories, not just vision/hearing.
2. Support the six core features: text scaling, dark mode, screen reader, voice control, switch control, external keyboard.
3. Text must scale to 200%+ without truncation/overlap — wrap screens in ScrollView.
4. Test with a screen reader and an external keyboard — they catch most issues.
5. Accessibility is woven in, never toggled on.

## Connects To
- **[Playbook] esdc-ch01/ch02**: the same disability categories from a service-delivery angle.
- **appt-ch03–ch06**: which WCAG criteria each feature satisfies.
- **[Giving a Damn] bh-ch02**: AT is framework/tool-specific (NVDA ≠ JAWS, HTML ≠ SWIFT).
