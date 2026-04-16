# Master Fact-Check & Required Fixes — All Three Grant Applications

**Date:** 2026-04-16
**Status:** Living document. Updated as validation agents report back.

---

## CLAIM VALIDATION TABLE

### GetaFIX & Rise Statistics

| Claim in Grant | Source Checked | Actual Data | Status |
|---|---|---|---|
| "126+ Manila members" | Wholesale Analysis (product_bible_v2) | 126 members (Oct 2025) | VALIDATED |
| "950+ Gbps peak" | Wholesale Analysis | 1 Tbps+ peak (2025) | UNDERSTATED — update to "1 Tbps+" |
| "96% CAGR" | Wholesale Analysis | Member CAGR = 59% (7yr); Traffic CAGR = 111% (4yr) | UNVALIDATED — 96% matches neither metric. Must reconcile. |
| "since 2018, ASN AS23942" | Wholesale Analysis | Confirmed 2018 launch, 5 founding members | VALIDATED |
| "GetaFIX Cebu 12 members, 20 Gbps" | Wholesale Analysis | Confirmed | VALIDATED |
| "GetaFIX Davao 8 members, 20 Mbps" | Wholesale Analysis | Confirmed — but 20 Mbps is real (not typo) | VALIDATED but flagged — 500x growth target to 10 Gbps needs explanation |
| "country's largest multi-city neutral IXP" | Wholesale Analysis | Only IXP with 3+ locations | VALIDATED |

### IXperience Workshop Data

| Claim in Grant | Source Checked | Actual Data | Status |
|---|---|---|---|
| "126 unique companies" | Attendee data (cleaned) | 155 unique companies (incl. FICTAP 2026) | UNDERSTATED — 2025-only = needs recount; total is 155 |
| "~155 participants" | Attendee data | 251 total attendees (incl. FICTAP 2026) | UNDERSTATED — 2025-only: 194 (Cebu 55 + Davao 63 + Manila 76) |
| "50%+ provincial coverage" | Attendee data (company_provinces.csv) | 71.3% provincial (where data available) | UNDERSTATED — update to "70%+" |
| "Cebu, Davao, Manila in 2025" | Attendee data | All 3 confirmed + FICTAP Manila Mar 2026 | VALIDATED + additional event |
| Partners: APNIC, DE-CIX, PhNOG | IXperience brief | Confirmed as Program Partners | VALIDATED |
| Community: FICTAP, PCTA, ITAP, ISOC PH | IXperience brief | All confirmed | VALIDATED |
| "86% attendance rate" | IXperience brief (sponsorship materials) | Mentioned in brief | VALIDATED (source: sponsorship docs) |

### Pricing Claims

| Claim in Grant | Source Checked | Actual Data | Status |
|---|---|---|---|
| "Manila wholesale $0.27-0.50/Mbps" | MCP rise-pricing (112 records) | Globe intra-city $0.27, Converge $0.50 at 10G | VALIDATED |
| "provincial ISPs pay $3-5/Mbps" | MCP rise-pricing (actual quotes) | Globe Camarines Norte $4-5.51, PLDT Iloilo $3.50 | VALIDATED |
| "$0.27-0.55 at 10-30G" (Challenge) | MCP rise-pricing | PLDT at 2G hits $0.55; range confirmed | VALIDATED |
| "9 long-haul DC-to-DC quotes" | MCP rise-pricing | 59 transport records available | PLAUSIBLE but exact 9-quote subset not verified |
| "structural cost gap only volume can close" | MCP + Wholesale Analysis | 7-15x gap confirmed by actual quotes | VALIDATED |
| "20-40x below current wholesale" (unit cost) | NOT VALIDATED | If wholesale = $0.27-0.50, then 20-40x below = $0.007-0.025/Mbps. Extraordinary claim, no source. | REMOVE or reframe |
| "order of magnitude below retail" | Consistent with 60-80% reduction? | 10x = $0.30-0.50 provincial rate. But 60-80% reduction = 2-5x. INCONSISTENT. | FIX — use one number |
| "60-80% reduction vs incumbent retail" | MCP pricing + Wholesale Analysis | Plausible if Rise offers ~$0.60-1.00/Mbps vs $3-5 retail | PLAUSIBLE — needs Rise's target provincial rate stated |

### Infrastructure & PDSCN Claims

| Claim in Grant | Source Checked | Actual Data | Status |
|---|---|---|---|
| "Rise commits $300K for PDSCN spectrum" | Dylan Clear (Slack, 2026-04-15) | Dylan: "assume 300k for the spectrum, 3.5% O&M." This is an engineering estimate, not a formal quote. $10M in shared_infra_plan is full 176-city network — different scope. | RESOLVED — $300K is segment-level spectrum IRU estimate. Say "estimated" not "committed." |
| "$30K per segment for 400G capacity" | Dylan Clear (Slack, 2026-04-15) | Dylan: "approximately 30k USD per segment for 400G capacity (segment being one point to point between nodes)." 3 segments (CEB/ILO/DVO) = ~$90K. | RESOLVED — Dylan's estimate. Not Ekinops-specific; generic 400G coherent transponder cost per segment. |
| "PDSCN 2,500 km, 33 landing points" | Session summary (from Dylan) | Stated as fact in prior session | UNVERIFIED from primary source |
| "existing Rise POPs in Cebu, Iloilo, Davao" | Shared infra plan (Phase 1 cities) | All three in Phase 1 deployment | VALIDATED |
| PDSCN resale rights | Shared infra plan (cost_assumptions_review) | "NOT YET CONFIRMED" — flagged as critical dependency | RISK — grant assumes access that isn't contractually secured |

### Market Claims

| Claim in Grant | Source Checked | Actual Data | Status |
|---|---|---|---|
| "~1,500 provincial ISPs" | Wholesale Analysis + MCP ecosystem | TAM: "1,000-1,500 networks"; MCP: 1,860 Cable/DSL/ISP entities, 1,289 "access" role | VALIDATED — 1,000-1,500 is defensible range |
| "50+ million users outside Manila" | Not independently verified | PH population ~115M, NCR ~13M, so ~102M outside. 50M+ plausible as ISP-served. | PLAUSIBLE |
| "three incumbent carriers" | MCP pricing + Wholesale Analysis | Converge, Globe, PLDT confirmed as primary carriers | VALIDATED |
| "70% of PH traffic trombones via SG/HK" | Not sourced in any data found | SPI note uses this claim with no citation. MCP shows HHI 2,028 (moderate concentration) and top 3 upstream providers control 67% of market. | UNSOURCED — need citation or remove |
| "three incumbent carriers" (Converge, Globe, PLDT) | MCP ecosystem | Top 4: PLDT (132 customers), Infinivan (99), Globe (90), Converge (68). Infinivan is #2, not usually called "incumbent." | MOSTLY VALIDATED — but Infinivan is bigger than Globe/Converge by customer count |
| RISE market position | MCP ecosystem | #1 peer count (1,776), #5 downstream customers (32), present at 29 IXPs globally | NEW DATA — use to strengthen OrgCap |

---

## REQUIRED FIXES BY APPLICATION

### ALL THREE APPLICATIONS

| # | Fix | Priority |
|---|---|---|
| A1 | Remove "96% CAGR" — unverifiable, matches no known metric. Replace with "59% member CAGR over seven years (5 to 126 members)" or "traffic growing from 50 Gbps to 1 Tbps+ in four years." Gio confirmed origin unknown. | HIGH |
| A2 | Update IXperience numbers: use 2025-only figures (194 participants, ~126 companies, 3 cities) OR include FICTAP 2026 (251 participants, 155 companies, 4 events). Be explicit about timeframe. | HIGH |
| A3 | Fill all [placeholder] brackets — bios, legal name, prior grant amount | HIGH |
| A4 | Add for-profit framing paragraph: commercial sustainability = public interest persists post-grant | HIGH |
| A5 | Vary language across notes — no copy-paste phrases between the three applications | MEDIUM |
| A6 | Add prior ISIF grant outcome. Verified data: USD 150,000 grant (2023, announced APNIC 56 Kyoto, Sep 12 2023); Rise co-invested USD 130,000; 50+ schools connected; ~80,000-100,000 students reached. Project lead: Angelie Chris Sambayan-Limbag. Status: "In progress" per APNIC Foundation. Use: "Rise previously received a USD 150,000 ISIF Asia grant (Project School Internet, 2023) — connecting 50+ schools and reaching approximately 80,000 students across Metro Cebu, with Rise co-investing USD 130,000 in services." | HIGH |
| A7 | **Remove ISOC Philippines** from community partner lists in all three notes. ISOC was NOT formally part of IXperience. Can reference as potential future alignment but not current partner. (Per Gio: "ISOC was not formally part of the IXperience workshops") | HIGH |
| A8 | **Remove all PHIX references** from SPI application. PHIX is PLDT paid transit, not a neutral IXP. Reframe: GetaFIX is the ONLY neutral open IXP in the Philippines. This strengthens the case. | HIGH |
| A9 | Change "Rise commits $300,000" to "Rise estimates $300,000" or "Rise allocates an estimated $300,000" — this is Dylan's engineering estimate, not a binding commitment or formal quote | MEDIUM |
| A10 | Replace "Ekinops 400G coherent transponders" with generic "400G coherent transponder pairs" — the $30K/segment estimate is not Ekinops-specific | MEDIUM |

### ISIF INFRASTRUCTURE ($75K)

| # | Fix | Priority |
|---|---|---|
| I1 | Remove "20-40x below current wholesale" and "order of magnitude" — use only "60-80% cost reduction vs provincial incumbent retail" consistently | CRITICAL |
| I2 | Replace "spectrum" with "wavelength capacity (IRU)" throughout — "spectrum" means RF to most telecom reviewers | HIGH |
| I3 | Add indicative budget split: e.g., ~$45K transponder CapEx, ~$15K commissioning/operations, ~$15K uplift cohort | HIGH |
| I4 | Clarify Davao 20 Mbps → 10 Gbps trajectory. Either temper target or explain why growth is credible (e.g., "contingent on PDSCN backhaul commissioning") | HIGH |
| I5 | Define jargon for non-PH reviewers: PDSCN (who owns it), "trombone," "VisMin," Konektadong Pinoy Act | HIGH |
| I6 | Add governance/neutrality language: published tariff, non-discrimination policy, post-project asset disposition | HIGH |
| I7 | Add 3-phase timeline: Q1 procurement, Q2-Q3 commissioning + cohort, Q4 audit | MEDIUM |
| I8 | Add post-grant sustainability sentence | MEDIUM |
| I9 | Quantify end-user reach: how many subscribers do 10-12 target ISPs serve? | MEDIUM |
| I10 | Add baselines to all M&E indicators | MEDIUM |
| I11 | Reconcile $300K claim with $10M in shared_infra_plan — clarify scope | HIGH |
| I12 | Address PDSCN access risk — resale rights not yet confirmed per internal docs | MEDIUM |

### ISIF CAPABILITY ($50K)

| # | Fix | Priority |
|---|---|---|
| C1 | Restructure Introduction — lead with "IXperience Pro is..." not market context | HIGH |
| C2 | Sharpen differentiation from APNIC Academy: cohort structure + provincial delivery + live IXP lab + PH localization | HIGH |
| C3 | Strengthen alumni network specifics: community manager, mentorship model, what makes it persist | MEDIUM |
| C4 | Reframe M&E pre/post target: drop "+40%", use "statistically significant gains"; elevate 6-month survey as headline | MEDIUM |
| C5 | Add counterfactual: what happens if program doesn't exist | LOW |
| C6 | Add survey data: "100% of IXperience participants want future sessions; 67% 'loved the event'" | HIGH |

### ISOC SPI ($25K)

| # | Fix | Priority |
|---|---|---|
| S1 | Fill budget with real line items (use IXperience brief: total 2026 costs = $70K; SPI covers incremental community layer) | CRITICAL |
| S2 | **Add conflict-of-interest ring-fencing** — grant funds not used for sales; participation not conditional on joining GetaFIX; PHIX and other IXPs get equal treatment; independent steering committee (PhNOG + APNIC) oversees fund use; separate accounting | CRITICAL |
| S3 | **Reframe outcomes as ecosystem-first, not GetaFIX-first** — measure new peering at ANY PH IXP, not just GetaFIX/PHIX. Remove "GetaFIX onboarding" from curriculum description. Add metrics with no commercial benefit to Rise (MANRS rates, curriculum downloads, chapters meeting without Rise staff). | CRITICAL |
| S4 | Fix event count: summary says "six" but lists 5 IXperience + 2 new + 1 national = 8-9 events. Budget says "6 workshops." Reconcile. | HIGH |
| S5 | State what SPI funds vs baseline IXperience: create a table "IXperience 2026 (self-funded)" vs "SPI-funded additions." Consider distinct name for SPI component. | HIGH |
| S6 | Source "70% of PH traffic trombones via SG/HK" or remove — cite PeeringDB, APNIC traffic studies, or NTC data | HIGH |
| S7 | Clarify PHIX relationship — partner or just mentioned? Get endorsement or remove references | MEDIUM |
| S8 | Define "regional chapter" model: local champion, quarterly call, playbook, 12-month Rise remote support | MEDIUM |
| S9 | Add for-profit framing: commercial alignment as sustainability mechanism, not a conflict. "As a commercial IXP, Rise has durable incentive..." BUT pair with ring-fencing (S2) | HIGH |
| S10 | Mention this would be first SPI grant in Philippines / SE Asia | HIGH |
| S11 | Prepare community interest document: letter of support from FICTAP, PCTA, or provincial ISPs | HIGH |
| S12 | Show Rise co-investment: $24.9K sponsorship + staff time alongside $25K SPI | MEDIUM |
| S13 | Add participant travel support plan — provincial ISPs in an archipelago can't always self-fund flights | MEDIUM |
| S14 | Add survey data from IXperience Manila: 100% want future sessions, 67% "loved the event" | HIGH |

---

## DATA POINTS TO ADD (from validated sources)

### Strengthening Numbers
- GetaFIX peak traffic: update to "1 Tbps+" (currently says 950+ Gbps)
- IXperience survey: 100% want future sessions, 67% "loved the event"
- GetaFIX aggregate member savings: $6.8M annually in avoided transit costs
- Per-member ROI: 10:1 median (10 Gbps member saves $7,500/mo vs $700 port)
- New leads: 66% of IXperience attendees were new (not existing customers)
- Provincial ISP economics: Stage 4 ISP (7,000 subs) pays $16,337/mo connectivity; transport = $3,990/mo (24% of costs)
- **PLDT has zero IXP memberships** — does not participate in open peering. (Note: Converge IS a GetaFIX member despite MCP PeeringDB data gap — confirmed by Gio.)
- **129 single-homed ISPs** nationally — one upstream provider, critically vulnerable to outages
- **467 access networks in VisMin** (36% of national total) — quantifies the underserved market
- RISE has **1,776 peering relationships** across 29 IXPs globally (MCP data — verify current count via bgp.he.net)
- Total PH market: **1,860 ISP entities**, of which **1,289 are access networks**
- Prior ISIF grant: USD 150,000 (2023), 50+ schools, ~80,000 students, Rise co-invested USD 130,000

### For SPI Specifically
- IXperience 2026 total budget: $70,198 (3 legs)
- Rise self-funds $24,900/year (1 Gold + 1 Beer with Peers per event)
- SPI $25K = incremental community layer on top of funded technical calendar
- ISOC Philippines already a community partner
- FICTAP Q1 2026 event already happened with 57 attendees, 25 companies
