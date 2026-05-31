# [Appt] Ch 5: WCAG Principle 3 — Understandable

## Core Idea
Users must be able to **understand** content and behavior. Set the language so assistive tech pronounces text correctly, make app behavior predictable, and help users avoid and recover from input errors.

## Frameworks Introduced
- **Guideline 3.1 Readable**
  - **3.1.1 Language of Page (A)** — set the app language so text-to-speech pronounces correctly.
  - **3.1.2 Language of Parts (AA)** — mark language of text written in another language.
- **Guideline 3.2 Predictable**
  - **3.2.1 On Focus (A)** — focusing an element must not unexpectedly activate it.
  - **3.2.2 On Input (A)** — entering data must not cause unexpected context change unless warned.
  - **3.2.3 Consistent Navigation (AA)** — navigation stays in the same place (back button top-left).
  - **3.2.4 Consistent Identification (AA)** — icons keep the same function (magnifier = search, never enlarge).
  - **3.2.6 Consistent Help (A)** — help is reachable from a consistent place.
- **Guideline 3.3 Input Assistance**
  - **3.3.1 Error Identification (A)** — clearly state which entry is wrong and why, in text.
  - **3.3.2 Labels or Instructions (A)** — label fields; mark required/optional; state expected formats.
  - **3.3.3 Error Suggestion (AA)** — suggest how to fix (e.g. expected date format yyyy-mm-dd).
  - **3.3.4 Error Prevention — Legal/Financial/Data (AA)** — allow undo, correct, or confirm for consequential submissions.
  - **3.3.7 Redundant Entry (A)** — don't re-ask previously entered info; auto-populate or offer to select.
  - **3.3.8 Accessible Authentication, minimum (AA)** — allow password managers / copy-paste; don't force memory/cognitive tests.

## Key Concepts
- **Predictability** — same layout, same icon meanings, no surprise context changes.
- **Input assistance** — clear labels, format hints, error messages *in text*, and fix suggestions.
- **Redundant entry / accessible auth** — reduce memory load (key for cognitive disabilities).

## Mental Models
- **Set the language, or the screen reader mispronounces everything.**
- **No surprises** — focus/input should never trigger unexpected actions or jumps.
- **Errors in text, with a suggested fix** — not color or position alone.
- **Don't tax memory** — auto-fill known data; allow password managers.

## Anti-patterns
- Unset/incorrect app language → garbled TTS.
- Auto-submitting or jumping on focus/input without warning.
- Icons that change meaning between screens.
- Errors signaled only by red border, no text/explanation.
- Re-asking data the user already entered; blocking password managers.

## Key Takeaways
1. Set page and parts language for correct pronunciation.
2. Keep behavior predictable: consistent navigation, icons, and help; no surprise activations.
3. Label inputs and state expected formats; identify errors in text with fix suggestions.
4. Allow undo/correct/confirm for legal/financial/data submissions.
5. Minimize memory load — avoid redundant entry; support password managers (accessible auth).

## Connects To
- **appt-ch07**: clear-language and labeled-input design guidance.
- **[Playbook] esdc-ch05**: plain language and clear error/instruction design.
- **[Playbook] esdc-ch02/ch04**: save-and-resume, no-time-limit forms for cognitive load.
