# ISIF Infrastructure — Catchment Hub Thesis and Grant Split Decision

**Date:** 2026-04-20
**Context:** Rewrite of `revised-ISIF-Infrastructure-v2.md` from "commission transponders at existing POPs" to "extend GetaFIX edge beyond existing POPs into data-driven catchment hubs."

## Thesis shift

### Old framing (v2 as of 2026-04-16)
Grant funds 400G transponder pairs at Rise's 3 existing POPs (Cebu, Iloilo, Davao). "Zero POP CapEx required" was cited as a feature. Narrower story: upgrade-in-place at existing sites.

### New framing (v2 as of 2026-04-20)
Grant funds catchment-hub **extension** — new provincial aggregation points beyond Rise's 4 existing POPs (Manila, Cebu, Davao, Iloilo). Target: let provincial ISPs connect to a nearby neutral aggregation point rather than backhaul to a main metro POP.

## Catchment hub selection (registry clustering)

| Zone | Hub | ISPs | Status |
|---|---|---|---|
| Visayas | Palompon, Leyte | 35 | NEW |
| Visayas | Iloilo City | 30 | Already Rise POP (no CapEx) |
| Mindanao | Cagayan de Oro | 61 | NEW |
| Mindanao | Liloy, Zamboanga del Norte | 28 | NEW |
| Luzon | Santa Maria, Pangasinan | 99 | NEW |
| Luzon | Tarlac City | 13 | NEW |

**Total: 5 new hubs + Iloilo existing = 236 new ISPs onboarded / 266 total catchment.**

## Grant split — decision: concentrated, 2 flagships

Options evaluated:

| Option | Description | Rejected because |
|---|---|---|
| A — Spread $15K × 5 hubs | Grant partial-CapEx at each hub | Muddy attribution; no flagship delivered fully; execution risk high |
| B — 2 flagships only | Grant fully commissions 2 highest-impact hubs | **CHOSEN** |
| C — Mix (1 flagship + 2 lighter nodes) | One full-stack hub + 2 aggregation-only | Less clean story; still 3 sites of deliverables |

**Flagships chosen: CDO (61) + Sta Maria Pangasinan (99) = 160 ISPs = 68% of new catchment.**

### Why concentrated

1. **Clean attribution** — reviewers can point to specific grant-delivered infrastructure
2. **Geographic diversity** — Mindanao + North Luzon = 2 of 3 macro-zones
3. **Failure mode** — if PDSCN slips at one site, the other still delivers
4. **ISIF evaluation criteria** — favour "working systems / pilot projects / scalable prototypes"
5. **Sustainability proof** — 2 hubs break-even is a tighter bet than 5; "prove 2, scale to 5 with commercial capital" is the post-grant narrative

## Budget structure

| Component | Amount | Funder |
|---|---|---|
| Transponder pair + node hardware + commissioning, CDO flagship | ~$32K | ISIF grant |
| Transponder pair + node hardware + commissioning, Sta Maria flagship | ~$32K | ISIF grant |
| RPKI/MANRS uplift cohort — 10–12 provincial ISPs | ~$11K | ISIF grant |
| **Grant subtotal** | **$75K** | |
| PDSCN wavelength IRU (network-wide) | ~$300K | Rise |
| 3 additional hubs (Palompon, Liloy, Tarlac) + all fiber tails + Year-1 opex | ~$100–200K | Rise |
| **Rise co-investment** | **~$400–500K** | |
| **Total project** | **~$475–575K** | |

**Grant ratio: ~14% of project cost** — stronger skin-in-the-game than 2023 Project School Internet (54% ISIF / 46% Rise).

## Open placeholders in the draft

1. Exact Rise co-investment figure — needs Dylan to confirm precise number
2. Opex sustainability math — needs "at N ISPs × M Mbps × $P/Mbps per hub, breakeven by month Q" from Dylan
3. `99*` asterisk on Sta Maria — user confirmed 99 is correct, asterisk removable
4. PDSCN resale rights — flagged unresolved in 2026-04-16 fact-check; not required for concept note but reviewers may ask

## Message artifacts produced in this session

- Revised CTO consult message to Dylan (opex-after-subsidy concern + catchment hub thesis)
- C-suite announcement message (3 grants, lodging within week, Infrastructure still being finalised)
