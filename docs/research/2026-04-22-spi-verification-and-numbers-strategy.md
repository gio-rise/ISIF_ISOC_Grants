# 2026-04-22: SPI verification + numbers strategy

## Context

Session focused on polishing SPI and Capability drafts ahead of submission (SPI deadline 23 Apr, Capability 24 Apr). Two factual questions surfaced that needed verification before final edits:

1. Claim that this would be the first SPI grant in the Philippines and in Southeast Asia.
2. The sentence "approximately 1,289 access networks, 129 are single-homed" in the SPI problem statement.

## Finding 1: SPI grant history

Verified via ISOC Foundation's 2024 and 2025 SPI grantee announcement pages. Complete awardee lists reviewed (16 in 2024, 24 in 2025, 40 total).

- No Philippine recipient in either cycle.
- One Southeast Asian recipient: **Myanmar Internet Exchange Association (MMIX)**, 2024, USD 49,645, IXP Operational Support grant.
- Confidence: high. Both pages publish complete rosters with org names and countries.

**Sources:**
- https://dev2.isocfoundation.org/2025/01/meet-the-new-grantees-improving-peering-and-interconnection-around-the-globe/
- https://www.isocfoundation.org/2026/02/introducing-the-2025-sustainable-peering-infrastructure-grantee/

**Decision:** Reinstate the claim in a corrected form. Applied: *"If awarded, this would be the first SPI grant in the Philippines, and only the second in Southeast Asia, following the Myanmar Internet Exchange Association (MMIX) in 2024."*

## Finding 2: PH ISP counts and the numbers strategy

Ran two checks:

- rise-ecosystem-remote MCP returned: 1,289 total access networks across 18 PH regions, 125 single-homed (NCR 55, Central Luzon 16, CALABARZON 14). Data timestamp 2026-04-22.
- Web cross-checks (CAIDA AS Rank, PeeringDB, APNIC) did not resolve to a single authoritative public figure.

User rejected reliance on MCP data for this submission on the grounds that the underlying ingestion is still being cleaned and cannot be certified to decimal precision. Separately, user questioned the rhetorical purpose of the single-homed sentence.

**Analysis on the single-homed detour:**

- Single-homed is a transit-diversity metric, not a peering metric. Conflates two different arguments.
- 125 of 1,289 is under 10 percent. A skeptical reviewer reads that as weakening the peering urgency argument, not strengthening it.
- The paragraph's actual thesis is community distance, not resilience. The sentence was off-argument.

**Decision:**
- Drop the single-homed sentence entirely.
- Keep numbers in the draft but hedge them. Standard hedge: "Precise counts are hard to come by; there is no single authoritative Philippine ISP registry. Best-available estimates place the total at roughly 1,500 ISPs nationally, with around two-thirds operating outside Metro Manila."
- Replace the single-homed detour with the cable-TV-to-fiber operator cohort angle (operator reality: many provincial ISPs grew out of DOCSIS cable TV, now running fiber without formal networking staff; this explains why IXperience 2025 drew 155 companies and strengthens the case for the grants).

## Standing preference saved

User expressed strong preference against em-dashes in written output. Saved as permanent feedback memory at `~/.claude/projects/-Users-gio-Code---Professional-ISIF-ISOC-Grants/memory/feedback_no_em_dashes.md`. Applied across both grant drafts and CURRENT_STATE.md this session (final em-dash count: 0 across all three files).
