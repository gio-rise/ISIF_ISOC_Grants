---
marp: true
paginate: false
theme: default
style: |
  section {
    font-family: -apple-system, BlinkMacSystemFont, "Helvetica Neue", Arial, sans-serif;
    background: #ffffff;
    color: #1a202c;
    padding: 56px 72px;
    width: 1280px;
    height: 720px;
  }
  h1 {
    font-family: Georgia, "Source Serif Pro", serif;
    color: #1a365d;
    font-weight: 600;
    font-size: 1.85em;
    margin: 0 0 0.15em 0;
    border-bottom: 2px solid #e2e8f0;
    padding-bottom: 0.2em;
  }
  .subtitle {
    color: #4a5568;
    font-size: 1em;
    margin-bottom: 1em;
    font-style: italic;
  }
  .source {
    position: absolute;
    bottom: 28px;
    left: 72px;
    right: 72px;
    font-size: 0.65em;
    color: #a0aec0;
    font-family: Georgia, serif;
  }
  /* Slide 1: three stat cards */
  .stat-grid {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    gap: 24px;
    margin-top: 0.8em;
  }
  .stat-card {
    padding: 28px 24px;
    background: #f7fafc;
    border-left: 6px solid #1a365d;
    border-radius: 2px;
  }
  .stat-card .big {
    font-size: 3.2em;
    font-weight: 700;
    color: #1a365d;
    line-height: 1;
    margin: 0;
    font-family: Georgia, serif;
  }
  .stat-card .label {
    font-size: 0.85em;
    font-weight: 600;
    color: #2d3748;
    margin-top: 10px;
    text-transform: uppercase;
    letter-spacing: 0.08em;
  }
  .stat-card .context {
    font-size: 0.78em;
    color: #4a5568;
    margin-top: 12px;
    line-height: 1.4;
  }
  /* Slide 2: comparison table */
  .compare-table {
    width: 100%;
    margin-top: 0.6em;
    border-collapse: collapse;
  }
  .compare-table th {
    text-align: left;
    padding: 14px 16px;
    color: #2d3748;
    border-bottom: 2px solid #cbd5e0;
    font-size: 0.8em;
    text-transform: uppercase;
    letter-spacing: 0.06em;
  }
  .compare-table th.metric { width: 46%; }
  .compare-table th.small-isp { color: #c53030; text-align: center; }
  .compare-table th.duopoly { color: #2c5282; text-align: center; }
  .compare-table td {
    padding: 14px 16px;
    border-bottom: 1px solid #edf2f7;
    font-size: 1em;
  }
  .compare-table td.metric-name { color: #2d3748; }
  .compare-table td.number {
    font-weight: 700;
    font-family: Georgia, serif;
    font-size: 1.4em;
    text-align: center;
  }
  .compare-table td.small-isp { color: #c53030; }
  .compare-table td.duopoly { color: #2c5282; }
  .callout {
    margin-top: 0.8em;
    padding: 14px 18px;
    background: #fffaf0;
    border-left: 4px solid #d69e2e;
    font-size: 0.85em;
    color: #744210;
    line-height: 1.4;
  }
  /* Slide 3: causal chain */
  .chain {
    display: grid;
    grid-template-columns: 1fr 0.4fr 1fr 0.4fr 1fr 0.4fr 1fr 0.4fr 1.1fr;
    gap: 0;
    margin-top: 1.4em;
    align-items: stretch;
  }
  .chain-box {
    padding: 22px 14px;
    background: #f7fafc;
    border-top: 4px solid #1a365d;
    text-align: center;
    font-size: 0.9em;
    color: #2d3748;
    display: flex;
    align-items: center;
    justify-content: center;
    min-height: 100px;
    line-height: 1.35;
    font-weight: 500;
  }
  .chain-arrow {
    display: flex;
    align-items: center;
    justify-content: center;
    color: #a0aec0;
    font-size: 1.6em;
    font-weight: 300;
  }
  .chain-outcome {
    background: #ebf8ff;
    border-top-color: #2c5282;
    font-weight: 600;
    color: #2c5282;
  }
  .chain-note {
    margin-top: 1.5em;
    font-size: 0.85em;
    color: #4a5568;
    font-style: italic;
    text-align: center;
  }
  /* Slide 4: curriculum */
  .curriculum {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr 1fr;
    gap: 14px;
    margin-top: 0.8em;
  }
  .module {
    padding: 22px 16px;
    background: #f7fafc;
    border-top: 4px solid #1a365d;
    border-radius: 2px;
  }
  .module .num {
    font-family: Georgia, serif;
    font-size: 0.72em;
    color: #718096;
    letter-spacing: 0.12em;
    text-transform: uppercase;
  }
  .module .name {
    font-weight: 600;
    font-size: 1.05em;
    color: #1a365d;
    margin-top: 8px;
    line-height: 1.3;
  }
  .ttt-strip {
    margin-top: 1em;
    padding: 16px 22px;
    background: #f0fff4;
    border-left: 4px solid #38a169;
    font-size: 0.92em;
    color: #22543d;
    line-height: 1.5;
  }
  .ttt-strip strong { color: #276749; }
  /* Slide 5: credibility */
  .cred-stats {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr 1fr;
    gap: 18px;
    margin-top: 0.6em;
  }
  .cred-stat {
    padding: 18px 14px;
    background: #f7fafc;
    border-top: 3px solid #1a365d;
    text-align: center;
  }
  .cred-stat .num {
    font-family: Georgia, serif;
    font-size: 2.6em;
    font-weight: 700;
    color: #1a365d;
    line-height: 1;
  }
  .cred-stat .label {
    font-size: 0.78em;
    color: #4a5568;
    margin-top: 8px;
    text-transform: uppercase;
    letter-spacing: 0.06em;
  }
  .cred-pills {
    display: flex;
    flex-direction: column;
    gap: 10px;
    margin-top: 1em;
  }
  .pill {
    padding: 12px 18px;
    background: #edf2f7;
    border-left: 3px solid #2c5282;
    font-size: 0.85em;
    color: #2d3748;
    border-radius: 2px;
  }
  .pill strong { color: #1a365d; }
  /* Photo placeholder */
  .photo-placeholder {
    margin-top: 1em;
    background: #edf2f7;
    border: 2px dashed #cbd5e0;
    padding: 28px 20px;
    text-align: center;
    color: #718096;
    font-size: 0.78em;
    font-style: italic;
    border-radius: 4px;
  }
  /* Closing slide */
  section.closing {
    background: #1a365d;
    color: #edf2f7;
    padding: 72px 96px;
  }
  section.closing h1 {
    color: #ffffff;
    border-bottom-color: #4a5568;
    font-size: 2em;
  }
  section.closing ul.loop {
    list-style: none;
    padding: 0;
    margin-top: 1.2em;
  }
  section.closing ul.loop li {
    font-size: 1.25em;
    margin-bottom: 18px;
    color: #edf2f7;
    padding-left: 28px;
    position: relative;
    line-height: 1.3;
  }
  section.closing ul.loop li::before {
    content: '→';
    position: absolute;
    left: 0;
    color: #90cdf4;
  }
  section.closing .partner-row {
    position: absolute;
    bottom: 48px;
    left: 96px;
    right: 96px;
    display: flex;
    gap: 28px;
    color: #a0aec0;
    font-size: 0.78em;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    border-top: 1px solid #2d3748;
    padding-top: 18px;
  }
---

<!-- Slide 1: The measurable gap -->

# The Philippines has a broadband problem

<div class="subtitle">The World Bank measures it on three axes.</div>

<div class="stat-grid">
  <div class="stat-card">
    <p class="big">33%</p>
    <div class="label">Access</div>
    <div class="context">Household fixed-broadband penetration. Viet Nam 76%. Malaysia 50%.</div>
  </div>
  <div class="stat-card">
    <p class="big">11%</p>
    <div class="label">Affordability</div>
    <div class="context">Fixed broadband as share of GNI per capita. Highest in ASEAN.</div>
  </div>
  <div class="stat-card">
    <p class="big">Low</p>
    <div class="label">Quality</div>
    <div class="context">Median fixed speeds below every major ASEAN peer.</div>
  </div>
</div>

<div class="source">World Bank, "Better Internet for All Filipinos" (January 2024). Ookla (2023, 2025).</div>

<!--
Speaker notes:
The Philippines has a broadband problem. The World Bank measures it on three axes: access, affordability, and quality. Household fixed penetration, 33 percent. Bandwidth, 11 percent of GNI per capita, the highest in ASEAN. Speeds lag every major ASEAN peer.
-->

---

<!-- Slide 2: Why the gap persists -->

# Small ISPs carry the expansion

<div class="subtitle">But the margin structure traps them.</div>

<table class="compare-table">
  <thead>
    <tr>
      <th class="metric">Five-year average, 2017-2022</th>
      <th class="small-isp">Small ISPs</th>
      <th class="duopoly">Globe / PLDT</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td class="metric-name">Revenue growth</td>
      <td class="number small-isp">83%</td>
      <td class="number duopoly">29%</td>
    </tr>
    <tr>
      <td class="metric-name">Net income margin</td>
      <td class="number small-isp">4%</td>
      <td class="number duopoly">14%</td>
    </tr>
    <tr>
      <td class="metric-name">CAPEX as % of revenue</td>
      <td class="number small-isp">17%</td>
      <td class="number duopoly">47%</td>
    </tr>
    <tr>
      <td class="metric-name">Wholesale bandwidth as % of revenue</td>
      <td class="number small-isp">~33%</td>
      <td class="number duopoly">&mdash;</td>
    </tr>
  </tbody>
</table>

<div class="callout">Many small ISPs began as cable TV operators, now running fiber. They can't build faster, cheaper, or better because there's almost no revenue left to reinvest.</div>

<div class="source">World Bank, 2024, based on PSE and SEC financial statements.</div>

<!--
Speaker notes:
Small ISPs carry the expansion. Many began as cable TV operators, now running fiber. Their revenues grew 83 percent over five years. But they earn just 4 percent net margin, reinvest only 17 percent of revenue in CAPEX, and roughly a third of their revenue goes straight to wholesale bandwidth. That's why they can't build faster, cheaper, or better.
-->

---

<!-- Slide 3: The lever -->

# Capability is the lever

<div class="subtitle">Regulatory reform is coming. Capability is controllable today.</div>

<div class="chain">
  <div class="chain-box"><strong>Capability</strong></div>
  <div class="chain-arrow">→</div>
  <div class="chain-box">Peering,<br/>routing security,<br/>IXP participation</div>
  <div class="chain-arrow">→</div>
  <div class="chain-box">Lower<br/>bandwidth<br/>spend</div>
  <div class="chain-arrow">→</div>
  <div class="chain-box">Restored<br/>reinvestment<br/>capacity</div>
  <div class="chain-arrow">→</div>
  <div class="chain-box chain-outcome">Access<br/>Affordability<br/>Quality</div>
</div>

<div class="chain-note">Reinvestment is what moves the three World Bank indicators.</div>

<!--
Speaker notes:
Regulatory reform is coming. In the meantime, capability is the one lever operators themselves control. Peering, routing security, and IXP participation reduce the bandwidth bill directly. That restores reinvestment capacity. And reinvestment is what moves the three World Bank indicators.
-->

---

<!-- Slide 4: IXperience Pro -->

# IXperience Pro

<div class="subtitle">A structured cohort program for provincial Philippine engineers, co-developed with APNIC Academy.</div>

<div class="curriculum">
  <div class="module">
    <div class="num">Module 1</div>
    <div class="name">BGP fundamentals</div>
  </div>
  <div class="module">
    <div class="num">Module 2</div>
    <div class="name">Peering and interconnection</div>
  </div>
  <div class="module">
    <div class="num">Module 3</div>
    <div class="name">Routing security (RPKI / MANRS)</div>
  </div>
  <div class="module">
    <div class="num">Module 4</div>
    <div class="name">IXP operations</div>
  </div>
</div>

<div class="ttt-strip">
  <strong>4 cohorts × 15 engineers = 60 certified.</strong> Train-the-trainer track certifies 4 to 6 Filipino facilitators, so delivery becomes independent of international instructors. All materials publish under Creative Commons.
</div>

<div class="photo-placeholder">
  [ PHOTO PLACEHOLDER: past IXperience workshop, participants in learning mode ]
</div>

<!--
Speaker notes:
IXperience Pro is a structured cohort program for provincial Philippine engineers. Four modules: BGP, peering, routing security, and IXP operations, co-developed with APNIC Academy. Four cohorts of fifteen, sixty engineers from at least twenty ISPs. And a train-the-trainer track that certifies four to six Filipino facilitators, so delivery becomes independent of international instructors.
-->

---

<!-- Slide 5: Not an experiment -->

# Not an experiment

<div class="subtitle">Scaling something already working.</div>

<div class="cred-stats">
  <div class="cred-stat"><div class="num">4</div><div class="label">Prior events</div></div>
  <div class="cred-stat"><div class="num">155</div><div class="label">Companies</div></div>
  <div class="cred-stat"><div class="num">251</div><div class="label">Engineers trained</div></div>
  <div class="cred-stat"><div class="num">71%</div><div class="label">Provincial</div></div>
</div>

<div class="cred-pills">
  <div class="pill"><strong>Curriculum runs on APNIC Academy labs and courseware.</strong> With APNIC and PhNOG as co-delivery partners.</div>
  <div class="pill"><strong>2023 ISIF grant delivered:</strong> Project School Internet. 50+ schools connected in Cebu, contributing to 100,000+ students.</div>
  <div class="pill"><strong>Standing MOA with FICTAP:</strong> RISE serves as the community's designated capability partner for Philippine ISPs.</div>
</div>

<div class="photo-placeholder">
  [ PHOTO PLACEHOLDER: past IXperience participant mosaic ]
</div>

<!--
Speaker notes:
This isn't an experiment. With APNIC and PhNOG, we've trained 251 engineers from 155 companies, seventy-one percent provincial. Curriculum runs on APNIC Academy labs. Our 2023 ISIF grant, Project School Internet, connected over 50 schools in Cebu. And under standing MOA with FICTAP, the fiber ISP trade association, RISE serves as the community's designated capability partner.
-->

---

<!-- _class: closing -->

# The loop

<ul class="loop">
  <li>Filipino engineers trained by Filipino engineers</li>
  <li>Lower bandwidth costs</li>
  <li>Restored reinvestment capacity</li>
  <li>Measurable movement on the indicators the World Bank tracks</li>
</ul>

<div class="partner-row">
  <span>RISE</span>
  <span>APNIC Academy</span>
  <span>PhNOG</span>
  <span>FICTAP</span>
</div>

<!--
Speaker notes:
Filipino engineers trained by Filipino engineers. Lower bandwidth costs. Restored reinvestment capacity. Measurable movement on the indicators the World Bank tracks.
-->
