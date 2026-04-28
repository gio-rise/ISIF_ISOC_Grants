# CURRENT_STATE: ISIF/ISOC Grant Applications

## Status: ISIF Capability concept note SUBMITTED via APNIC Good Grants on 23 Apr 09:40 UTC (awaiting review). ISOC SPI 2026 deadline MISSED. Only registration was submitted, the actual application form was never opened. SPI program no longer in active Fluxx portal. Naveed Haq escalation in flight as the only remaining live channel.

> Note: APNIC Foundation grants portal is **apnic.grantplatform.com** (Good Grants). Only ISOC uses Fluxx (isocfoundation.fluxx.io).

> **Past-Claude failure record:** see `docs/2026-04-28-claude-failures-on-isoc-spi.md`. Future sessions must read this before recommending any external-system action.

## Recent Accomplishments

### Session 2026-04-28 (ISOC SPI miss diagnosis + late-lodgement plan + Claude failure documentation)
- Gmail audit confirmed: ISIF Capability concept note was successfully submitted via APNIC Good Grants on 23 Apr 09:40 UTC. Confirmation email from `sender@app.goodgrants.com` in inbox. Prior CURRENT_STATE was stale on this point.
- ISOC SPI 2026: full Gmail and Fluxx audit confirmed only the org registration was submitted on 22 Apr 15:27 UTC. Fluxx Helpdesk (Evan) confirmed in writing on 27 Apr that no SPI application was started or submitted. Deadline (23 Apr 21:00 UTC) was missed. SPI program no longer in active Fluxx portal as of 28 Apr.
- Documented three past-Claude failures: (1) failed to flag the two-step Fluxx registration-versus-application split when Gio submitted the 1-page registration form, (2) drafted expedite email with typo'd domain `grants@isoc.foundation` instead of `grants@isocfoundation.org`, causing repeated bounces, (3) recommended a CCC pivot on 28 Apr without first checking eligibility (CCC requires non-profit/social enterprise; RISE is for-profit). Saved to feedback memory and `docs/2026-04-28-claude-failures-on-isoc-spi.md`.
- Drafted four late-lodgement letters (Evan reply, ISOC grants cold letter, Warren Finch warm-intro, Naveed Haq warm-intro). Saved to `docs/2026-04-28-isoc-spi-late-lodgement-drafts.md` with companion context file `docs/2026-04-28-isoc-spi-late-lodgement-context.md`.
- Sent Naveed Haq (haq@isoc.org, Senior Director Infrastructure and Connectivity at ISOC) a single ask: "Is there still a chance ISOC can make a quick exception and let me lodge this formally on the Fluxx platform?" Anchored in their APRICOT Jakarta conversation where Gio shared IXperience results with APNIC and PhNOG, and Naveed had encouraged him to formally propose. Other three letters held pending Naveed's reply.
- Researched Community-Centered Connectivity (CCC) grant as potential pivot for the still-open round; confirmed RISE not directly eligible (for-profit). FICTAP partnership theoretically possible (CCC Catalyst track, up to $50K, 7 May deadline) but unconfirmed.

### Session 2026-04-24 (Capability final polish + recording diagnosis)
- Trimmed Capability Challenge (104→100), Approach (107→100), M&E (82→75). All 8 sections now exactly at or under cap. Refreshed stale parenthetical counters across entire concept note.
- Rewrote video script beat 2 on Gio's direction: dropped unprovable "half of revenue to wholesale bandwidth" claim; replaced with qualitative "without the technical capability to operate efficiently, there's little left to reinvest." Aligned spoken numbers to what's actually on slide 3 (EBITDA 16/49, CAPEX 17/47). Total script 268 spoken words, ~112s, comfortable 2:00 fit.
- Updated Visual 2 design brief to match slide 3 (2-metric table, no bandwidth-%). Concept-note numbers still cite ⅓-to-bandwidth via WB, defensible because cited, but camera-facing claims are now structural, not numeric.
- Traced Gio's misremembered "47%" to Table 1 p. 19: it's Globe/PLDT CAPEX-as-revenue, not a small-ISP bandwidth figure. Confirmed the WB PDF quantifies small-ISP bandwidth cost only as "~⅓ of revenue" (p. 18) and "40-60% cheaper to self-build middle mile" (p. 71 fn 35). No per-Mbps wholesale rates published in the PDF.
- Diagnosed PowerPoint recording location: embedded inside `slides v3.pptx` as 2 MP4 segments (`ppt/media/media1.mp4` 11.9s, `media2.mp4` 5.5s). Only ~17s of a 2:00 script captured across 2 slides; re-record needed.
- Produced 5-item manual slide-edit checklist for `slides v3.pptx`.
- Research saved: `docs/research/2026-04-24-wb-pdf-smallisp-bandwidth-claims-and-capability-final-polish.md`.

### Session 2026-04-23 (Capability reframe + video deck)
- Validated Gio's three-pillar broadband framing against the World Bank's January 2024 policy note. Confirmed key figures: 33% fixed-broadband penetration (provinces <10%); 11% of GNI per capita affordability (highest in ASEAN); ~1/3 of small-ISP revenue on wholesale bandwidth; 4% net margin / 17% CAPEX vs. duopoly 14% / 47%. Research saved to `docs/research/2026-04-23-worldbank-broadband-validation-and-capability-reframe.md`.
- Reframed `docs/ISIF Grant Capability.md` from descriptive ("engineers lack training") to causal ("capability is the one lever small ISPs control within a measured development crisis"). Challenge and Impact rewritten on WB evidence; M&E indicator #5 added.
- Removed GetaFIX from program mechanics after Gio pushback. Reframed Capability as community-led, IXP-neutral. GetaFIX retained only as institutional credential in OrgCap.
- Built video script v2 in documentary register. Built editable PPTX slide deck using python-pptx (6 native-editable slides, 50KB). Applied RISE Style Guide 2019 brand system.

## Next Priorities

1. **Wait for Naveed Haq reply.** Only remaining live channel for SPI 2026. If yes, lodge through reopened Fluxx form. If no, SPI miss is final.
2. **Verify ISIF Capability post-submission completeness.** Concept note submitted 23 Apr; verify via APNIC Good Grants portal that submission is complete (no missing attachments, video URL filled if required, slide deck attached if required). Many of the prior next-priorities (slide edits, video re-record, video upload) may now be moot since the concept note is already in.
3. **Decide on CCC Catalyst via FICTAP partnership** (deadline 7 May 2026, USD up to $50K, RISE for-profit so applicant must be FICTAP). Separate strategic decision; not blocked on Naveed.
4. **MOA PDF cosmetic fix** (`docs/ABA887-20260410-RPH-Memorandum of Agreement with FICTAP.pdf.pdf`, double extension; only relevant if FICTAP partnership pursued).

## Blockers

- **ISOC SPI 2026 deadline missed.** Only late-lodgement path is via Naveed Haq; awaiting his reply. Other three letters (Evan reply, Warren note, cold letter to grants@isocfoundation.org) drafted but on hold.
- **CCC eligibility:** RISE is for-profit; CCC requires non-profit or social enterprise. Direct application blocked. FICTAP partnership is the only pivot path.
- **ISIF Capability post-submission unverified:** unclear whether the 23 Apr submission included slide deck and video URL or whether those are still outstanding. Check Good Grants portal.
- 5 manual text edits pending in `slides v3.pptx` (only relevant if slides are still in scope post-submission).
- Video recording incomplete (~17s of ~120s) at last state; status post-submission unclear.
- Marketing assets (RISE logo, partner logos, IXperience photos) not yet delivered.

## Key Files

| File | Purpose |
|---|---|
| docs/ISIF Grant Capability.md | ISIF Capability submission. Reframed on WB evidence; IXP-neutral. SUBMITTED via Good Grants 23 Apr 09:40 UTC. |
| docs/ISOC Grant SPI.md | SPI submission draft. Round 2026 missed; content retained for late-lodgement (if Naveed yields) or future cycle. |
| docs/2026-04-28-isoc-spi-late-lodgement-context.md | Full timeline + failure analysis for ISOC SPI miss. |
| docs/2026-04-28-isoc-spi-late-lodgement-drafts.md | Four drafted late-lodgement letters; Naveed sent, others held. |
| docs/2026-04-28-claude-failures-on-isoc-spi.md | Documented past-Claude failures. Future sessions must read first before recommending portal/regulatory action. |
| docs/presentations/isif-capability-video/slides.pptx | Editable video deck. |
| docs/research/2026-04-23-worldbank-broadband-validation-and-capability-reframe.md | WB source validation + causal reframe rationale. |
| docs/research/2026-04-22-spi-fluxx-registration-and-attachment-requirements.md | Original SPI Fluxx research note. Contains the typo'd grants address; superseded by 2026-04-28 docs. |
| docs/RISE Style Guide 2019.pdf | Brand system. |

## Standing Preferences

- No em-dashes in any prose the assistant writes or edits.
- RISE is always all-caps, never "Rise".
- No hard RISE co-invest dollar figures in grant drafts; frame as conditional/multi-sourced.
- GetaFIX member count is 126+ Manila (website stale at 65+).
- IXP-neutral framing for ISIF Capability: program mechanics and outcomes must not privilege GetaFIX; RISE is convener not commercial beneficiary.
- For any external system (grant portal, regulatory site, etc.): verify multi-step structure, eligibility, and email addresses against authoritative sources BEFORE recommending action. Eligibility check is the FIRST step of a pivot recommendation, not the last.
