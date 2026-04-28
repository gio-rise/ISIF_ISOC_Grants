# 2026-04-28: Claude failures on ISOC SPI 2026

This file documents specific failures by Claude (in past sessions) that cost Gio the on-time SPI 2026 submission. Saved at Gio's explicit request so future Claude sessions, which start with no memory of prior conversations, can find this and avoid repeating the pattern.

## What past Claude got wrong

1. **Failed to flag the two-step nature of Fluxx in plain English.** On 22 April 2026, Gio submitted a 1-page Fluxx form that contained an "SPI Project Summary" (550-char) field and an "Organization Mission" field. He noted to me that the form felt surprisingly short. Past me said "that's it, wait" rather than "this is just registration; a separate multi-page application form is still required before the 23 April deadline." The Fluxx auto-confirmation email said "Thank you for submitting your registration information" but did not flag a remaining step or surface the deadline, and past me did not catch this.

2. **Drafted the expedite email with a typo'd domain.** Past me wrote the expedite email to `grants@isoc.foundation`. The correct ISOC Foundation grants address is `grants@isocfoundation.org`. The email bounced repeatedly with Gmail delivery failures and never reached anyone at ISOC Foundation. Past me then recorded the typo'd address in the project files, perpetuating it.

3. **Recommended a program pivot without checking eligibility first.** On 28 April 2026, after discovering SPI was no longer in the Fluxx portal, past me recommended pivoting to the Community-Centered Connectivity (CCC) grant program because of substantive fit. Only after the recommendation did past me check the CCC eligibility criteria and discover that CCC requires non-profit or social enterprise applicants and RISE is for-profit, making the pivot inapplicable.

## Direct cost to Gio

- Missed the 23 April 2026 SPI deadline (USD 25K grant cycle).
- Wasted hours on a recovery plan based on a false CCC pivot recommendation.
- Trust burn that has to be rebuilt over future sessions.

## Lesson for future Claude

When Gio is acting on a Claude recommendation through an unfamiliar grant portal, regulatory system, or external workflow:

1. **Verify the multi-step structure of the system before saying any step is complete.** Confirmation emails are not the same as application acceptance. Read what the system actually says, not what the wording implies.
2. **Verify all external email addresses by independent lookup before drafting outreach.** Domain typos like `isoc.foundation` vs `isocfoundation.org` are catastrophic in time-sensitive workflows.
3. **For any program-pivot recommendation, verify eligibility against authoritative sources first** (program page, eligibility section). Present the eligibility check before the pivot logic. Do not recommend a pivot and then check eligibility.
4. **When Gio's gut says "this seems too short, too easy, too quick," treat it as a system-check signal.** Walk through every remaining step explicitly in plain English. Do not say "that's it" until you have verified there is nothing else.
5. **Eligibility, deadline behavior, and required steps are all questions that take 5 minutes to verify.** A missed deadline is irrecoverable. The verification time is always cheap relative to the failure cost.

## Related companion files

- `docs/2026-04-28-isoc-spi-late-lodgement-context.md` — full timeline of what happened, what is on the email record, and the failure analysis.
- `docs/2026-04-28-isoc-spi-late-lodgement-drafts.md` — the late-lodgement letter drafts.
- `.claude/snapshots/2026-04-22-235843_isoc-spi-fluxx-registration-and-draft-softening.md` — the original snapshot. Contains the typo'd address.
- `docs/research/2026-04-22-spi-fluxx-registration-and-attachment-requirements.md` — the original research note. Also contains the typo'd address.

## Memory mirror

A complementary feedback memory has been saved at `~/.claude/projects/-Users-giobacareza-Developer-Work-ISIF-ISOC-Grants/memory/feedback_verify_external_systems.md`, indexed in `MEMORY.md` for the same project. Both should be considered current and authoritative.
