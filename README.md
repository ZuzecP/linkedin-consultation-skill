# linkedin-consultation-skill

Reviews LinkedIn profile and optimises it (mainly) for job seekers, based
on a specific named methodology. Built for use as a Claude skill.

## Methodology / authorship

Built on the LinkedIn consultation methodology of Zuzana Pešková — Head of People & Culture and
Sr. People Business Partner with 12+ years in SaaS and tech, and a practitioner who has reviewed
thousands of CVs and LinkedIn profiles.

## How to use it

Upload the SKILL.md file in Claude.ai under Settings → Customize → Skills, and start using it.  It triggers
automatically whenever you ask Claude to review, assess, improve, rewrite, or give feedback on
a LinkedIn profile, on phrases like "review my LinkedIn," "help me improve my profile,"
"LinkedIn feedback," "rewrite my headline/about/experience," "audit my LinkedIn," or any mention
of LinkedIn profile work — including just uploading a LinkedIn screenshot and asking what to do
with it. 

## What's in the repo

- `SKILL.md` — the actual skill Claude loads and follows.
- `linkedin_guide.md` — the original source guide, kept for human reading. Not loaded separately
  at runtime; its content is embedded inline in `SKILL.md`.
- `CHANGELOG.md` — version history. See that file for the full history of changes.
- `LICENSE` — usage terms (CC BY-NC 4.0).
- `CONTRIBUTING.md` — how to propose changes via pull request.

## License / usage terms

Licensed under [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/) — free to share
and adapt with attribution to Zuzana Pešková, not for commercial use. See `LICENSE` for full
terms. Contributions are welcome — see `CONTRIBUTING.md`.
