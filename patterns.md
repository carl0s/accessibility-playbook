# Patterns & Techniques — Accessibility Knowledge Base

Source tags: **[P]** Playbook (ESDC) · **[GD]** Giving a Damn · **[Appt]** Appt Handbook.

## Strategy & Mindset

### Give a Damn first [GD]
**When**: any inaccessible product/team. **How**: recognize the root cause is people, not tech; name the resistance archetype (allergic to change / business-case / proof-demander / new-over-old / "small number" / "not our audience") and counter it. **Trade-off**: cultural work is slow but is the actual blocker.

### Ableism substitution test [GD]
**When**: someone defends an inaccessible decision. **How**: swap "disability" for another underrepresented group; if the statement is obviously unacceptable, it's ableist. **Trade-off**: confrontational; use to reframe, not to attack.

### Ship awful, then iterate (the flywheel) [GD]
**When**: starting out / paralyzed by perfectionism. **How**: accept the first attempt won't be great ("better than 98%"); run a continuous improvement loop, not a project. **Trade-off**: requires tolerating visible imperfection and criticism.

### Good → Great [GD]
**When**: already compliant, want excellence. **How**: compliance→empathy (AAA where it matters, colorblind/focus contrast); product→whole experience (docs/support/packaging); research→testing *with* disabled users; accessible design systems; release gates; evangelize at design events. **Trade-off**: needs cross-stakeholder commitment.

## Org & Process

### 5 Barrier Areas audit [P]
**When**: evaluating any service. **How**: check Physical Space, Policies & Processes, Language & Information, Awareness & Attitude, Technology. **Trade-off**: fast triage; pair with channel checklist.

### Culture change (Values→Governance→Awareness) [P]
**When**: making accessibility durable. **How**: express values, embed in governance (investment gates, tracking, accountability), raise awareness via repeated messaging. **Trade-off**: slow; "culture eats strategy for breakfast."

### W3C Maturity Model (7 dimensions) [Appt]
**When**: assessing org readiness. **How**: score Communications, Knowledge & Skills, Support, Dev Process, Personnel, Procurement, Culture. **Trade-off**: diagnostic, not a fix list.

### Vet accessibility vendors [GD]
**When**: procuring consulting. **How**: treat like security/privacy specialists; red flags = magic-wand claims, no disabled employees, "we do everything," can't define PDF/UA. **Trade-off**: buyer must do the homework.

### Co-design with persons with disabilities [P][GD]
**When**: building/improving. **How**: recruit via NGOs through multiple channels; test *with* disabled users (never simulate); ask several people (congenital vs acquired). **Trade-off**: avoid consultation fatigue.

## Design

### 7 Universal Design principles [P]
**When**: proactively designing. **How**: Equitable use, Flexibility, Simple & intuitive, Perceptible info, Tolerance for error, Low physical effort, Size & space. **Trade-off**: prevents barriers; doesn't replace user testing.

### Shift Left design checklist [Appt]
**When**: design phase. **How**: contrast (4.5:1 / 3:1), text scaling at 2×–3×, portrait+landscape, group + annotate related elements, simple language + labeled inputs. **Trade-off**: cheapest place to fix issues.

### Channel × Disability matrix + 3-Lens checklist [P]
**When**: designing in-person/phone/online service. **How**: map each disability across channels; cover Service Design + Assistive Technology + Training & Culture. **Trade-off**: thorough but effortful; use personas as shortcuts.

## Build & Verify

### Name, Role, Value on every interactive element [Appt]
**When**: development, esp. custom components. **How**: expose Name (identity), Role (button/tab), Value (state/property/value). **Trade-off**: native components give it free; custom ones need explicit work.

### Keyboard-first + gesture alternatives [Appt][P]
**When**: any interaction. **How**: full keyboard operability, no traps, single-pointer alternative for every gesture/drag/motion, targets ≥24×24 px, activate on release. **Trade-off**: forces simpler interaction models (usually a win).

### Always-on form defaults [P][Appt]
**When**: any form. **How**: no time limits (or adjustable), save-and-resume, autofill/no redundant entry, labels + format hints, errors in text with fix suggestions, undo/confirm for legal/financial. **Trade-off**: small dev cost, large cognitive-load reduction.

### 80/20 manual testing [Appt]
**When**: quick accessibility check. **How**: screen-reader pass (alt text, layout, operability, no traps, order, NRV) + external keyboard + contrast + 200% text + color-independence. **Trade-off**: finds ~80%; bring an expert for full eval.

### Dynamic, non-sticky interface [Appt]
**When**: development. **How**: no fixed width/height (grow with scaling/rotation); avoid sticky top/bottom bars. **Trade-off**: more layout effort; survives scaling and landscape.

### "Press 0" / live-agent escape hatch [P]
**When**: phone/IVR. **How**: always offer a live agent; answer TTY/VRS with equal standards. **Trade-off**: trivial to add, removes a major barrier.
