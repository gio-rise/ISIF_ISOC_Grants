# ISIF Asia 2026 — Infrastructure Concept Note (Revised Draft v2)

**Category:** Infrastructure | **Amount:** USD 75,000 | **Duration:** 12 months | **Deadline:** 24 April 2026, 11:59 PM UTC+10

---

## Title

GetaFIX Provincial Edge Extension: Data-Driven Catchment Hubs for Underserved Philippine ISPs

---

## 1. Introduction (229 words)

The Philippine internet is two networks in one country. Metro Manila has dense peering, wholesale bandwidth at $0.27–0.50/Mbps, and 15–35 ms latency to major content. Outside Manila, approximately 1,500 provincial ISPs serving 50+ million users pay $3–5/Mbps for retail Layer-2 circuits that "trombone" — routing through Manila and back before reaching peering or transit — a structural provincial tax driven by the absence of wholesale alternatives outside three incumbent carriers.

Rise operates GetaFIX, the Philippines' largest multi-city neutral IXP (Manila 126+ members, 1 Tbps+ peak; since 2018, ASN AS23942), currently reaching four cities: Manila, Cebu, Davao, and Iloilo. Rise also runs IXperience, a technical-workshop series co-delivered with APNIC and PhNOG that engaged 155 companies and 251 participants across four events in 2025–2026.

This twelve-month program extends the GetaFIX edge beyond existing POPs into five new provincial catchment hubs — Palompon (Visayas), Cagayan de Oro and Liloy (Mindanao), and Santa Maria Pangasinan and Tarlac City (Luzon) — selected from registry clustering to maximise provincial-ISP aggregation (236 ISPs combined catchment). Rise co-invests an estimated $400–500K covering PDSCN wavelength IRU, node hardware, fiber tails, and Year-1 operations.

The grant anchors the public-interest layer: commissioning the two highest-impact flagship hubs (CDO, 61 ISPs; Sta Maria Pangasinan, 99 ISPs — 68% of new-ISP footprint), plus an RPKI/MANRS uplift cohort onboarding 10–12 provincial ISPs ahead of the Konektadong Pinoy Act's licensing wave. All playbooks publish openly under CC-BY.

---

## 2. Alignment (70 words)

The project advances ISIF Asia 2026's Infrastructure focus by deploying critical internet infrastructure — catchment-hub edge aggregation for underserved provincial Philippine networks — measurably improving performance, reliability, affordability, and local benefits for Filipino users outside Metro Manila. It strengthens RPKI and MANRS deployment at IXP and operator levels, delivers open playbooks and a PDSCN-backed catchment-extension reference topology reusable across APAC economies facing urban-rural backhaul asymmetry, and advances pilot and scalable-prototype objectives.

---

## 3. Challenge (96 words)

Provincial Philippine ISPs pay three-to-ten times Manila's wholesale rates because no edge-aggregation infrastructure exists in their regions — forcing them to backhaul through Manila on incumbent retail circuits. Even where GetaFIX reaches (Cebu, Davao, Iloilo), coverage is metro-only; provincial ISPs in Misamis Oriental, Zamboanga del Norte, Pangasinan, Tarlac, and Leyte have no nearby neutral aggregation point. A small provincial ISP buying 1–2G retail pays $3–5/Mbps versus $0.27–0.50/Mbps at volume in Manila. RPKI ROA publication and MANRS compliance among provincial ASNs remain sparse, amplifying routing-security risk as the Konektadong Pinoy Act brings new entrants.

---

## 4. Approach (99 words)

Two coordinated workstreams over 12 months. Workstream A — Catchment-hub edge extension: Rise co-invests ~$400–500K for PDSCN wavelength IRU, node hardware, fiber tails, and Year-1 operations across five new catchment hubs (Palompon, CDO, Liloy, Sta Maria Pangasinan, Tarlac — 236 provincial ISPs). Grant funds transponder pairs, node hardware, and commissioning at the two flagship hubs (CDO and Sta Maria Pangasinan — 68% of new-ISP footprint), with dual redundant route servers, RPKI ROV, MANRS-IXP compliance, and published non-discriminatory tariffs. Workstream B — Provincial uplift cohort: 10–12 provincial ISPs from the catchment publish ROAs, deploy ROV, achieve MANRS-Operator. Progress publishes openly.

---

## 5. Impact (99 words)

Within 12 months: flagship GetaFIX catchment hubs operational at Cagayan de Oro and Santa Maria Pangasinan over PDSCN-backed wholesale capacity, serving 160 provincial ISPs (68% of new catchment); published wholesale rates delivering 60–80% cost reduction versus incumbent retail. Ten-to-twelve provincial ISPs from the catchment publish ROAs, deploy ROV, and achieve MANRS-Operator compliance. Measurable latency reduction for provincial users across Visayas, Mindanao, and Luzon to top-20 content destinations. Rise extends to three additional hubs (Palompon, Liloy, Tarlac) from commercial capital by month 18 — 236 ISPs under coverage. Post-grant, wavelength and node assets sustain wholesale revenue independently. All playbooks publish under CC-BY.

---

## 6. M&E (73 words)

Six indicators tracked monthly on an open dashboard: (1) wholesale rate per Mbps at CDO and Sta Maria versus incumbent baseline ($3–5/Mbps); (2) provincial ISPs onboarded at flagship hubs (baseline: zero); (3) traffic at flagship hubs (baseline: zero); (4) RPKI ROA coverage and MANRS compliance across participating ASNs; (5) new peering sessions at flagship sites; (6) provincial-to-top-20-content latency, baselined at project start. PhNOG-nominated independent reviewers audit at months 6 and 12.

---

## 7. Organisational Capability (96 words)

Rise is a Philippine for-profit operating GetaFIX — the country's largest multi-city neutral IXP (Manila, Cebu, Davao, Iloilo; since 2018; ASN AS23942; 1 Tbps+ peak) — and runs IXperience with APNIC and PhNOG (155 companies, 251 participants across four events, 2025–2026). Rise previously received a USD 150,000 ISIF Asia grant (Project School Internet, 2023) — 50+ schools and ~80,000 students across Metro Cebu, with Rise co-investing USD 130,000; the same skin-in-the-game pattern extends here. Core team: Gio Bacareza, President — 25+ years internet/telecom, former VP Smart Communications; Dylan Clear, Group CTO — 19 years carrier networking, former Juniper; Robertas Zudys, Group COO — former Head of Wholesale, Telia Lietuva.

---

## Open placeholders (to confirm before submission)

1. **Exact Rise co-investment total** — currently stated as "~$400–500K." Confirm with Dylan the precise figure covering PDSCN IRU + node hardware across 5 hubs + fiber tails + Year-1 opex.
2. **Opex sustainability math** — currently implicit in Impact ("assets sustain wholesale revenue independently"). Reviewers will ask "what happens after Year 1?" Need a line like "at N committed ISPs × M Mbps × $P/Mbps wholesale per flagship hub, each hub covers recurring wave + node opex by month Q." Dylan's numbers.
3. **`99*` on Sta Maria Pangasinan** — confirmed correct per clustering; asterisk can be removed from the source table when submitting.
4. **PDSCN resale rights** — flagged as unresolved in the 2026-04-16 fact-check. Needs written confirmation from Eastern Telecom / Globe / Infinivan before full-proposal stage (not required for concept note, but reviewers may ask).
