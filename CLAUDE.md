# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Grant application workspace for Rise (rise.ph) — three concurrent submissions targeting late-April 2026 deadlines:

- **ISIF Asia 2026 — Infrastructure** (USD 75K) — concept note due 24 Apr 2026. Spectrum-backed multi-city edge network using PDSCN fiber, with grant funding the public-interest de-risking layer (transponder commissioning at Cebu/Iloilo/Davao + RPKI/MANRS cohort for provincial ISPs).
- **ISIF Asia 2026 — Capability** (USD 50K) — concept note due 24 Apr 2026. IXperience Pro structured BGP/peering/routing-security curriculum for provincial ISP engineers.
- **ISOC SPI — Peering Ecosystem Support** (USD 25K) — application due 23 Apr 2026. Six regional peering-community workshops seeding provincial peering chapters.

Combined ceiling: USD 150K. Workstreams are separable — no double-billing across grants.

## Key Context

- **Rise** operates GetaFIX (Manila/Cebu/Davao IXP, ASN AS23942) and IXperience (community workshop series with APNIC, DE-CIX, PhNOG).
- The grants address the Philippine "provincial tax" — ~1,500 provincial ISPs serving 50M+ Filipinos pay $3–5/Mbps vs. Manila's $0.27–0.50/Mbps due to lack of wholesale alternatives outside three incumbents.
- Infrastructure thesis rests on Rise acquiring PDSCN spectrum IRU ($300K) with $30K Ekinops 400G transponder pairs per segment. Rise commits CapEx; grant funds public-interest layer.
- Pricing figures are backed by a statistically defensible DC-to-DC curve fit: `MRC = 823.9 × BW^0.722`, R² = 0.940, fitted on 9 incumbent observations (Infinivan treated as outlier).

## File Structure

| File | Purpose |
|---|---|
| `Grant-Applications-Rise-DRAFT.docx` | All three concept notes — cover page, ISIF Infrastructure, ISIF Capability, ISOC SPI, finalization checklist. Word-count compliant per ISIF caps. |
| `Grants-Research-Brief-Rise.docx` | Funder landscape research (ISIF/ISOC/ICANN/IGF) and bid recommendations. |
| `Grants-Tracker-Rise.xlsx` | Pipeline tracker with deadlines and status. |
| `SESSION-SUMMARY-2026-04-14-to-15.md` | Detailed session log covering pricing model validation, strategic reframing, and drafting. |

## Working with Documents

- Use the `docx` skill to read/edit Word files and `xlsx` skill for the tracker spreadsheet.
- ISIF concept notes have strict per-section word caps (Intro 250, Alignment 75, Challenge 100, Approach 100, Impact 100, M&E 75, OrgCap 100). Always verify word counts after edits.
- The docx builder script is at `/sessions/eloquent-clever-einstein/build_applications.js` (docx-js generator). If that session path is unavailable, treat the `.docx` file as the source of truth.

## Related Projects

- `isp_economics` repo — contains the production transport model (`model.py`), DC-to-DC curve fit research note, and backhaul curve CSV backing the pricing figures cited in the Infrastructure concept note.

## Open Items

- Official application forms from APNIC Foundation grants portal (ISIF) and ISOC Fluxx (SPI) need to be dropped into this folder by Gio for field mapping.
- Team bios needed: Gio Bacareza, Robertas Zudys (COO), Dylan Clear (CTO).
- Prior ISIF grant details needed: Project School Internet (Basak Elementary, Cebu) — amount and year.
- SPI workshop cities need confirmation (current placeholders: Cebu, Davao, Iloilo, Cagayan de Oro, Baguio, Puerto Princesa).
