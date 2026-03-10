---
layout: page
permalink: /research/
title: Research
description: 
nav: true
nav_order: 1
---

<style>

/* ── RESEARCH WRAPPER ── */
.nh-research {
  --line:      rgba(255,255,255,0.06);
  --line-hi:   rgba(255,255,255,0.12);
  --text:      #aaaaaa;
  --text-hi:   #f0f0f0;
  --text-lo:   #3a3a3a;
  --text-mid:  #666;
  --orange:    #F47321;
  --green-hi:  #00a060;
}

/* ── SECTION ── */
.nh-section {
  border-top: 1px solid var(--line);
  padding-top: 3.5rem;
  margin-bottom: 0;
  display: grid;
  grid-template-columns: 100px 1fr;
  gap: 4rem;
}
.nh-section:first-of-type { border-top: none; }
.nh-section-label {
  font-size: 0.75rem; font-weight: 500;
  letter-spacing: 0.18em; text-transform: uppercase;
  color: var(--text-lo); padding-top: 0.2rem;
  position: sticky; top: 72px; height: fit-content;
}

/* ── RESEARCH AREAS ── */
.area-grid {
  display: flex; flex-wrap: wrap; gap: 0.5rem;
  padding: 1rem 0 1.5rem;
}
.area-tag {
  font-size: 0.85rem; font-weight: 300; letter-spacing: 0.06em;
  padding: 0.5rem 1.1rem;
  border: 1px solid var(--line);
  color: #ffffff;
  background: transparent;
  clip-path: polygon(6px 0%, 100% 0%, calc(100% - 6px) 100%, 0% 100%);
  transition: all 0.2s ease; cursor: none;
  user-select: none;
}
.area-tag:hover {
  border-color: #F47321;
  color: #F47321;
  background: rgba(244,115,33,0.06);
}

/* ── FILTER BAR ── */
.filter-bar {
  display: flex; align-items: center; gap: 0.5rem;
  flex-wrap: wrap; padding: 3rem 0 2rem;
}
.filter-btn {
  font-size: 0.68rem; font-weight: 400; letter-spacing: 0.1em;
  text-transform: uppercase; padding: 0.4rem 1rem;
  border: 1px solid var(--line); color: var(--text-lo);
  background: transparent; cursor: none;
  clip-path: polygon(6px 0%, 100% 0%, calc(100% - 6px) 100%, 0% 100%);
  transition: all 0.2s ease; font-family: inherit;
}
.filter-btn:hover { border-color: var(--line-hi); color: var(--text); }
.filter-btn.active {
  border-color: #F47321; color: #F47321;
  background: rgba(244,115,33,0.08);
}
.filter-count {
  font-size: 0.62rem; color: var(--text-lo);
  margin-left: auto; letter-spacing: 0.08em; font-weight: 300;
}

/* ── PUB LIST ── */
.pub-list { display: flex; flex-direction: column; }

.pub-item {
  display: grid;
  grid-template-columns: 44px 1fr auto;
  gap: 1.5rem;
  padding: 1.5rem 0;
  border-bottom: 1px solid var(--line);
  align-items: start;
  transition: padding-left 0.25s ease;
  position: relative;
  opacity: 0; transform: translateY(6px);
  transition: opacity 0.4s ease, transform 0.4s ease, padding-left 0.25s ease;
}
.pub-item:first-child { border-top: 1px solid var(--line); }
.pub-item::before {
  content: ''; position: absolute;
  left: 0; top: 0; bottom: 0;
  width: 2px; background: #F47321;
  transform: scaleY(0); transform-origin: top;
  transition: transform 0.3s ease;
}
.pub-item:hover { padding-left: 12px; }
.pub-item:hover::before { transform: scaleY(1); }
.pub-item.nh-visible { opacity: 1; transform: translateY(0); }
.pub-item.hidden { display: none; }

.pub-num {
  font-size: 0.72rem; font-weight: 500; letter-spacing: 0.06em;
  color: var(--text-lo); padding-top: 4px; transition: color 0.2s;
}
.pub-item:hover .pub-num { color: #F47321; }

.pub-body { display: flex; flex-direction: column; gap: 0.35rem; }

.pub-title {
  font-size: 0.9rem; font-weight: 400; color: var(--text-hi);
  line-height: 1.5; text-decoration: none; transition: color 0.2s;
}
.pub-title:hover { color: #8cc4de; }

.pub-authors {
  font-size: 0.78rem; font-weight: 300; color: var(--text-mid); line-height: 1.5;
}
.pub-authors strong { color: var(--text); font-weight: 400; }

.pub-meta {
  display: flex; align-items: center; gap: 0.75rem;
  flex-wrap: wrap; margin-top: 0.15rem;
}
.pub-journal {
  font-size: 0.7rem; font-weight: 300; font-style: italic; color: var(--text-mid);
}
.pub-year {
  font-size: 0.65rem; font-weight: 300; color: var(--text-lo); letter-spacing: 0.05em;
}
.pub-note {
  font-size: 0.6rem; font-weight: 500; letter-spacing: 0.1em;
  text-transform: uppercase; color: var(--green-hi);
  border: 1px solid rgba(0,160,96,0.3);
  padding: 0.1rem 0.5rem;
  clip-path: polygon(4px 0%, 100% 0%, calc(100% - 4px) 100%, 0% 100%);
}
.pub-badge {
  font-size: 0.68rem; font-weight: 500; letter-spacing: 0.1em;
  color: var(--text-lo); white-space: nowrap;
  padding-top: 3px; transition: color 0.2s; text-align: right;
}
.pub-item:hover .pub-badge { color: var(--text-mid); }

/* ── REVEAL ── */
.nh-reveal { opacity: 0; transform: translateY(14px); transition: opacity 0.65s ease, transform 0.65s ease; }
.nh-reveal.nh-visible { opacity: 1; transform: none; }

/* ── RESPONSIVE ── */
@media (max-width: 760px) {
  .nh-section { grid-template-columns: 1fr; gap: 1.25rem; }
  .nh-section-label { position: static; }
  .pub-item { grid-template-columns: 32px 1fr; }
  .pub-badge { display: none; }
}
</style>

<div class="nh-research">

  <!-- RESEARCH AREAS -->
  <div class="nh-section nh-reveal">
    <div class="nh-section-label">Research<br>Areas</div>
    <div class="area-grid">
      <div class="area-tag">Human-AI Interaction</div>
      <div class="area-tag">Workflow Automation</div>
      <div class="area-tag">Digital Content Platform</div>
      <div class="area-tag">Online Matching Platforms</div>
      <div class="area-tag">Online Healthcare</div>
      <div class="area-tag">Future of Work</div>
      <div class="area-tag">Social Media Analytics</div>
      <div class="area-tag">Online Commerce</div>
    </div>
  </div>

  <!-- PUBLICATIONS -->
  <div class="nh-section nh-reveal" style="padding-bottom:4rem;">
    <div class="nh-section-label">Selected<br>Publications</div>
    <div>

      <div class="filter-bar">
        <button class="filter-btn active" data-filter="all">All</button>
        <button class="filter-btn" data-filter="ISR">ISR</button>
        <button class="filter-btn" data-filter="MISQ">MISQ</button>
        <button class="filter-btn" data-filter="MS">MS</button>
        <button class="filter-btn" data-filter="POM">POM</button>
        <button class="filter-btn" data-filter="other">Other</button>
        <span class="filter-count" id="filterCount">25 papers</span>
      </div>

      <div class="pub-list" id="pubList">

        <div class="pub-item" data-journal="ISR">
          <span class="pub-num">01</span>
          <div class="pub-body">
            <a class="pub-title" href="https://pubsonline.informs.org/doi/10.1287/isre.2024.1551" target="_blank">Workflow Automation in Open-Source Software Development: Accelerating Innovation through Mechanization and Orchestration</a>
            <div class="pub-authors">Huang A, <strong>Huang N</strong>, Hong Y</div>
            <div class="pub-meta">
              <span class="pub-journal">Information Systems Research</span>
              <span class="pub-year">2026</span>
              <span class="pub-note">Forthcoming</span>
            </div>
          </div>
          <span class="pub-badge">ISR</span>
        </div>

        <div class="pub-item" data-journal="MISQ">
          <span class="pub-num">02</span>
          <div class="pub-body">
            <a class="pub-title" href="https://misq.umn.edu/misq/article-abstract/doi/10.25300/MISQ/2025/18603/3258/What-Happens-When-Machines-Become-Smarter-An" target="_blank">What Happens When Machines Become Smarter? An Empirical Investigation of Artificial Intelligence (AI) Opponents in Online Gaming</a>
            <div class="pub-authors">Yuan H, He Q, Wang L, <strong>Huang N</strong>, Wei Q, Zhang J</div>
            <div class="pub-meta">
              <span class="pub-journal">MIS Quarterly</span>
              <span class="pub-year">2026</span>
              <span class="pub-note">Forthcoming</span>
            </div>
          </div>
          <span class="pub-badge">MISQ</span>
        </div>

        <div class="pub-item" data-journal="MS">
          <span class="pub-num">03</span>
          <div class="pub-body">
            <a class="pub-title" href="https://pubsonline.informs.org/doi/10.1287/mnsc.2021.03495" target="_blank">Evaluating the Efficacy of Application Costs for Managing Congestion in Online Matching Market</a>
            <div class="pub-authors"><strong>Huang N</strong>, Burtch G, Chen P, Huang A</div>
            <div class="pub-meta">
              <span class="pub-journal">Management Science</span>
              <span class="pub-year">2026</span>
              <span class="pub-note">Forthcoming</span>
            </div>
          </div>
          <span class="pub-badge">MS</span>
        </div>

        <div class="pub-item" data-journal="ISR">
          <span class="pub-num">04</span>
          <div class="pub-body">
            <a class="pub-title" href="https://pubsonline.informs.org/doi/abs/10.1287/isre.2022.0402" target="_blank">Forced to Change? Media Exposure of Labor Issues and Firm Artificial Intelligence (AI) Investment</a>
            <div class="pub-authors">Li B, <strong>Huang N</strong>, Shi W</div>
            <div class="pub-meta">
              <span class="pub-journal">Information Systems Research</span>
              <span class="pub-year">2026</span>
              <span class="pub-note">Forthcoming</span>
            </div>
          </div>
          <span class="pub-badge">ISR</span>
        </div>

        <div class="pub-item" data-journal="MISQ">
          <span class="pub-num">05</span>
          <div class="pub-body">
            <a class="pub-title" href="https://misq.umn.edu/misq/article-abstract/49/4/1567/3274/Real-Time-Sales-Data-Streamer-Improvisation-and" target="_blank">Real-Time Sales Data, Streamer Improvisation, and Sales Performance: Evidence From Live Stream Selling</a>
            <div class="pub-authors">He Y, <strong>Huang N</strong>, Wang L, Sun Y</div>
            <div class="pub-meta">
              <span class="pub-journal">MIS Quarterly</span>
              <span class="pub-year">2025</span>
              <span class="pub-year">49(4):1567–1594</span>
            </div>
          </div>
          <span class="pub-badge">MISQ</span>
        </div>

        <div class="pub-item" data-journal="ISR">
          <span class="pub-num">06</span>
          <div class="pub-body">
            <a class="pub-title" href="https://pubsonline.informs.org/doi/10.1287/isre.2023.0103" target="_blank">Artificial Intelligence (AI) Assistant in Online Shopping: A Randomized Field Experiment on a Livestream Selling Platform</a>
            <div class="pub-authors">Wang L, <strong>Huang N</strong>, He Y, Liu D, Guo X, Sun Y, Chen G</div>
            <div class="pub-meta">
              <span class="pub-journal">Information Systems Research</span>
              <span class="pub-year">2025</span>
              <span class="pub-year">36(4):2358–2374</span>
            </div>
          </div>
          <span class="pub-badge">ISR</span>
        </div>

        <div class="pub-item" data-journal="other">
          <span class="pub-num">07</span>
          <div class="pub-body">
            <a class="pub-title" href="https://dl.acm.org/doi/10.1145/3736418" target="_blank">Mining Linguistic Styles in Bilateral Matching: A Contrastive Learning Approach to Reciprocal Recommendation</a>
            <div class="pub-authors">Guan Y, He Y, <strong>Huang N</strong>, Guo X, Chen G</div>
            <div class="pub-meta">
              <span class="pub-journal">ACM Transactions on Knowledge Discovery from Data</span>
              <span class="pub-year">2025</span>
              <span class="pub-year">19(6):1–25</span>
            </div>
          </div>
          <span class="pub-badge">TKDD</span>
        </div>

        <div class="pub-item" data-journal="ISR">
          <span class="pub-num">08</span>
          <div class="pub-body">
            <a class="pub-title" href="https://pubsonline.informs.org/doi/10.1287/isre.2021.0379" target="_blank">Enhancing User Privacy Through Ephemeral Sharing Design: Experimental Evidence from the Online Dating Context</a>
            <div class="pub-authors">He Y, Xu X, <strong>Huang N</strong>, Hong Y, Liu D</div>
            <div class="pub-meta">
              <span class="pub-journal">Information Systems Research</span>
              <span class="pub-year">2024</span>
              <span class="pub-year">36(1):162–183</span>
            </div>
          </div>
          <span class="pub-badge">ISR</span>
        </div>

        <div class="pub-item" data-journal="other">
          <span class="pub-num">09</span>
          <div class="pub-body">
            <a class="pub-title" href="https://www.tandfonline.com/doi/full/10.1080/07421222.2024.2415767" target="_blank">How to Translate Firm-Generated Content to Sales? Evidence from Online Healthcare Platforms</a>
            <div class="pub-authors">Qiao W, <strong>Huang N</strong>, Yan Z</div>
            <div class="pub-meta">
              <span class="pub-journal">Journal of Management Information Systems</span>
              <span class="pub-year">2024</span>
              <span class="pub-year">41(4):1173–1197</span>
            </div>
          </div>
          <span class="pub-badge">JMIS</span>
        </div>

        <div class="pub-item" data-journal="ISR">
          <span class="pub-num">10</span>
          <div class="pub-body">
            <a class="pub-title" href="https://pubsonline.informs.org/doi/full/10.1287/isre.2023.1234" target="_blank">When the Clock Strikes: A Multimethod Investigation of On-the-Hour Effects in Online Learning</a>
            <div class="pub-authors"><strong>Huang N</strong>, Wang L, Hong Y, Lin L, Guo X, Chen G</div>
            <div class="pub-meta">
              <span class="pub-journal">Information Systems Research</span>
              <span class="pub-year">2023</span>
              <span class="pub-year">35(2):766–782</span>
            </div>
          </div>
          <span class="pub-badge">ISR</span>
        </div>

        <div class="pub-item" data-journal="POM">
          <span class="pub-num">11</span>
          <div class="pub-body">
            <a class="pub-title" href="https://onlinelibrary.wiley.com/doi/10.1111/poms.13953" target="_blank">Voice-based AI in Call Center Customer Service: A Natural Field Experiment</a>
            <div class="pub-authors">Wang L, <strong>Huang N</strong>, Hong Y, Liu L, Guo X, Chen G</div>
            <div class="pub-meta">
              <span class="pub-journal">Production and Operations Management</span>
              <span class="pub-year">2023</span>
              <span class="pub-year">32(4):1002–1018</span>
            </div>
          </div>
          <span class="pub-badge">POM</span>
        </div>

        <div class="pub-item" data-journal="ISR">
          <span class="pub-num">12</span>
          <div class="pub-body">
            <a class="pub-title" href="https://pubsonline.informs.org/doi/10.1287/isre.2022.1148" target="_blank">Managing Congestion in a Matching Market via Demand Information Disclosure</a>
            <div class="pub-authors"><strong>Huang N</strong>, Burtch G, He Y, Hong Y</div>
            <div class="pub-meta">
              <span class="pub-journal">Information Systems Research</span>
              <span class="pub-year">2022</span>
              <span class="pub-year">33(4):1196–1220</span>
            </div>
          </div>
          <span class="pub-badge">ISR</span>
        </div>

        <div class="pub-item" data-journal="MISQ">
          <span class="pub-num">13</span>
          <div class="pub-body">
            <a class="pub-title" href="https://misq.umn.edu/misq/downloads/download/editorial/759/" target="_blank">Causality Meets Diversity in Information Systems Research</a>
            <div class="pub-authors">Mithas S, Xue L, <strong>Huang N</strong>, Burton-Jones A</div>
            <div class="pub-meta">
              <span class="pub-journal">MIS Quarterly</span>
              <span class="pub-year">2022</span>
              <span class="pub-year">46(3):i–xvii</span>
            </div>
          </div>
          <span class="pub-badge">MISQ</span>
        </div>

        <div class="pub-item" data-journal="POM">
          <span class="pub-num">14</span>
          <div class="pub-body">
            <a class="pub-title" href="https://onlinelibrary.wiley.com/doi/abs/10.1111/poms.13381" target="_blank">Effects of Online-Offline Service Integration on e-Healthcare Providers: A Quasi-Natural Experiment</a>
            <div class="pub-authors"><strong>Huang N</strong>, Yan Z, Yin H</div>
            <div class="pub-meta">
              <span class="pub-journal">Production and Operations Management</span>
              <span class="pub-year">2021</span>
              <span class="pub-year">30(8):2359–2378</span>
            </div>
          </div>
          <span class="pub-badge">POM</span>
        </div>

        <div class="pub-item" data-journal="ISR">
          <span class="pub-num">15</span>
          <div class="pub-body">
            <a class="pub-title" href="https://pubsonline.informs.org/doi/10.1287/isre.2021.1003" target="_blank">Just DM Me (Politely): Direct Messaging, Politeness, and Hiring Outcomes in Online Labor Markets</a>
            <div class="pub-authors">Hong Y, Peng J, Burtch G, <strong>Huang N</strong></div>
            <div class="pub-meta">
              <span class="pub-journal">Information Systems Research</span>
              <span class="pub-year">2021</span>
              <span class="pub-year">32(3):786–800</span>
            </div>
          </div>
          <span class="pub-badge">ISR</span>
        </div>

        <div class="pub-item" data-journal="ISR">
          <span class="pub-num">16</span>
          <div class="pub-body">
            <a class="pub-title" href="https://pubsonline.informs.org/doi/10.1287/isre.2021.0999" target="_blank">Not Registered? Please Sign Up First: A Randomized Field Experiment on the Ex Ante Registration Request</a>
            <div class="pub-authors"><strong>Huang N</strong>, Mojumder P, Sun T, Lv J, Golden J</div>
            <div class="pub-meta">
              <span class="pub-journal">Information Systems Research</span>
              <span class="pub-year">2021</span>
              <span class="pub-year">32(3):914–931</span>
            </div>
          </div>
          <span class="pub-badge">ISR</span>
        </div>

        <div class="pub-item" data-journal="ISR">
          <span class="pub-num">17</span>
          <div class="pub-body">
            <a class="pub-title" href="https://pubsonline.informs.org/doi/abs/10.1287/isre.2020.0974" target="_blank">Combating Procrastination on Massive Online Open Courses via Optimal Calls to Action</a>
            <div class="pub-authors"><strong>Huang N</strong>, Zhang J, Burtch G, Li X, Chen P</div>
            <div class="pub-meta">
              <span class="pub-journal">Information Systems Research</span>
              <span class="pub-year">2020</span>
              <span class="pub-year">32(2):301–316</span>
            </div>
          </div>
          <span class="pub-badge">ISR</span>
        </div>

        <div class="pub-item" data-journal="MISQ">
          <span class="pub-num">18</span>
          <div class="pub-body">
            <a class="pub-title" href="https://misq.umn.edu/designing-promotional-incentives-to-embrace-social-sharing-evidence-from-field-and-online-experiments.html" target="_blank">Designing Promotion Incentive to Embrace Social Sharing: Evidence from Field and Online Experiments</a>
            <div class="pub-authors">Sun T, Viswanathan S, <strong>Huang N</strong>, Zheleva E</div>
            <div class="pub-meta">
              <span class="pub-journal">MIS Quarterly</span>
              <span class="pub-year">2020</span>
              <span class="pub-year">45(2):789–820</span>
            </div>
          </div>
          <span class="pub-badge">MISQ</span>
        </div>

        <div class="pub-item" data-journal="ISR">
          <span class="pub-num">19</span>
          <div class="pub-body">
            <a class="pub-title" href="https://pubsonline.informs.org/doi/abs/10.1287/isre.2019.0896" target="_blank">Unemployment and Worker Participation in the Gig Economy: Evidence from an Online Labor Market</a>
            <div class="pub-authors"><strong>Huang N</strong>, Burtch G, Hong Y, Pavlou PA</div>
            <div class="pub-meta">
              <span class="pub-journal">Information Systems Research</span>
              <span class="pub-year">2020</span>
              <span class="pub-year">31(2):431–448</span>
            </div>
          </div>
          <span class="pub-badge">ISR</span>
        </div>

        <div class="pub-item" data-journal="ISR">
          <span class="pub-num">20</span>
          <div class="pub-body">
            <a class="pub-title" href="https://pubsonline.informs.org/doi/abs/10.1287/isre.2018.0832" target="_blank">Word-of-Mouth System Implementation and Customer Conversion: A Randomized Field Experiment</a>
            <div class="pub-authors"><strong>Huang N</strong>, Sun T, Chen P, Golden J</div>
            <div class="pub-meta">
              <span class="pub-journal">Information Systems Research</span>
              <span class="pub-year">2019</span>
              <span class="pub-year">30(3):711–1105</span>
            </div>
          </div>
          <span class="pub-badge">ISR</span>
        </div>

        <div class="pub-item" data-journal="MS">
          <span class="pub-num">21</span>
          <div class="pub-body">
            <a class="pub-title" href="https://pubsonline.informs.org/doi/10.1287/mnsc.2017.2944" target="_blank">Motivating User-Generated Content with Performance Feedback: Evidence from Randomized Field Experiments</a>
            <div class="pub-authors"><strong>Huang N</strong>, Burtch G, Gu B, Hong Y, Liang C, Wang K, Fu D, Yang B</div>
            <div class="pub-meta">
              <span class="pub-journal">Management Science</span>
              <span class="pub-year">2019</span>
              <span class="pub-year">65(1):327–345</span>
            </div>
          </div>
          <span class="pub-badge">MS</span>
        </div>

        <div class="pub-item" data-journal="other">
          <span class="pub-num">22</span>
          <div class="pub-body">
            <a class="pub-title" href="https://www.tandfonline.com/doi/abs/10.1080/07421222.2018.1550564" target="_blank">Spillover Effects of Financial Incentives on User Engagement: Evidence From an Online Knowledge Exchange Platform</a>
            <div class="pub-authors">Kuang L, <strong>Huang N</strong>, Hong Y, Yan Z</div>
            <div class="pub-meta">
              <span class="pub-journal">Journal of Management Information Systems</span>
              <span class="pub-year">2019</span>
              <span class="pub-year">36(1):289–320</span>
            </div>
          </div>
          <span class="pub-badge">JMIS</span>
        </div>

        <div class="pub-item" data-journal="MISQ">
          <span class="pub-num">23</span>
          <div class="pub-body">
            <a class="pub-title" href="https://misq.org/social-network-integration-and-user-content-generation-evidence-from-natural-experiments.html" target="_blank">Social Network Integration and User Content Generation: Evidence from Natural Experiments</a>
            <div class="pub-authors"><strong>Huang N</strong>, Hong Y, Burtch G</div>
            <div class="pub-meta">
              <span class="pub-journal">MIS Quarterly</span>
              <span class="pub-year">2017</span>
              <span class="pub-year">41(4):1035–1058</span>
            </div>
          </div>
          <span class="pub-badge">MISQ</span>
        </div>

        <div class="pub-item" data-journal="other">
          <span class="pub-num">24</span>
          <div class="pub-body">
            <a class="pub-title" href="http://aisel.aisnet.org/jais/vol17/iss11/2/" target="_blank">Culture, Conformity and Emotional Suppression in Online Reviews</a>
            <div class="pub-authors">Hong Y, <strong>Huang N</strong>, Burtch G, Li C</div>
            <div class="pub-meta">
              <span class="pub-journal">Journal of the Association for Information Systems</span>
              <span class="pub-year">2016</span>
              <span class="pub-year">17(11):308–329</span>
            </div>
          </div>
          <span class="pub-badge">JAIS</span>
        </div>

        <div class="pub-item" data-journal="other">
          <span class="pub-num">25</span>
          <div class="pub-body">
            <a class="pub-title" href="https://doi.org/10.1016/j.jcps.2016.03.001" target="_blank">Effects of Multiple Psychological Distances on Construal and Consumer Evaluation: A Field Study of Online Reviews</a>
            <div class="pub-authors"><strong>Huang N</strong>, Burtch G, Hong Y, Polman E</div>
            <div class="pub-meta">
              <span class="pub-journal">Journal of Consumer Psychology</span>
              <span class="pub-year">2016</span>
              <span class="pub-year">26(4):474–482</span>
            </div>
          </div>
          <span class="pub-badge">JCP</span>
        </div>

      </div><!-- end pub-list -->
    </div>
  </div>

</div><!-- end nh-research -->

<script>
// Cursor
var nhCursor = document.getElementById('nhCursor');
var nhRing = document.getElementById('nhCursorRing');
document.addEventListener('mousemove', function(e) {
  nhCursor.style.left = e.clientX + 'px';
  nhCursor.style.top = e.clientY + 'px';
  nhRing.style.left = e.clientX + 'px';
  nhRing.style.top = e.clientY + 'px';
});
document.querySelectorAll('a, button, .area-tag').forEach(function(el) {
  el.addEventListener('mouseenter', function() {
    nhCursor.style.width = '14px'; nhCursor.style.height = '14px';
    nhRing.style.width = '44px'; nhRing.style.height = '44px';
  });
  el.addEventListener('mouseleave', function() {
    nhCursor.style.width = '8px'; nhCursor.style.height = '8px';
    nhRing.style.width = '32px'; nhRing.style.height = '32px';
  });
});

// Scroll reveal
var reveals = document.querySelectorAll('.nh-reveal');
var obs = new IntersectionObserver(function(e) {
  e.forEach(function(x) {
    if (x.isIntersecting) { x.target.classList.add('nh-visible'); obs.unobserve(x.target); }
  });
}, { threshold: 0.05 });
reveals.forEach(function(r) { obs.observe(r); });

// Stagger pub items
var items = document.querySelectorAll('.pub-item');
var po = new IntersectionObserver(function(entries) {
  if (entries[0].isIntersecting) {
    var visible = Array.from(items).filter(function(i) { return !i.classList.contains('hidden'); });
    visible.forEach(function(item, i) {
      setTimeout(function() { item.classList.add('nh-visible'); }, i * 45);
    });
    po.disconnect();
  }
}, { threshold: 0.02 });
po.observe(document.getElementById('pubList'));

// Filter
var filterBtns = document.querySelectorAll('.filter-btn');
var filterCount = document.getElementById('filterCount');
filterBtns.forEach(function(btn) {
  btn.addEventListener('click', function() {
    filterBtns.forEach(function(b) { b.classList.remove('active'); });
    btn.classList.add('active');
    var f = btn.dataset.filter;
    var count = 0;
    items.forEach(function(item) {
      var show = f === 'all' || item.dataset.journal === f;
      item.classList.toggle('hidden', !show);
      if (show) { item.classList.remove('nh-visible'); count++; }
    });
    filterCount.textContent = count + ' paper' + (count !== 1 ? 's' : '');
    setTimeout(function() {
      Array.from(items).filter(function(i) { return !i.classList.contains('hidden'); })
        .forEach(function(item, i) {
          setTimeout(function() { item.classList.add('nh-visible'); }, i * 40);
        });
    }, 30);
  });
});
</script>
