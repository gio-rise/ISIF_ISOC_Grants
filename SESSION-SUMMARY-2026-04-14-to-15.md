# Session Summary — Rise Grant Applications

**Dates:** 14–15 April 2026 (continued into 16 April)
**Owner:** Gio Bacareza (gio.bacareza@rise.ph)
**Subject:** ISIF Asia 2026 + ISOC SPI 2026 grant submissions for Rise / GetaFIX

---

## Purpose

Get Rise three submission-ready grant applications before the late-April 2026 deadlines:

- **ISIF Asia 2026 — Infrastructure** (USD 75,000) — concept note due 24 Apr 2026
- **ISIF Asia 2026 — Capability** (USD 50,000) — concept note due 24 Apr 2026
- **ISOC Sustainable Peering Infrastructure — Peering Ecosystem Support** (USD 25,000) — application due 23 Apr 2026

Combined potential funding: USD 150,000 across the three programs.

---

## Problem we are solving (the underlying thesis the grants address)

The Philippine internet is two networks in one country. Metro Manila has dense peering, wholesale bandwidth at $0.27–0.50/Mbps, and 15–35 ms latency to major content. Outside Manila, ~1,500 provincial ISPs serving 50+ million Filipinos pay $3–5/Mbps for small retail Layer-2 circuits that trombone through Manila — a structural "provincial tax" caused by the absence of any wholesale alternative outside three incumbent carriers.

Rise already operates the public-interest infrastructure to fix this — GetaFIX (Manila / Cebu / Davao IXP, ASN AS23942) and IXperience (community workshop series with APNIC, DE-CIX, PhNOG). The grants are designed to fund three coordinated, separable workstreams:

1. **Infrastructure** — commission spectrum-backed wholesale backhaul + regional GetaFIX edge nodes to collapse the cost gap.
2. **Capability** — convert IXperience into IXperience Pro, a structured BGP / peering / routing-security curriculum for provincial ISP engineers.
3. **Peering ecosystem** — six regional peering-community workshops to seed durable provincial peering chapters.

---

## How we did it (chronological)

### Phase 1 — Pricing model rigor
- Validated and updated the production transport curve in the parallel `isp_economics` project. Discovered the previously cited March curve (25th percentile, $0.20/Mbps at 100G) was stale; the current production median curve is `MRC = 580 × BW^0.880 × 1.10` ($0.37/Mbps at 100G).
- Drew the distinction between **DC-to-POI** (transport with last-mile tail, exponent 0.88) and **DC-to-DC** (wholesale backhaul, exponent 0.72) — they differ in shape and cross around 5G.
- Fitted a log-log OLS regression on 9 incumbent long-haul DC-to-DC observations: `MRC = 823.9 × BW^0.722`, R² = 0.940. Computed 95% prediction intervals out to 200G. Treated Infinivan as an outlier providing a ~40% discount vs. incumbent.
- Documented this in the `isp_economics` repo (research note + CSV curve table) so the numbers used in the grant are statistically defensible.

### Phase 2 — Strategic reframing
- After the fit, Dylan (Rise CTO) shared a quote: Rise can acquire **network-wide PDSCN spectrum IRU for $300K** with **$30K Ekinops 400G transponder pairs per segment**.
- This invalidated the original "subsidize wave fill" thesis. The Infrastructure concept note was reframed around a **spectrum-backed multi-city edge network** — a structurally different wholesale model where Rise commits the $300K spectrum CapEx and the grant funds the public-interest layer (transponder commissioning at Cebu / Iloilo / Davao + RPKI/MANRS uplift cohort for 10–12 provincial ISPs).
- Confirmed PDSCN topology (2,500 km, 33 landing points, owners Eastern Telecom / Globe / Infinivan, RFS April 2023). Davao isn't on PDSCN directly, but Infinivan's Cagayan de Oro–Davao terrestrial extension closes the gap.
- Confirmed Rise already has POPs in Cebu, Davao, and Iloilo — zero POP CapEx required.

### Phase 3 — Drafting and document build
- Built `build_applications.js`, a docx-js generator that produces all three concept notes in a single Word document with consistent formatting, orange-highlighted placeholders, and word-count target annotations.
- Rewrote the ISIF Infrastructure note end-to-end around the PDSCN narrative.
- Verified all seven capped sections programmatically — every section comes in within ISIF's strict word limits (Intro 247/250, Alignment 73/75, Challenge 96/100, Approach 94/100, Impact 92/100, M&E 72/75, OrgCap 91/100).
- Capability and SPI concept notes left intact — already consistent with the new framing; cover page asserts "no activity is double-billed" between the three.

### Phase 4 — Finding the official application templates
- Attempted to download the official ISIF and SPI question forms.
- Both `apnic.foundation` and `isocfoundation.org` are blocked by my network egress proxy. The forms are also gated behind portal login (APNIC Foundation grants portal for ISIF; ISOC Fluxx for SPI).
- Outcome: Gio needs to log in and pull the forms manually, then drop them into this folder. Once they're here, I can map the current draft content onto the official field structure.

---

## Key decisions made

| # | Decision | Rationale |
|---|---|---|
| 1 | Shift Infrastructure thesis from "subsidize wave fill" to "spectrum-backed edge network with grant-funded de-risking layer" | Dylan's $300K PDSCN spectrum quote inverted the economics — Rise can credibly commit the CapEx itself |
| 2 | Treat Infinivan as outlier in pricing curve, fit on incumbent quotes only | Infinivan offers a structurally different (40%+) discount; mixing distorts the prevailing-rate baseline |
| 3 | Use median DC-to-DC curve (not 25th percentile) for grant figures | The 25th percentile is a best-case quote, not a defensible baseline; median + 95% PI is the rigorous choice |
| 4 | Cite Cebu, Iloilo, Davao as Workstream A edge sites | Existing Rise POPs at all three → zero POP CapEx; Davao reachable via Infinivan CDO terrestrial extension |
| 5 | Bid all three grants concurrently rather than sequence | Workstreams are separable (no double-billing); deadline pressure is comparable; combined ceiling materially larger |
| 6 | Keep concept notes within ISIF word caps without exception | ISIF is strict about word limits; over-cap drafts get cut by reviewers, not by us |
| 7 | Submit ISOC SPI first (23 Apr), ISIF concept notes second (24 Apr) | Ordered by deadline |
| 8 | Defer S5 "Rise-owned PDSCN wave" model strategy in `isp_economics` until after submissions | Modeling work doesn't block grant submissions; submissions block on a hard external deadline |

---

## Files in this folder relevant to the project

| File | What it is | Status |
|---|---|---|
| `Grant-Applications-Rise-DRAFT.docx` | All three concept notes in one Word document — cover page, ISIF Infrastructure, ISIF Capability, ISOC SPI, finalization checklist | Current draft. Word-count compliant. Awaits Gio's bios + prior-grant numbers + official-form mapping. |
| `Grants-Research-Brief-Rise.docx` | Earlier research brief mapping the funder landscape (ISIF / ISOC / ICANN / IGF / others) and recommending which to bid | Reference. Created 14 Apr. |
| `Grants-Tracker-Rise.xlsx` | Tracker spreadsheet for grant pipeline, deadlines, status | Reference. Currently open (lock file present). |
| `SESSION-SUMMARY-2026-04-14-to-15.md` | This document | Just created. |

### Files outside this folder, but relevant
- `/sessions/eloquent-clever-einstein/build_applications.js` — the docx-js builder. Edit this and re-run `node build_applications.js` to regenerate `Grant-Applications-Rise-DRAFT.docx`.
- `/sessions/eloquent-clever-einstein/mnt/isp_economics/docs/research/2026-04-15_dcdc-backhaul-curve-fit.md` — DC-to-DC curve fit research note backing the pricing figures cited in the Infrastructure concept note's Challenge section.
- `/sessions/eloquent-clever-einstein/mnt/isp_economics/data/backhaul_dcdc_curve.csv` — curve table at 1–200G with prediction intervals.
- `/sessions/eloquent-clever-einstein/mnt/isp_economics/report/model.py` — production transport model (current curve: median, 59 MCP records, updated 2026-04-13).

---

## Open items for Gio

1. **Pull the official application forms** from the APNIC Foundation grants portal and ISOC Fluxx, drop into this folder. (See previous response for the exact steps.)
2. **Provide team bios** — Gio Bacareza, Robertas Zudys (COO), Dylan Clear (CTO).
3. **Provide prior ISIF grant details** — Project School Internet (Basak Elementary School, Cebu): grant amount in USD and year awarded.
4. **Confirm SPI workshop cities** — current draft lists Cebu, Davao, Iloilo, Cagayan de Oro, Baguio, Puerto Princesa as placeholders.
5. **Once the official forms arrive**, I will map current draft content onto the official field structure and produce final submission-ready versions for Gio's review.

---

## Next session — start here

> "I've dropped the official ISIF and SPI forms into the Grants folder. Map my current drafts onto the official fields and tell me what's missing."
