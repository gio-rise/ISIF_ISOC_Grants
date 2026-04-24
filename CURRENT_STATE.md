# CURRENT_STATE: ISIF/ISOC Grant Applications

## Status: ISIF Capability concept note word-compliant and submission-ready. Video recording incomplete (~17s of 2:00 captured). Slide deck has 5 manual text edits pending in `slides v3.pptx`. ISOC SPI Fluxx registration submitted (awaiting approval).

> Note: APNIC Foundation grants portal is **apnic.grantplatform.com** (Good Grants), not Fluxx. Only ISOC uses Fluxx (isocfoundation.fluxx.io).

## Recent Accomplishments

### Session 2026-04-24 (Capability final polish + recording diagnosis)
- Trimmed Capability Challenge (104→100), Approach (107→100), M&E (82→75). All 8 sections now exactly at or under cap. Refreshed stale parenthetical counters across entire concept note.
- Rewrote video script beat 2 on Gio's direction: dropped unprovable "half of revenue to wholesale bandwidth" claim; replaced with qualitative "without the technical capability to operate efficiently, there's little left to reinvest." Aligned spoken numbers to what's actually on slide 3 (EBITDA 16/49, CAPEX 17/47). Total script 268 spoken words, ~112s, comfortable 2:00 fit.
- Updated Visual 2 design brief to match slide 3 (2-metric table, no bandwidth-%). Concept-note numbers still cite ⅓-to-bandwidth via WB — defensible because cited — but camera-facing claims are now structural, not numeric.
- Traced Gio's misremembered "47%" to Table 1 p. 19: it's Globe/PLDT CAPEX-as-revenue, not a small-ISP bandwidth figure. Confirmed the WB PDF quantifies small-ISP bandwidth cost only as "~⅓ of revenue" (p. 18) and "40–60% cheaper to self-build middle mile" (p. 71 fn 35). No per-Mbps wholesale rates published in the PDF.
- Diagnosed PowerPoint recording location: embedded inside `slides v3.pptx` as 2 MP4 segments (`ppt/media/media1.mp4` 11.9s, `media2.mp4` 5.5s). Only ~17s of a 2:00 script captured across 2 slides — re-record needed. Also explained PowerPoint's behavior: "Record Slide Show" embeds per-slide; no standalone video file is produced until File → Export → Create a Video.
- Produced 5-item manual slide-edit checklist for `slides v3.pptx` (cannot be patched via `build_slides.py` — PPTX was hand-edited to 12 slides after Python build): Slide 2 "a Internet"→"an Internet"; Slide 3 "expansions"→"expansion"; Slide 3 "EBITDAs"→"EBITDA margin"; Slide 4 widen or shorten "Reinvestment capacity restored"; Slide 5 "IXPerience"→"IXperience" to match cover.
- Research saved: `docs/research/2026-04-24-wb-pdf-smallisp-bandwidth-claims-and-capability-final-polish.md`.

### Session 2026-04-23 (Capability reframe + video deck)
- Validated Gio's three-pillar broadband framing against the World Bank's January 2024 policy note. Confirmed key figures: 33% fixed-broadband penetration (provinces <10%); 11% of GNI per capita affordability (highest in ASEAN); speeds below peer ASEAN (SG/TH/VN/MY); ~1/3 of small-ISP revenue on wholesale bandwidth; 4% net margin / 17% CAPEX vs. duopoly 14% / 47%. Research saved to `docs/research/2026-04-23-worldbank-broadband-validation-and-capability-reframe.md`.
- Reframed `docs/ISIF Grant Capability.md` from descriptive ("engineers lack training") to causal ("capability is the one lever small ISPs control within a measured development crisis"). Challenge and Impact rewritten on WB evidence; M&E indicator #5 added (wholesale bandwidth spend as share of revenue); Intro/Alignment/Approach/Target Beneficiaries/OrgCap lightly reworked.
- Removed GetaFIX from program mechanics after Gio pushback. Reframed Capability as community-led, IXP-neutral. GetaFIX retained only as institutional credential in OrgCap; production notes and Visual 5 mention GetaFIX only in negative form. Same ring-fencing SPI already has.
- Built video script v2 in documentary register. Built editable PPTX slide deck using python-pptx (6 native-editable slides, 50KB). Applied RISE Style Guide 2019 brand system.
- Saved integrated operational model as project memory: SPI + ISIF run as one program (IXperience Philippines 2026) with two funding-attributed layers.

### Session 2026-04-22 (late, ISOC): Fluxx registration + SPI draft softening
- Submitted RISE organization registration to ISOC Foundation Grants Portal; awaiting approval (1-2 business day SLA). Expedite email sent.
- Filled Fluxx "SPI Project Summary" (528/550 chars) and "Organization Mission" fields.
- Removed hard USD 25,000 RISE co-invest commitments from SPI draft Sections 1, 5, 7; reframed as conditional/multi-sourced.
- Verified SPI attachment requirements via WebFetch: combined Budget/Workplan/Equipment Request template + 1 community-interest doc. RISE-FICTAP MOA satisfies community-interest requirement.
- Research: `docs/research/2026-04-22-spi-fluxx-registration-and-attachment-requirements.md`.

## Next Priorities

1. **Apply 5 manual text edits to `slides v3.pptx`** in PowerPoint/Keynote (Slide 2 grammar, Slide 3 title + table header, Slide 4 word-break, Slide 5 capitalization). See session 2026-04-24 notes or `docs/research/2026-04-24-wb-pdf-smallisp-bandwidth-claims-and-capability-final-polish.md`.
2. **Re-record full 2-minute video** using corrected slide deck as background with webcam overlay. Current recording is only ~17 seconds across 2 slides. After recording: File → Export → Create a Video (MP4) → upload YouTube unlisted → paste URL into Concept Note tab.
3. **Submit ISIF Capability.** Remaining portal blockers: Application Title fix to `RISE - IXperience Pro - 2026`; Legal Registration PDF + List of Officers PDF uploads (both PDFs now staged in `docs/`).
4. **Marketing ask:** RISE signature logo PNG, 3-5 IXperience workshop photos, APNIC Academy + PhNOG + FICTAP logos. Optional Project School Internet photo.
5. **Submit SPI.** Wait for Fluxx approval, map `docs/ISOC Grant SPI.md` into Fluxx, complete Budget/Workplan template, attach MOA PDF (staged as `docs/ABA887-20260410-RPH-Memorandum of Agreement with FICTAP.pdf.pdf` — note double `.pdf.pdf` extension).

## Blockers

- 5 manual text edits pending in `slides v3.pptx` (Python source no longer matches the hand-edited v3 deck).
- Video recording incomplete: only ~17s of ~120s script captured; re-record needed.
- Video not yet exported to MP4 or uploaded to YouTube.
- Application Title needs "RISE -" prefix correction in ISIF portal.
- Legal Registration PDF + List of Officers PDF staged locally but not yet uploaded to ISIF portal.
- MOA PDF filename has double `.pdf.pdf` extension — cosmetic but worth fixing before upload.
- ISOC Fluxx registration awaiting approval (expedite email sent).
- Marketing assets (RISE logo, partner logos, IXperience photos) not yet delivered.

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
