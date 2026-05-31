# [Appt] Ch 3: WCAG Principle 1 — Perceivable

## Core Idea
Users must be able to **perceive** content. If someone can't see the interface or hear the audio, the information must be available in an alternative form. WCAG 2.2 has 4 principles / 13 guidelines / 86 success criteria across levels A, AA, AAA (orgs typically target A + AA).

## Frameworks Introduced
- **Guideline 1.1 Text Alternatives**
  - **1.1.1 Non-text Content (A)** — alt text for all images/icons/graphs describing their *meaning*; decorative images excepted.
- **Guideline 1.2 Time-based Media**
  - **1.2.1 Audio/Video-only (A)** — transcript for audio-only; description for video-only.
  - **1.2.2 Captions, prerecorded (A)** — captions for all videos with sound.
  - **1.2.3 Audio Description / Media Alternative (A)** — transcript or audio description for prerecorded video.
  - **1.2.4 Captions, live (AA)** — real-time captions for live video with audio.
  - **1.2.5 Audio Description, prerecorded (AA)** — extra audio track for important visual info.
- **Guideline 1.3 Adaptable** (expose structure to assistive tech)
  - **1.3.1 Info and Relationships (A)** — headings/lists/tables marked in code, not just visually.
  - **1.3.2 Meaningful Sequence (A)** — AT reading order matches meaning.
  - **1.3.3 Sensory Characteristics (A)** — don't rely on shape/size/location/orientation/sound alone.
  - **1.3.4 Orientation (AA)** — usable in both portrait and landscape.
  - **1.3.5 Identify Input Purpose (AA)** — set input types for autofill (e.g. email).
- **Guideline 1.4 Distinguishable** (foreground vs background)
  - **1.4.1 Use of Color (A)** — color is never the only cue (add shape/number).
  - **1.4.2 Audio Control (A)** — audio >3s can be paused/stopped.
  - **1.4.3 Contrast Minimum (AA)** — text **4.5:1**; large/bold text **3:1**.
  - **1.4.4 Resize Text (AA)** — text scales (system font size) without truncation/overlap.
  - **1.4.5 Images of Text (AA)** — use real text, not images of text.
  - **1.4.10 Reflow (AA)** — no two-directional scrolling at once.
  - **1.4.11 Non-text Contrast (AA)** — icons/inputs/focus indicator **3:1**.
  - **1.4.12 Text Spacing (AA)** — enough space between paragraphs/letters/words (helps dyslexia).
  - **1.4.13 Content on Hover or Focus (AA)** — hover/focus content is dismissible and persistent.

## Key Concepts
- **Contrast ratios** — 4.5:1 normal text; 3:1 large/bold text and non-text/graphical elements.
- **Alt text** — describes *meaning*; skip purely decorative images.
- **Reflow** — content reachable without scrolling in two directions simultaneously.

## Mental Models
- **"Perceivable in an alternative way"** — every visual has a non-visual equivalent and vice versa.
- **Color is a cue, never the cue.**
- **Mark structure in code, not just in pixels.**

## Anti-patterns
- Text baked into images (won't scale).
- Color-only status (green=ok/red=error with no shape/text).
- Contrast below 4.5:1 (text) / 3:1 (large, non-text).

## Key Takeaways
1. Alt text on meaningful non-text content; captions + transcripts on media.
2. Hit contrast: 4.5:1 text, 3:1 large/bold and non-text.
3. Text scales to 200%+ without breaking; never use images of text.
4. Mark headings/lists/tables in code; keep a meaningful reading order.
5. Never convey info by color alone.

## Connects To
- **appt-ch07**: design-phase contrast & text-scaling guidance.
- **[Playbook] esdc-ch05**: plain language, alt text, captions from a comms angle.
