# accessiblity-playbook
Multi-book accessibility knowledge base as a Claude Code / Amp skill — distills the AccessAbility Playbook, Giving a Damn About Accessibility, and the Appt Handbook into on-demand frameworks for service, design, and WCAG/mobile.

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
