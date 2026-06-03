# accessiblity-playbook
Multi-book accessibility knowledge base as a Claude Code / Amp skill — distills the AccessAbility Playbook, Giving a Damn About Accessibility, and the Appt Handbook into on-demand frameworks for service, design, and WCAG/mobile.

## What this skill does

It gives Claude Code (or Amp) a **curated, source-tagged accessibility reference** that loads only when you need it. Instead of relying on the model's generic, sometimes-outdated accessibility knowledge, it pulls answers from three vetted books — each covering a different layer of the problem:

- **Service & organization [P]** — *AccessAbility Playbook* (Gov. of Canada): how to deliver accessible client service in person, by phone, and online; barrier audits, personas, culture change.
- **Mindset & advocacy [GD]** — *Giving a Damn About Accessibility* (Sheri Byrne-Haber): how to win the argument internally, counter resistance, avoid overlay snake-oil, and go from compliant to genuinely great.
- **Build & WCAG [Appt]** — *Appt Accessibility Handbook*: WCAG 2.2 (POUR) criteria at A/AA, mobile-app specifics, contrast/target-size/keyboard rules, and a shift-left testing approach.

The skill ships a `SKILL.md` index plus per-chapter files, a glossary, reusable patterns, and a cheatsheet — so Claude reads the *relevant* chapter on demand rather than guessing.

## What you can use it for

- **During code review or design** — "is this contrast ratio compliant?", "what's the minimum touch-target size?", "does this custom component have proper Name/Role/Value?"
- **Writing UI copy & forms** — plain-language checks, accessible error messages, time-limit and save-and-resume patterns.
- **Making the case for accessibility** — turn "only a few users need this" or "where's the ROI?" into a grounded counter-argument (the 6 resistance archetypes, the substitution test).
- **Auditing a service or product** — the 5 Barrier Areas, the Channel × Disability matrix, the maturity/shift-left model.
- **Looking up a specific WCAG criterion or chapter** — pass a topic, a criterion, a book, or a chapter id like `appt-ch03` and get a scoped answer.

## Why use it instead of asking the model directly

- **Grounded, not hallucinated** — answers come from named sources with chapter citations, so you can verify and quote them.
- **Always the right altitude** — it spans the *whole* problem (people → process → design → code), not just WCAG line-items, so you don't miss the organizational or advocacy side.
- **On-demand, low-noise** — it stays out of the way until an accessibility question comes up, then loads only the chapter that matters.
- **Multi-perspective** — three authors with different lenses (government service, advocate, mobile/WCAG engineer) cross-check each other, with a "WCAG is a floor, not a ceiling" stance baked in.
- **Practical defaults** — opinionated, ship-it guidance ("press 0", no time limits, errors in text + fix suggestion, test *with* disabled users) rather than abstract principles.

> Honest scope: the WCAG summaries are condensed paraphrases (A/AA only) — for normative text consult the W3C spec, and always pair this with a real screen-reader pass for hands-on work. See [Scope & Limits in `SKILL.md`](SKILL.md).

## Install as a Claude Code skill

The skill lives in `SKILL.md` (with supporting content in `chapters/`, `glossary.md`, `patterns.md`, and `cheatsheet.md`). To use it in Claude Code, copy this repo into a skills directory under the skill's name (`accessability-playbook`).

### Personal skill (available in every project)

```bash
git clone https://github.com/<your-org>/accessiblity-playbook.git \
  ~/.claude/skills/accessability-playbook
```

Or, if you already have the repo checked out:

```bash
mkdir -p ~/.claude/skills
cp -R /path/to/accessiblity-playbook ~/.claude/skills/accessability-playbook
```

### Project skill (shared with a single repo)

```bash
mkdir -p .claude/skills
cp -R /path/to/accessiblity-playbook .claude/skills/accessability-playbook
```

Commit `.claude/skills/accessability-playbook/` so teammates get it automatically.

### Verify and use

1. Restart Claude Code (or run `/doctor`) so it picks up the new skill.
2. Run `/skills` (or ask "what skills do you have?") and confirm `accessability-playbook` is listed.
3. Invoke it by asking an accessibility question, or pass a topic/chapter directly, e.g. `appt-ch03`, a WCAG criterion, or a framework name.

> The directory name must match the `name:` field in `SKILL.md` (`accessability-playbook`). Claude Code loads any folder containing a `SKILL.md` from `~/.claude/skills/` (personal) or `.claude/skills/` (project).

## Contributing

**This is a collaborative project — PRs are more than welcome!** 🙌

The goal is a living, multi-source accessibility knowledge base. If you know a great resource — a book, handbook, standard, guideline, research paper, or practical pattern — please open a PR to integrate it. When adding a new source, credit the original author(s) and cite the work's license (see below), and only include material whose license permits redistribution.

See [CONTRIBUTING.md](CONTRIBUTING.md) for the full guide.

## License

This work is licensed under [**Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)**](https://creativecommons.org/licenses/by-sa/4.0/) — see [LICENSE](LICENSE).

CC BY-SA 4.0 is required here (rather than a more permissive license) to comply with the **ShareAlike** obligation of the Appt Accessibility Handbook, whose content is itself CC BY-SA 4.0. Any redistribution or adaptation of this knowledge base must therefore keep the same license and preserve attribution to all original sources listed below — including a visible link to <https://appt.org>.

> Note: *Giving a Damn About Accessibility* is **not** distributed under an open-content license. It is summarized here (not reproduced verbatim) with attribution; this repo's CC BY-SA 4.0 license covers the original distillation, **not** the underlying work. Please refer to the author's terms before reusing material derived from it.

## Credits & source licenses

This knowledge base distills and is built upon the work of others. All credit for the underlying material goes to the original authors and publishers. Their works are reused here in line with their respective licenses; please honor those terms (including attribution) in any further reuse.

- **AccessAbility Playbook** — by **ESDC, Centre of Expertise for Accessible Client Service (Government of Canada)**. Crown Copyright © His Majesty the King in Right of Canada; Government of Canada material is generally made available for reuse under the [Open Government Licence – Canada](https://open.canada.ca/en/open-government-licence-canada). Source: <https://ceacs-cesca.github.io/playbook/>.
- **Giving a Damn About Accessibility** — by **Sheri Byrne-Haber, CPACC**. © Sheri Byrne-Haber. Distributed free of charge by the author (PDF + audiobook); it does not carry an explicit open-content license, so please refer to the author's terms before redistributing. Source: <https://www.accessibility.uxdesign.cc/>.
- **Appt Accessibility Handbook** — by the **Appt Foundation**. Content licensed under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) and code under the [MIT license](https://opensource.org/licenses/MIT); attribution requires a visible link to <https://appt.org>. Source: <https://appt.org/en/handbook>.

> Note on licenses: where a source uses a ShareAlike or restrictive license, any redistribution (including this repo's derived summaries) must comply with the original terms. If you believe content here misattributes or misuses a source, please open an issue and it will be corrected promptly.
