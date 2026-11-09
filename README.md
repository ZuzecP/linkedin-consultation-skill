# linkedin-consultation-skill

Reviews a LinkedIn profile and optimises it, mainly for job seekers, based on a specific named
methodology. Packaged as a Claude skill. It assesses the profile the way a recruiter first sees
it, prioritises what to fix, and drafts section copy grounded in evidence you provide rather
than invented for you.

## Methodology / authorship

Built on the LinkedIn consultation methodology of Zuzana Pešková, Head of People & Culture and
Sr. People Business Partner with 12+ years in SaaS and tech, and a practitioner who has reviewed
thousands of CVs and LinkedIn profiles.

The figures and rules of thumb in this skill are her practitioner observations, not published
research, and the skill states them as such.

## Installing

The repository is a Claude plugin containing one skill. Pick the route for where you use Claude.

**Claude Code, as a plugin marketplace.** This repository is its own plugin marketplace. It is not
listed in Anthropic's plugin directory.

```bash
claude plugin marketplace add ZuzecP/linkedin-consultation-skill
claude plugin install linkedin-consultation@linkedin-consultation-skill
```

**Claude Code, as a personal skill:**

```bash
ln -s "$PWD/skills/linkedin-consultation" ~/.claude/skills/linkedin-consultation
```

Run it from inside a clone of this repository. Claude Code follows the symlink and picks up
edits without a restart.

**Cowork and the Claude desktop app:** under **Customize > Plugins**, add this GitHub repository as a
marketplace, or zip the repository and use **Add > Upload plugin**.

**claude.ai:** zip the `skills/linkedin-consultation` folder, so that `linkedin-consultation/` is the
top level of the archive, and upload it under **Customize > Skills**.

## Using it

It triggers on phrases like "review my LinkedIn," "help me improve my profile," "rewrite my
headline," or "audit my LinkedIn," and when you share a profile screenshot, PDF export or text
and ask what to do with it. You can also invoke it directly with `/linkedin-consultation`.

It will ask how you want to work: quick wins first, or a full top-to-bottom review. Then it
needs your profile, by whichever of these is available:

1. **Reading it live in your browser**, if a browser signed in to LinkedIn as you is available:
   Claude for Chrome, or the browser built into the Claude desktop app. It asks before opening
   anything, reads only your own profile, and never clicks a control that changes state.
   LinkedIn's terms restrict automated access to the site; reading only your own profile in your
   own signed-in browser is a narrow use, but it isn't a risk-free reading of those terms, and
   the skill says so before it opens anything.
2. **LinkedIn's own More → Save to PDF export**, plus one screenshot of the top of your profile.
   The fallback if the browser isn't signed in, you'd rather not grant access, or none is
   available. Nearly as good, and it sidesteps the terms question entirely.
3. **A full-page screenshot**, via GoFullPage or similar.
4. **Pasted text**, with the skill stating what it can't assess from that alone.

It never edits your profile. You make every change yourself, by pasting copy you've approved.

## What's in the repo

- `skills/linkedin-consultation/SKILL.md` — the skill Claude loads and follows
- `skills/linkedin-consultation/references/` — the methodology in detail, loaded per section as
  the consultation reaches it
- `.claude-plugin/` — plugin and marketplace manifests
- `CHANGELOG.md` — version history
- `CONTRIBUTING.md` — how to propose changes
- `LICENSE` — CC BY-NC 4.0

## Scope

The skill covers the profile itself: URL, photo, cover, headline, About, Featured, experience,
skills, recommendations, and Open to work settings. It does not cover content creation, posting
strategy, or algorithm optimisation. It reads your profile but never edits it. It does not
fabricate facts, metrics or achievements, and it will decline if asked to.

For complex career pivots or positioning questions, it recommends
[booking a session with Zuzana directly](https://calendar.app.google/cteEUoLRwGwuPfWH7).

## License / usage terms

Licensed under [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/): free to share
and adapt with attribution to Zuzana Pešková, not for commercial use. See `LICENSE` for full
terms. Contributions are welcome, see `CONTRIBUTING.md`.
