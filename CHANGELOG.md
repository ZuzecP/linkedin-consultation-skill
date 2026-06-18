# Changelog — linkedin-consultation skill

---

## v2.2 — 2026-06-18

### Changed
- Byline corrected: "Zuzka Pešková — Senior People Business Partner" → "Zuzana Pešková — Head
  of People & Culture and Sr. People Business Partner" (intro section).
- AI Sourcing Tip callout marked inline as "(2026, illustrative — not a sourced statistic)."
  No source was found for the specific "average" / "Expert-Level" classification claim during
  review; left as-is per decision, now explicitly labelled as illustrative rather than factual.
- "What this tool does not do": booking recommendation now links directly to Zuzana's booking
  page (https://calendar.app.google/cteEUoLRwGwuPfWH7). Byline in this line also corrected to
  Zuzana Pešková.

### Reverted
- Skills algorithm claim reverted to "top 3" (was briefly changed to "top 5" earlier in this
  version, then reversed at the user's request along with the associated note about it
  overlapping with the "Top Skills — 5 visible before the fold" claim). No net change to this
  section from v2.1.

### Added
- Reference to the full LinkedIn 1.0 guide and its Notion link, added directly under the intro
  (in addition to the archived `references/linkedin_guide.md` file already in the package).
- New behavioural rule #9, "Question sequencing": questions must be asked one at a time in
  logical order, or batched by topic — never scattered. If the user moves on before answering
  all questions in a batch, the skill must flag which ones are still outstanding.
- Final checklist: added an alternative wrap-up option — uploading a fresh full-page screenshot
  of the updated profile for a before/after style summary against the original screenshot,
  offered alongside (not instead of) the checklist.

---

## v2.1 — 2026-06-18

### Added
- Non-job-seeker branch: new subsection "If the user's goal is not job search" after Step 1
  (opening flow). If it becomes clear the user isn't job hunting (networking, consulting,
  general credibility), the skill states its job-seeker design intent but offers to proceed
  anyway, since the principles apply broadly. No refusal, no redirect.
- Mid-consultation conflict handling: new subsection after Step 3. If evidence revealed later
  contradicts the chosen approach (quick wins vs. full review), the skill notes the conflict
  and offers a revision, without pushing. User decides whether to address it now or later.
- Decline-probing fallback (Experience section protocol): if the user declines the Socratic
  evidence-gathering exercise, the skill says it can polish the existing text, but flags that
  without specifics the result will be generic (phrasing only, no added impact/evidence). No
  fabrication to compensate.
- Copy language question (Drafting and copywriting rules): new step — before drafting any
  section, ask which language the profile copy should be written in, independent of the
  language used in the consultation itself.

### Changed
- Headline emoji guidance softened: "use keywords, symbols and emojis for better legibility"
  → "use keywords, and consider using symbols and emojis for better legibility." Removed the
  directive tone.
- Final checklist scope clarified: explicitly a chat recap, not a deliverable — no separate
  document generated for it.

### Not changed
- "AI Sourcing Tip" framing (headline and Featured sections) — left as-is per review decision;
  treated as illustrative heuristic, not a sourced statistic.

---

## v2.0 — 2026-05-20

### Major release
This version marks the completion of the inline integration of the reference guide into the
skill itself. The skill is now fully self-contained — no external files required at runtime.
All structural inconsistencies from the integration have been resolved (v1.7). The skill
has been through a full editorial and audit cycle and is considered stable for distribution.

See v1.6 and v1.7 for the detailed change log of the integration and fixes.

---

## v1.7 — 2026-05-20

### Fixed
- Heading level inconsistency: Section guidance for Headline, Cover picture, and Location
  promoted from `###` to `##` — now consistent with all other Section guidance headings.
- Removed duplicate "About written last" note from Experience section protocol — canonical
  location is Section guidance: About.
- Moved "500+ connections" Reality Check from Skills to Recommendations — network trust
  signals belong in that context. Added note to encourage ongoing network maintenance.
- Removed "From the guide:" labels in URL and Photo sections — redundant now that all
  content is inline. Converted trailing paragraphs to blockquote callout style for visual
  consistency with Reality Check callouts elsewhere.

### Not changed
- No fabrication rule appears in both Behavioural rules and Drafting and copywriting rules
  intentionally — different contexts, both correct.
- Top 3 vs top 5 skills: not a contradiction. Top 3 = algorithmic weight; Top 5 = visible
  before the fold to human visitors. Both correct and complementary.

---

## v1.6 — 2026-05-20

### Changed
- Guide content from `references/linkedin_guide.md` merged inline into SKILL.md. The
  reference file is retained in the package for archival purposes but is no longer loaded
  separately — all framework content is now embedded directly in the relevant sections.
- Removed instruction to load external reference file at session start.
- Added inline section guidance for: Headline, Cover picture, Location, About, Featured,
  Skills, Recommendations.
- Added Final checklist section directly into SKILL.md.
- Removed "Reference file" section at the bottom (no longer needed).

---

## v1.5 — 2026-05-20

### Changed
- URL assessment: removed abbreviated example `jana-novakova-pm` from the options list
  (consistent with no-abbreviation rule added in v1.4).
- URL assessment: kept `jana-novakova-product` (domain) in the list; removed and restored
  after review.

---

## v1.4 — 2026-05-20

### Changed
- URL assessment: added rule to never suggest abbreviated URLs (e.g. `john-doe-pm`) —
  abbreviations are not industry-agnostic. If seen in existing URL, flag and explain ambiguity.
  Always recommend full spelling of role or domain, or clean name-surname baseline.
- URL assessment: clean name-surname tier — removed "no pressure to change." Now instructs
  to acknowledge as correct, then explain the value of adding a keyword using context-specific
  reasoning. Convince, don't push.
- Photo assessment: added guidance to briefly explain the value of a strong, up-to-date photo
  when flagging issues or confirming a good one (first impression, mobile dominance,
  expectation-reality gap).

---

## v1.3 — 2026-05-20

### Changed
- Intro and opening flow: "tens of thousands" → "thousands" in both places.
- Behavioural rule #1: added emotional intelligence guidance — assessments should use
  probabilistic language ("there is a high chance," "this might") rather than absolute
  statements when flagging negative outcomes. Candour and humility are not mutually exclusive.

---

## v1.2 — 2026-05-19

### Changed
- URL assessment: calibrated push level now has three tiers — number string (must-fix),
  clean name-surname (desired baseline, no pressure), role/technology add-ons (nice-to-have).
- Photo assessment: removed recency check as a standalone rule; mood/artistic photos still
  flagged directly, but follow-up recommendation urgency is now explicitly calibrated to
  role, background, and industry context (must-fix for conservative industries, worth
  reconsidering for creative roles).

---

## v1.1 — 2026-05-19

### Added
- Opening intro now explicitly states the tool is designed for job seekers, not for
  marketing or sales purposes, and defines scope boundary (profile only — no content
  strategy, posting, or algorithm advice).
- URL assessment rules: no diacritics in suggested URLs; always offer multiple options
  with role-adapted examples; calibrated push level (number string = must-fix,
  clean name-surname = nice-to-have).
- Photo assessment rules: corporate-relaxed headshot as benchmark; mood/artistic photos
  flagged directly; role and industry context required before assessing; recency check;
  fallback to request closer screenshot if full-page image is too small to judge.

---

## v1.0 — 2026-05-19

### Initial release
- Full consultation workflow: approach selection, full-page screenshot input, first-pass
  assessment, quick wins path (A) and full review path (B).
- Seven behavioural rules: no validation of bad work, ask before advising, verdict first,
  no fabrication, direct tone, Socratic approach, digestible doses.
- Experience section protocol: evidence-first, no drafting until impact metrics are solid.
- Copywriting rules: audience-first, section-by-section, no fabrication, confirm before
  finalising.
- GoFullPage / Full Page Screen Capture guidance for input.
- Scope boundaries documented.
- Reference file: `references/linkedin_guide.md` (Zuzka Pešková's full framework,
  converted from PDF).
