# CURRENT_STATE: ISIF/ISOC Grant Applications

## Status: ISIF Capability concept reframed on World Bank evidence; video deck and script ready. ISOC SPI Fluxx registration submitted (awaiting approval). Three Capability sections over word cap (18 words total).

> Note: APNIC Foundation grants portal is **apnic.grantplatform.com** (Good Grants), not Fluxx. Only ISOC uses Fluxx (isocfoundation.fluxx.io).

## Recent Accomplishments

### Session 2026-04-23 (Capability reframe + video deck)
- Validated Gio's three-pillar broadband framing against the World Bank's January 2024 policy note. Confirmed key figures: 33% fixed-broadband penetration (provinces <10%); 11% of GNI per capita affordability (highest in ASEAN); speeds below peer ASEAN (SG/TH/VN/MY); ~1/3 of small-ISP revenue on wholesale bandwidth; 4% net margin / 17% CAPEX vs. duopoly 14% / 47%. Research saved to `docs/research/2026-04-23-worldbank-broadband-validation-and-capability-reframe.md`.
- Reframed `docs/ISIF Grant Capability.md` from descriptive ("engineers lack training") to causal ("capability is the one lever small ISPs control within a measured development crisis"). Challenge and Impact rewritten on WB evidence; M&E indicator #5 added (wholesale bandwidth spend as share of revenue); Intro/Alignment/Approach/Target Beneficiaries/OrgCap lightly reworked.
- Removed GetaFIX from program mechanics after Gio pushback. Reframed Capability as community-led, IXP-neutral. GetaFIX retained only as institutional credential in OrgCap; production notes and Visual 5 mention GetaFIX only in negative form. Same ring-fencing SPI already has.
- Corrected factual error: training runs on APNIC Academy labs and courseware, not a "live production IXP." GetaFIX not a lab.
- Built video script v2 in documentary register (documentary not marketing). Rejected Gio's mission-first opener and his Beat 2 rewrite that dropped WB Table 1 data. Preserved evidence, added cable-TV context, added 2023 ISIF Project School Internet credibility signal, closed the WB-indicator loop at the end.
- Built editable PPTX slide deck using python-pptx (6 native-editable slides, 50KB). Replaced the MARP-rendered PPTX which was rasterized and uneditable. Applied RISE Style Guide 2019 brand system: BG Navy #104B84, RISE Pink #F04F6C, RISE Black #333232, Maison Neue with Calibri fallback. File: `docs/presentations/isif-capability-video/slides.pptx` with `build_slides.py` source.
- Saved integrated operational model as project memory: SPI + ISIF run as one program (IXperience Philippines 2026) with two funding-attributed layers, shared logistics, separate ledgers, two reports to two grantors.

### Session 2026-04-22 (late, ISOC): Fluxx registration + SPI draft softening
- Submitted RISE organization registration to ISOC Foundation Grants Portal; awaiting approval (1-2 business day SLA). Expedite email sent.
- Filled Fluxx "SPI Project Summary" (528/550 chars) and "Organization Mission" fields.
- Removed hard USD 25,000 RISE co-invest commitments from SPI draft Sections 1, 5, 7; reframed as conditional/multi-sourced.
- Verified SPI attachment requirements via WebFetch: combined Budget/Workplan/Equipment Request template + 1 community-interest doc. RISE-FICTAP MOA satisfies community-interest requirement.
- Research: `docs/research/2026-04-22-spi-fluxx-registration-and-attachment-requirements.md`.

### Session 2026-04-22 (late, ISIF): ISIF portal mapping + Capability rewrite
- Confirmed APNIC Foundation portal is Good Grants. ISIF 2026 has three categories: IPV6, Project Implementation, Research. Capability bid submitted under Project Implementation at $50K.
- Rewrote Capability to form spec: portal-selections metadata table, Target Beneficiaries 50-word bulleted block, Intro and Approach trimmed.
- Org Capability rewritten with verified figures: GetaFIX 126+ members, 1,952 networks, 11 DCs, 1 Tbps+; 2024 USTDA ~$1.27M award; team bios tightened.
- Gio completed Organisation tab in portal; preview clean.

## Next Priorities

1. **Trim Challenge (4), Approach (7), and M&E (7) to word cap before submission.** 18 words total. Audit revealed overages missed in prior drafting.
2. **Submit ISIF Capability by 2026-04-24 10:00 GMT+10.** Remaining blockers unchanged: Application Title fix to `RISE - IXperience Pro - 2026`; Legal Registration PDF upload; List of Officers PDF upload.
3. **Record video using `slides.pptx`** as presentation background with webcam overlay. Upload to YouTube unlisted. Paste URL into Concept Note tab.
4. **Marketing ask:** RISE signature logo PNG, 3-5 IXperience workshop photos, APNIC Academy + PhNOG + FICTAP logos. Optional Project School Internet photo.
5. **Submit SPI by 2026-04-23 21:00 UTC.** Wait for Fluxx approval, map `docs/ISOC Grant SPI.md` into Fluxx, complete Budget/Workplan template, attach MOA PDF.
6. **Stage a clean PDF of the RISE-FICTAP MOA** for SPI upload.

## Blockers

- Word-count overages in Capability: Challenge 104/100, Approach 107/100, M&E 82/75. Must trim before submission.
- Legal Registration PDF + List of Officers PDF not yet uploaded to ISIF portal.
- Application Title needs "RISE -" prefix correction in ISIF portal.
- ISOC Fluxx registration awaiting approval (expedite email sent).
- Clean RISE-FICTAP MOA PDF not yet staged for SPI upload.
- Marketing assets (RISE logo, partner logos, IXperience photos) not yet delivered for video production.

## Key Files

| File | Purpose |
|---|---|
| docs/ISIF Grant Capability.md | ISIF Capability submission. **Reframed on WB evidence; IXP-neutral; video script v2 and visual briefs embedded. Word-count trim needed in 3 sections.** |
| docs/ISOC Grant SPI.md | SPI submission draft. |
| docs/presentations/isif-capability-video/slides.pptx | Editable video deck (6 slides, RISE brand, photo placeholders). |
| docs/presentations/isif-capability-video/build_slides.py | python-pptx build script. Re-run to regenerate PPTX from scratch. |
| docs/research/2026-04-23-worldbank-broadband-validation-and-capability-reframe.md | WB source validation + causal reframe rationale. |
| docs/research/2026-04-22-spi-fluxx-registration-and-attachment-requirements.md | SPI portal mapping. |
| docs/research/2026-04-16_master-fact-check-and-fixes.md | Claim validation tracker. |
| Sample Form ISIF 2026.pdf | Portal field spec reference. |
| docs/RISE Style Guide 2019.pdf | Brand system (colors, typography, logo rules). |

## Standing Preferences

- No em-dashes in any prose the assistant writes or edits.
- RISE is always all-caps, never "Rise".
- No hard RISE co-invest dollar figures in grant drafts; frame as conditional/multi-sourced.
- GetaFIX member count is 126+ Manila (website stale at 65+).
- IXP-neutral framing for ISIF Capability: program mechanics and outcomes must not privilege GetaFIX; RISE is convener not commercial beneficiary.
