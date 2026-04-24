# 2026-04-24 — WB PDF small-ISP bandwidth claims + Capability final polish

## Part 1. WB PDF: what it actually says about small-ISP bandwidth costs

Source: `docs/research/Reforms Promoting Competition and Increasing Investment for Broadband Infrastructure.pdf` (World Bank, January 2024, 77 pages).

### The two quantified small-ISP cost figures

| Figure | What it measures | Location |
|---|---|---|
| **~⅓ of revenue** | Wholesale bandwidth cost (OPEX paid to telcos) | p. 18 prose + Table 1 footnote |
| **17% of revenue** | CAPEX — small-ISP own network build | p. 19 Table 1 |

Table 1 headline prose (p. 18): *"Small ISPs are estimated to have invested less than 20 percent of revenue to CAPEX in the last 5 years, while cost of wholesale bandwidth increased, reaching one-third of revenue in 2022."*

### The 47% misremembering

The 47% in the PDF is **not** a small-ISP bandwidth figure. It's **Globe/PLDT CAPEX as % of aggregate revenue** (Table 1, p. 19) — the duopoly side of the comparison. Small ISPs sit at 17%. The report's causal argument: small ISPs can't reinvest (17% CAPEX) because wholesale bandwidth OPEX (~⅓ of revenue) is crushing their margins.

Full Table 1 (p. 19, 2017–22 averages):

| Metric | Globe/PLDT | Small ISPs |
|---|---|---|
| Revenue growth | 29% | 83% |
| EBITDA margin | 49% | 16% |
| Net income margin | 14% | 4% |
| CAPEX (% of aggregate revenue) | 47% | 17% |

### Other defensible references from the PDF

- **p. 26:** "Small players find that connecting local communities to the nearest local telco facility costs more than connecting to a data center overseas."
- **p. 71 fn 35:** "It can be 40–60 percent cheaper for a cable operator to lay its own infrastructure instead of going through a telco."
- **p. 9:** "Small ISPs rely on the telcos for wholesale bandwidth and facilities. There are no regulations preventing anti-competitive interconnection price discrimination."
- **p. 26 §3.2:** "As infrastructure owners and wholesalers, the large telcos have an advantage on access and pricing, and small ISPs have little power to negotiate for a fair price."

The PDF **does not publish per-Mbps wholesale rates**. All quantified claims about small-ISP bandwidth cost are relative (% of revenue, % cheaper to self-build), not absolute prices.

## Part 2. Capability concept note final polish

Word-count audit revealed three sections still over cap after prior drafting. All trimmed today:

| Section | Before | Cap | After |
|---|---|---|---|
| Challenge | 104 | 100 | 100 |
| Approach | 107 | 100 | 100 |
| M&E | 82 | 75 | 75 |

Stale parenthetical counters refreshed across all 8 sections.

### Video script beat 2 softened (causal-chain rewrite)

Original beat 2 made an on-camera claim that "roughly half of their revenue goes straight to wholesale bandwidth." This conflicted with both the concept note (which says "roughly a third", citing WB) and the WB source itself (one-third, p. 18). Gio preferred not to commit to a specific unprovable bandwidth-% claim on camera.

**Rewritten beat 2** (57 words, 0:15–0:40):

> Small ISPs carry the expansion. Many began as cable TV operators, now running fiber. They earn a sixteen percent EBITDA margin, against the duopoly's forty-nine, and reinvest only seventeen percent of revenue in CAPEX, against forty-seven. Without the technical capability to operate efficiently, there's little left to reinvest. That's why they can't build faster, cheaper, or better.

Two defensive moves:
1. Replaces the unprovable "half of revenue to bandwidth" with the **qualitative** "without the technical capability to operate efficiently, there's little left to reinvest" — lines the video up with the grant's capability thesis instead of relying on a % claim Gio can't fully vouch for.
2. Aligns the spoken numbers to **what's actually on slide 3** (EBITDA 16 vs 49; CAPEX 17 vs 47). Previous script cited net margin 4% and bandwidth % — neither appeared on the slide the speaker stands in front of.

Visual 2 brief in the concept note updated to match the slide (two metrics, not four) and to explicitly state the bandwidth-% figure is omitted from the slide for defensibility.

Total script now 268 spoken words at ~112s, comfortably inside 2:00.

### Slide deck manual fixes flagged (to be applied in PowerPoint/Keynote)

Because `slides v3.pptx` was hand-edited after `build_slides.py` produced `slides.pptx` (12 slides vs. 6 in the Python source), these edits have to happen in PowerPoint — the Python build script is no longer the source of truth for v3:

1. Slide 2 title: "a Internet" → "an Internet"
2. Slide 3 title: "expansions" → "expansion"
3. Slide 3 header: "EBITDAs" → "EBITDA margin"
4. Slide 4 fourth box: widen or shorten to "Reinvestment capacity restored" (text currently breaks "reinvestmen | t" mid-word)
5. Slide 5 title: "IXPerience Pro" → "IXperience Pro" (match cover)

## Part 3. PowerPoint recording discovery

Gio recorded narration in PowerPoint but couldn't find the output. Diagnosed:

- `slides v3.pptx` (32 MB) contains **two embedded MP4 segments**: `ppt/media/media1.mp4` (11.9s) and `ppt/media/media2.mp4` (5.5s). Combined: ~17 seconds of 960×540 h.264 video + AAC audio.
- PowerPoint's "Record Slide Show" embeds audio/video **per slide into the PPTX**, not as a standalone video file. To get a shareable MP4 for YouTube upload, an explicit **File → Export → Create a Video** step is required (which Gio had not yet done).
- Of a 2-minute script, only ~17 seconds was captured — 1–2 slides narrated, the rest bare. Re-record needed.

Extracted segments sit in `docs/presentations/isif-capability-video/extracted-recording/` and are gitignored (regeneratable from the PPTX).
