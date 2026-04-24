# BACKLOG

## Active

### ISIF Capability submission (blocks 2026-04-24 10:00 GMT+10)

- **Apply 5 manual text edits to `slides v3.pptx`.** Why: Python `build_slides.py` no longer matches the hand-edited 12-slide v3 deck; edits have to happen in PowerPoint/Keynote directly. Edits: S2 "a Internet"→"an Internet"; S3 "expansions"→"expansion"; S3 "EBITDAs"→"EBITDA margin"; S4 widen box or shorten to "Reinvestment capacity restored"; S5 "IXPerience Pro"→"IXperience Pro" (match cover).
- **Re-record 2-minute video using corrected `slides v3.pptx`.** Why: current recording captured only ~17s across 2 slides (verified: `media1.mp4` 11.9s + `media2.mp4` 5.5s inside the PPTX). Script v2 in Capability.md is the source to read from.
- **Export recorded PPTX to MP4 via File → Export → Create a Video.** Why: PowerPoint "Record Slide Show" embeds audio/video in the PPTX but does not produce a standalone video file; explicit export step is needed.
- **Upload exported MP4 to YouTube unlisted, paste URL into Concept Note tab.** Why: Concept Note optional attachment.
- **Fix Application Title in ISIF portal: `RISE - IXperience Pro - 2026`.** Why: portal instruction requires "Org name - Title - YYYY" format; current entry omits the "RISE -" prefix.
- **Upload Legal Registration PDF (Certificate of Incorporation) to Organisation tab (ISIF portal).** Why: mandatory Phase 1 attachment. Staged at `docs/AAA001-20150622-RPH-Certificate of Incorporation.pdf`.
- **Upload List of Officers PDF (GIS 2026) to Organisation tab (ISIF portal).** Why: mandatory Phase 1 attachment. Staged at `docs/ABA442-20260313-RPH-General Information Sheet (GIS) 2026 - RISE.pdf`.
- **Rename MOA PDF to fix double `.pdf.pdf` extension before SPI upload.** Why: cosmetic — current file is `docs/ABA887-20260410-RPH-Memorandum of Agreement with FICTAP.pdf.pdf`.
- **Marketing ask: RISE signature logo PNG, 3-5 IXperience workshop photos (participants in learning mode + audience shot + speaker at podium), APNIC Academy + PhNOG + FICTAP logos (PNG/SVG), optional Project School Internet photo, written consent confirmation for participant photos.** Why: swaps into photo placeholders in slides 4 and 5; upgrades slide 6 partner row and bottom-left RISE mark from text to logo.

### ISOC SPI submission (blocks 2026-04-23 21:00 UTC)

- **Fill combined Budget/Workplan/Equipment Request template inside Fluxx after login.** Why: ISOC serves a single combined template inside the portal, not three separate files; Equipment Request section expected N/A for workshops program. Requires Fluxx approval first.
- **Stage clean PDF of RISE-FICTAP MOA for SPI upload.** Why: required community-interest attachment; don't scramble at submission time.
- **Escalation insurance: if Fluxx approval not received by 2026-04-23 noon UTC, follow up again with grants@isoc.foundation.** Why: application deadline is 21:00 UTC same day; need buffer to complete the Fluxx form once in.

### Letters of support

- **Optional: chase FICTAP letter of support for ISIF Capability.** Why: no longer required for SPI (MOA satisfies community-interest requirement); would marginally strengthen ISIF Capability only. Request drafted at `docs/letter-request-FICTAP.md`.
- **Chase PCTA letter of support.** Why: PCTA's endorsement corroborates the cable-TV-to-fiber cohort narrative now in both grants. Request drafted at `docs/letter-request-PCTA.md`.

### Trainer pipeline (independent of grant decisions)

- **Send APNIC Academy fellowship ask for Filipino trainer development.** Why: ensures pipeline exists even if ISIF Capability is not awarded; low friction, existing relationship from IXperience 2025.
- **Send NSRC instructor-matching request.** Why: second independent path; NSRC has long-running APNIC/PhNOG ties and deploys instructors to LMICs at no cost.

### SPI delivery readiness

- **Per-leg sponsor outreach: Globe, PLDT, Converge, GreenIX, DE-CIX.** Why: SPI budget closes at lean with $500/leg gap; sponsor funding closes gap and unlocks premium uplift for Clark and CDO.
- **Confirm Cebu leg co-location with PhNOG Conference 2026 and secure PhNOG budget absorption of direct event costs.** Why: SPI budget assumes this absorption; verbal commitment exists but needs written confirmation.

### Data and rigor (medium-term)

- **Clean the rise-ecosystem MCP data so it can be cited in future grants.** Why: current dataset is usable internally but not yet certified to precision reviewers would demand.
- **Document PDSCN resale rights (contractual).** Why: not required for these submissions but will be asked at full-proposal stage for any future Infrastructure or wholesale grant.

## Done (recent)

- **2026-04-24 — Capability Challenge trimmed 104→100 words.**
- **2026-04-24 — Capability Approach trimmed 107→100 words.**
- **2026-04-24 — Capability M&E trimmed 82→75 words.**
- **2026-04-24 — Video script beat 2 rewritten: dropped unprovable "half to wholesale bandwidth" claim; aligned spoken numbers to slide 3 (EBITDA 16/49, CAPEX 17/47); pivoted on capability-driven inefficiency framing.**
- **2026-04-24 — Visual 2 design brief updated to match the 2-metric slide Gio actually built.**
- **2026-04-24 — WB PDF small-ISP bandwidth claims re-traced. Confirmed 47% = Globe/PLDT CAPEX (not small-ISP bandwidth); only ⅓-to-bandwidth (p. 18) and 40-60% self-build savings (p. 71 fn 35) are WB-quantified small-ISP figures.**
- **2026-04-24 — PowerPoint recording location diagnosed: embedded inside `slides v3.pptx` as per-slide MP4 segments; only ~17s captured of 2:00 script; re-record needed.**
- **2026-04-23 — WB broadband three-pillar framing validated against World Bank Jan 2024 policy note; key figures cited verbatim in Capability Challenge and Impact.**
- **2026-04-23 — Capability reframed causal: training → peering/routing → lower bandwidth spend → reinvestment capacity → WB access/affordability/quality indicators. Challenge and Impact rewritten; M&E indicator #5 added.**
- **2026-04-23 — GetaFIX removed from Capability program mechanics (Intro, Approach, video beat 5, Visual 5, production notes). GetaFIX retained only in OrgCap as institutional credential. IXP-neutrality explicit.**
- **2026-04-23 — Factual error corrected: training runs on APNIC Academy labs and courseware, not a live production IXP.**
- **2026-04-23 — Video script v2 written (documentary register). Rejected mission-first opener and the Beat 2 rewrite that dropped WB Table 1 data; merged cable-TV context; added 2023 ISIF grant credibility; closed WB-indicator loop.**
- **2026-04-23 — Editable PPTX deck built with python-pptx (6 slides, 50KB). Replaced MARP-rendered PPTX which was rasterized. RISE Style Guide 2019 brand applied.**
- **2026-04-23 — Integrated operational program model (SPI + ISIF as IXperience Philippines 2026) saved as project memory.**
- **2026-04-22 (late, ISOC) — ISOC Fluxx organization registration submitted; awaiting approval (1-2 business day SLA). Expedite email sent to grants@isoc.foundation.**
- **2026-04-22 (late, ISOC) — SPI Fluxx "Project Summary" (528/550 chars) and "Organization Mission" fields filled and submitted.**
- **2026-04-22 (late, ISOC) — Hard USD 25,000 RISE co-invest commitments removed from SPI draft Sections 1, 5, 7; now framed as conditional/multi-sourced. Feedback memory saved.**
- **2026-04-22 (late, ISOC) — ISOC SPI attachment requirements verified via WebFetch: combined Budget/Workplan/Equipment Request template + 1 community-interest doc. For-profit eligibility on PES track confirmed.**
- **2026-04-22 (late, ISOC) — SPI community-interest blocker resolved: existing RISE-FICTAP MOA satisfies the requirement.**
- **2026-04-22 (late) — APNIC Foundation portal confirmed as apnic.grantplatform.com (Good Grants), not Fluxx. Gio registered and logged in.**
- **2026-04-22 (late) — ISIF Capability draft trimmed to form word caps; portal-selections table and Target Beneficiaries block added.**
- **2026-04-22 (late) — Org Capability rewritten with verified GetaFIX metrics (126+ / 1,952 / 11 DCs / 1 Tbps) and 2024 USTDA award; unverified USD 150K/130K figures dropped.**
- **2026-04-22 (late) — Organisation tab filled in ISIF portal; preview reviewed clean.**
- **2026-04-22 (late) — Rise → RISE swept across Capability draft; all-caps rule saved to memory.**
- **2026-04-22 (late) — RISE legal entity (Responsible Internet Sustainability Effort, Inc.) and registered address saved to reference memory.**
- **2026-04-22 — SPI Section 2 rewritten with cable-TV cohort narrative; numbers hedged; single-homed detour dropped.**
- **2026-04-22 — SPI budget rebuilt against marketing's per-city 3-day cost model with layered funding.**
- **2026-04-22 — SPI delivery decoupled from ISIF Capability outcome.**
- **2026-04-22 — Capability Section 3 (Challenge) updated with cable-TV cohort angle, within 100-word cap.**
- **2026-04-22 — "First in PH, second in SEA after MMIX" verified and added to SPI summary.**
- **2026-04-22 — ISIF Infrastructure formally dropped from scope.**
- **2026-04-22 — Em-dash aversion saved as permanent feedback memory and swept from working files.**
