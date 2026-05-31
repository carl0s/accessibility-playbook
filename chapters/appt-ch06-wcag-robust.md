# [Appt] Ch 6: WCAG Principle 4 — Robust

## Core Idea
Users must be able to make **proper use** of apps across a wide variety of devices and assistive-technology versions. The mechanism: clean code and correct semantic exposure (name, role, value) for every interactive element.

## Frameworks Introduced
- **Guideline 4.1 Compatible**
  - **4.1.1 Parsing (A)** — source code free of errors and deprecated functions; AT may misbehave on non-conforming code.
  - **4.1.2 Name, Role, Value (A)** — every interactive element exposes:
    - **Name** — identifies the element (screen reader speaks it; voice control targets it).
    - **Role** — what to expect ("button" → activatable).
    - **Value** — current state/property/value (disabled, selected, 50%).
    - *Example*: a tab → name "Home", role "tab", property "selected", value "1 of 4".
  - **4.1.3 Status Messages (AA)** — status messages (errors, connection loss) are announced to AT without moving focus; blind users can't see new on-screen info appear.

## Key Concepts
- **Name / Role / Value (NRV)** — the semantic triple every custom/interactive component must expose; the single most-overlooked thing when building custom components.
- **Status message** — dynamic info (error, loading, offline) that must be programmatically announced.
- **Parsing** — conformant, non-deprecated code so AT behaves predictably.

## Mental Models
- **"Name, Role, Value" is the contract with assistive technology** — if a custom control lacks it, AT can't see it.
- **Robust = future-proof** — works across many devices, OS versions, and AT versions.
- **Custom components are where NRV breaks** — native controls usually get it for free.

## Anti-patterns
- Custom buttons/tabs/toggles with no exposed role or state.
- Status changes (errors, spinners, offline) that are silent to screen readers.
- Deprecated/error-laden code that confuses assistive technology.

## Key Takeaways
1. Set a correct Name, Role, and Value on every interactive element — especially custom components.
2. Announce status messages to AT without stealing focus.
3. Keep source code clean and standards-conformant (no deprecated functions).
4. Prefer native components when possible — they expose NRV by default (see appt-ch07 framework choice).

## Connects To
- **appt-ch07**: development guidance reiterates Name/Role/Value for custom components; native frameworks offer best support.
- **appt-ch04**: "Label in Name" (2.5.3) pairs with the Name part of NRV.
- **[Giving a Damn] bh-ch04**: accessible design systems expose the ARIA properties developers must set.
