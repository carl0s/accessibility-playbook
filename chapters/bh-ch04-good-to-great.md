# [Giving a Damn] Ch 4: Turning good accessibility into great accessibility

## Core Idea
Only ~2% of web pages do a good *or* great job at accessibility. Within that 2%, what separates good from great is a shift from **compliance to empathy** — going beyond the standard because you genuinely want an equal experience, not just a passing audit.

## Frameworks Introduced
- **The Good → Great Differentiators**:
  1. **Compliance → Empathy.** Don't stop at AA: follow AAA criteria that *should* be AA (touch target size); check contrast in colorblindness modes and for focus indicators/icons, not just text (beyond WCAG 1.4.3); make employee-facing tools as accessible as public ones; use "premium language."
  2. **Product → Entire experience.** Customers buy experiences, not products. Make adjacent services accessible too — docs, training, customer support, surveys (the "last car on the accessibility train"). Physical packaging counts (Xbox).
  3. **User research → Feedback from people with disabilities.** "Nothing about us, without us." Never assume impact — *ask*, respectfully, and ask several people (congenital vs acquired disability gives different perspectives). Use testers *with* disabilities; simulating disability is never sufficient.
  4. **Accessible design systems.** Build/adopt accessible component libraries ("software Legos") — one defect propagates to thousands of places. Accessible examples: Clarity (VMware), Lightning (Salesforce), Spectrum (Adobe), Carbon (IBM). Expose required ARIA properties; contribute fixes back upstream.
  5. **Accessibility as a release gate.** A go/no-go check with a visible exceptions process, so requesting a release without closing the gate exposes bad decisions to powerful stakeholders.
  6. **Speak at design events, not (only) accessibility events.** At accessibility conferences you preach to the choir; at UI/UX/design conferences you convince the non-believers — far higher impact.

## Key Concepts
- **Empathy-driven accessibility** — wanting to do it right vs merely complying.
- **Adjacent services** — docs/training/support/surveys; the last thing to get accessible, a good overall signal.
- **Design system as a multiplier** — one accessible (or inaccessible) component scales everywhere.
- **Release gate** — final go/no-go check that only accessible software ships.
- **Congenital vs acquired disability** — different lived perspectives; ask several people.

## Mental Models
- **"Good is compliance, great is empathy."**
- **"The difference between good and great is a chasm the size of the Grand Canyon."** (Rob Light)
- **Customers buy experiences, not products** — accessibility extends to everything adjacent.
- **"Nothing about us, without us"** — testers with disabilities, never simulation.
- **One design-system defect = thousands of broken places.**

## Anti-patterns
- **Stopping the moment AA is met.**
- **Checking contrast only for text** in unimpaired vision mode.
- **Simulating disability** instead of testing with disabled users.
- **Public site accessible, employee tools ignored.**
- **Building a design system without accessible components / exposed ARIA.**

## Key Takeaways
1. Go beyond compliance: AAA where it matters, colorblind/focus contrast, adjacent services.
2. Make accessibility a release gate with a visible exceptions process.
3. Test with people with disabilities — ask several, never simulate.
4. Use/contribute to accessible design systems; one defect scales.
5. Evangelize at design events to reach non-believers; great accessibility is "priceless" to AT users.

## Connects To
- **bh-ch02**: great accessibility is the far end of the first-attempt spectrum.
- **[Playbook] esdc-ch04**: Universal Design as the "great" design discipline.
- **[Appt] appt-ch07**: design systems, release gates, and testing-with-users in app practice.
