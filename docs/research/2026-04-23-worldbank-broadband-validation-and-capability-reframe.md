# World Bank broadband validation and Capability concept reframe

**Date:** 2026-04-23
**Context:** Validated Gio's three-pillar broadband framing against the World Bank's January 2024 policy note. Used the findings to reframe the ISIF Capability concept paper from descriptive ("engineers lack training") to causal ("capability is the one lever small ISPs control within a measured development crisis").

## Primary source

**World Bank (January 2024) — "Better Internet for All Filipinos: Reforms Promoting Competition and Increasing Investment for Broadband Infrastructure. A Policy Note."** Document ID P502027179f71d08418678193f2fabcdbec. 58-page policy note. This is the authoritative WB assessment of the PH broadband market.

URL: https://documents1.worldbank.org/curated/en/099011824231036851/pdf/P502027179f71d08418678193f2fabcdbec.pdf

## Gio's three-pillar claims vs. WB findings

| Claim | Gio's estimate | WB finding | Verdict |
|---|---|---|---|
| Fixed broadband penetration | ~30% households, <10% in provinces | **33%** national; NCR only market >30%; "less connected" provinces (2/3 of provinces, 36% of population) <10% fixed wired | Validated; provincial gap even sharper than stated |
| Affordability | ~12% of income vs. ~5% ASEAN | Fixed broadband basket = **11% of GNI per capita**, >4x Malaysia/Viet Nam, 2x ASEAN average, **highest absolute USD price in ASEAN** | Validated at 11%, not 12% |
| Fixed speed rank | Bottom of ASEAN | PH 92 Mbps (Ookla Nov 2023), now ~105 Mbps (Aug 2025 Ookla). Below Singapore 264, Thailand 216, Viet Nam 105, Malaysia 112. Above Indonesia/Cambodia/Lao/Myanmar. | Validated against *peer* ASEAN (SG/TH/VN/MY); not literally last but the comparison that matters |
| Small-ISP bandwidth cost | ~50% of revenue | **~1/3 of revenue in 2022**, trending up | Directionally right; exact figure is one-third, not half |

## The decisive WB finding: small-ISP margin trap (Table 1)

Five-year average, 2017-2022, comparing Small ISPs vs. Globe/PLDT duopoly:

| Metric | Small ISPs | Globe/PLDT |
|---|---|---|
| Revenue growth | **83%** | 29% |
| EBITDA margin | 16% | 49% |
| Net income margin | **4%** | 14% |
| CAPEX as % of revenue | **17%** | 47% |

**Interpretation:** Small ISPs are carrying 3x the expansion growth but with 4% net margins and 17% CAPEX reinvestment. The duopoly earns 14% net and reinvests 47%. Wholesale bandwidth at ~1/3 of revenue is the single largest drain on small-ISP margins.

## The causal reframe

**Old thesis (what the Capability draft originally said):** Provincial engineers lack structured BGP/peering/RPKI training.

**New thesis (what the Capability draft now says):** The Philippines has a measurable broadband development crisis on three WB axes. Small ISPs carry the expansion mandate but are trapped in a margin structure: a third of revenue goes to wholesale bandwidth, leaving 4% net and 17% CAPEX. Within that market structure, capability is the one lever operators themselves control. Peering, routing security, and IXP participation reduce the wholesale bandwidth bill, restoring reinvestment capacity and translating into better access, affordability, and quality.

## Additional WB context worth knowing

- Philippines is the **only country worldwide that still requires a legislative franchise** for network construction and operation (regulatory entry barrier).
- The broadband market is an "effective duopoly" with Globe and PLDT vertically integrated across international, backbone, middle-mile, and last-mile.
- "There are no regulations preventing anti-competitive interconnection price discrimination, a situation disadvantageous to small ISPs."
- Open Access in Data Transmission (OADT) bill passed House in December 2022, pending Senate. Would simplify entry and mandate infrastructure sharing.
- 544 ISPs with valid NTC certificates as of 31 Aug 2022 (21 telco, 150 cable, 373 non-telco).

## PDP 2023-28 target

Government seeks to lift fixed broadband household penetration from 33% to 65%. Per WB note, WB search result cited "by 2026" but PDP plan runs to 2028; concept paper references "PDP 2023-28 target of 65 percent household fixed-broadband penetration" without a year commitment to stay safe.

## How this landed in the concept paper

- Section 3 (Challenge): full rewrite around WB three axes + small-ISP Table 1 data + "capability as lever" framing.
- Section 5 (Impact): second-order outcome explicit (reduced bandwidth spend → reinvestment → WB indicators + PDP target).
- Section 6 (M&E): added indicator #5, pre/post change in participating ISPs' wholesale bandwidth spend as share of revenue.
- Section 2 (Alignment): swapped generic strategic-aims language for explicit WB indicators.
- Section 1 (Introduction): added causal-chain closer.

## Other sources consulted

- Ookla Global Speed Index, August 2025: PH rank 54, 105 Mbps fixed.
- BusinessWorld, "The Philippines sees steady gains in internet connectivity" (April 2025).
- Opensignal, Philippines Fixed Broadband Experience Report (September 2025).
- World Bank, "Unlocking the Philippines' Digital Transformation" (July 2025 update).
