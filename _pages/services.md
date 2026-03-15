---
layout: page
permalink: /services/
title: Services
description:
nav: true
nav_order: 3
---

<style>
.nh-research {
  --line: rgba(255,255,255,0.06);
  --line-hi: rgba(255,255,255,0.12);
  --text: #aaaaaa;
  --text-hi: #f0f0f0;
  --text-lo: #3a3a3a;
  --text-mid: #666;
  --orange: #F47321;
  --green-hi: #00a060;
}

.nav-item.active > .nav-link {
  color: #00a060 !important;
}

.nh-section {
  border-top: 1px solid var(--line);
  padding-top: 2rem;
  margin-bottom: 0;
  display: grid;
  grid-template-columns: 100px 1fr;
  gap: 4rem;
}

.nh-section:first-of-type {
  border-top: none;
  padding-top: 0;
}

.nh-section-label {
  font-size: 0.85rem;
  font-weight: 500;
  letter-spacing: 0.18em;
  text-transform: uppercase;
  color: var(--text-lo);
  padding-top: 0.2rem;
  position: sticky;
  top: 72px;
  height: fit-content;
}

.service-list {
  display: flex;
  flex-direction: column;
}

.service-item {
  display: grid;
  grid-template-columns: 44px 1fr auto;
  gap: 1.5rem;
  padding: 1.5rem 0;
  border-bottom: 1px solid var(--line);
  align-items: start;
  position: relative;
  opacity: 0;
  transform: translateY(6px);
  transition: opacity 0.4s ease, transform 0.4s ease, padding-left 0.25s ease;
}

.service-list .service-item:first-child {
  padding-top: 0;
}

.service-item::before {
  content: "";
  position: absolute;
  left: 0;
  top: 0;
  bottom: 0;
  width: 2px;
  background: #F47321;
  transform: scaleY(0);
  transform-origin: top;
  transition: transform 0.3s ease;
}

.service-item:hover {
  padding-left: 12px;
}

.service-item:hover::before {
  transform: scaleY(1);
}

.service-item.nh-visible {
  opacity: 1;
  transform: translateY(0);
}

.service-num {
  font-size: 0.8rem;
  font-weight: 500;
  letter-spacing: 0.06em;
  color: var(--text-lo);
  padding-top: 4px;
  transition: color 0.2s;
}

.service-item:hover .service-num {
  color: #F47321;
}

.service-body {
  display: flex;
  flex-direction: column;
  gap: 0.35rem;
}

.service-title {
  font-size: 1rem;
  font-weight: 400;
  color: var(--text-hi);
  line-height: 1.5;
}

.service-title a {
  color: inherit;
  text-decoration: none;
  transition: color 0.2s;
}

.service-title a:hover {
  color: #00a060;
}

.service-meta {
  display: flex;
  align-items: center;
  gap: 0.75rem;
  flex-wrap: wrap;
  margin-top: 0.15rem;
}

.service-role {
  font-size: 0.8rem;
  font-weight: 300;
  color: var(--text-mid);
  line-height: 1.5;
}

.service-year {
  font-size: 0.9rem;
  font-weight: 300;
  color: var(--text-lo);
  letter-spacing: 0.05em;
}

.service-badge {
  font-size: 0.75rem;
  font-weight: 500;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  color: var(--text-hi);
  white-space: nowrap;
  padding-top: 3px;
  text-align: right;
  transition: color 0.2s;
}

.service-item:hover .service-badge {
  color: var(--orange);
}

.nh-reveal {
  opacity: 0;
  transform: translateY(14px);
  transition: opacity 0.65s ease, transform 0.65s ease;
}

.nh-reveal.nh-visible {
  opacity: 1;
  transform: none;
}

@media (max-width: 760px) {
  .nh-section {
    grid-template-columns: 1fr;
    gap: 1.25rem;
  }

  .nh-section-label {
    position: static;
  }

  .service-item {
    grid-template-columns: 32px 1fr;
  }

  .service-badge {
    display: none;
  }
}
</style>

<div class="nh-research">
  <div class="nh-section nh-reveal">
    <div class="nh-section-label">Journal<br>Editorial Service</div>
    <div class="service-list">
      <div class="service-item">
        <span class="service-num">01</span>
        <div class="service-body">
          <div class="service-title">Senior Editor, <a href="https://www.poms.org/pomjournal/departments/dpit" target="_blank"><em>Production and Operations Management</em></a></div>
          <div class="service-meta">
            <span class="service-year">February 2024-</span>
          </div>
        </div>
        <span class="service-badge">POM</span>
      </div>

      <div class="service-item">
        <span class="service-num">02</span>
        <div class="service-body">
          <div class="service-title">Associate Editor, <a href="https://pubsonline.informs.org/page/isre/editorial-board" target="_blank"><em>Information Systems Research</em></a></div>
          <div class="service-meta">
            <span class="service-year">January 2025-</span>
          </div>
        </div>
        <span class="service-badge">ISR</span>
      </div>

      <div class="service-item">
        <span class="service-num">03</span>
        <div class="service-body">
          <div class="service-title">Guest Associate Editor, <a href="https://misq.umn.edu/call-for-papers-ai-ia" target="_blank"><em>Information Systems Research</em> Special Issue on Compassionate Artificial Intelligence</a></div>
          <div class="service-meta">
            <span class="service-year">January 2026-</span>
          </div>
        </div>
        <span class="service-badge">ISR</span>
      </div>

      <div class="service-item">
        <span class="service-num">04</span>
        <div class="service-body">
          <div class="service-title">Guest Associate Editor, <em>MIS Quarterly</em> Special Issue on Artificial Intelligence-Information Assurance Nexus</div>
          <div class="service-meta">
            <span class="service-year">November 2024-</span>
          </div>
        </div>
        <span class="service-badge">MISQ</span>
      </div>

      <div class="service-item">
        <span class="service-num">05</span>
        <div class="service-body">
          <div class="service-title">Associate Editor, <a href="https://misq.org/board" target="_blank"><em>MIS Quarterly</em></a></div>
          <div class="service-meta">
            <span class="service-year">January 2021-December 2024</span>
          </div>
        </div>
        <span class="service-badge">MISQ</span>
      </div>

      <div class="service-item">
        <span class="service-num">06</span>
        <div class="service-body">
          <div class="service-title">Co-Editor, <a href="http://poms.org/cfp_POM_SI_ResDataScience.pdf" target="_blank"><em>Production and Operations Management</em> Special Issue on Responsible Data Science</a></div>
          <div class="service-meta">
            <span class="service-year">August 2022</span>
          </div>
        </div>
        <span class="service-badge">POM</span>
      </div>

      <div class="service-item">
        <span class="service-num">07</span>
        <div class="service-body">
          <div class="service-title">Guest Associate Editor, <a href="https://misq.org/skin/frontend/default/misq/pdf/CurrentCalls/DigitalResilience.pdf" target="_blank"><em>MIS Quarterly</em> Special Issue on Digital Resilience</a></div>
          <div class="service-meta">
            <span class="service-year">November 2020-March 2022</span>
          </div>
        </div>
        <span class="service-badge">MISQ</span>
      </div>

      <div class="service-item">
        <span class="service-num">08</span>
        <div class="service-body">
          <div class="service-title">Guest Senior Editor, <a href="https://www.poms.org/sites/default/files/callforpapers/POM%20Social%20Technology%20special%20issue.pdf" target="_blank"><em>Production and Operations Management</em> Special Issue on Social Technologies in Operations</a></div>
          <div class="service-meta">
            <span class="service-year">January 2022-May 2023</span>
          </div>
        </div>
        <span class="service-badge">POM</span>
      </div>

      <div class="service-item">
        <span class="service-num">09</span>
        <div class="service-body">
          <div class="service-title">Co-Editor, <a href="https://www.emeraldgrouppublishing.com/journal/intr/bright-side-and-dark-side-digital-health" target="_blank"><em>Internet Research</em> Special Issue on the Bright Side and the Dark Side of Digital Health</a></div>
          <div class="service-meta">
            <span class="service-year">February 2020-December 2021</span>
          </div>
        </div>
        <span class="service-badge">INTR</span>
      </div>
    </div>
  </div>

  <div class="nh-section nh-reveal" style="padding-bottom: 4rem;">
    <div class="nh-section-label">Conference<br>Service</div>
    <div class="service-list">
      <div class="service-item">
        <span class="service-num">01</span>
        <div class="service-body">
          <div class="service-title">Mentor &amp; Competition Winner, <a href="https://aisel.aisnet.org/icis" target="_blank">International Conference on Information Systems (ICIS)</a> Paper-A-Thon</div>
          <div class="service-meta">
            <span class="service-year">2025</span>
          </div>
        </div>
        <span class="service-badge">ICIS</span>
      </div>

      <div class="service-item">
        <span class="service-num">02</span>
        <div class="service-body">
          <div class="service-title">Track Co-chair, User Behavior, Engagement, and Consequences, <a href="https://aisel.aisnet.org/icis" target="_blank">ICIS</a></div>
          <div class="service-meta">
            <span class="service-year">2024, 2023, 2021</span>
          </div>
        </div>
        <span class="service-badge">ICIS</span>
      </div>

      <div class="service-item">
        <span class="service-num">03</span>
        <div class="service-body">
          <div class="service-title">Session Chair, User Behavior in Online Platforms, <a href="https://aisel.aisnet.org/icis" target="_blank">ICIS</a></div>
          <div class="service-meta">
            <span class="service-year">2020</span>
          </div>
        </div>
        <span class="service-badge">ICIS</span>
      </div>

      <div class="service-item">
        <span class="service-num">04</span>
        <div class="service-body">
          <div class="service-title">Associate Editor, User Behaviors, User Engagement, and Consequences Track, <a href="https://aisel.aisnet.org/icis" target="_blank">ICIS</a></div>
          <div class="service-meta">
            <span class="service-year">2020</span>
          </div>
        </div>
        <span class="service-badge">ICIS</span>
      </div>

      <div class="service-item">
        <span class="service-num">05</span>
        <div class="service-body">
          <div class="service-title">Associate Editor, Economics and IS Track, <a href="https://aisel.aisnet.org/icis" target="_blank">ICIS</a></div>
          <div class="service-meta">
            <span class="service-year">2019</span>
          </div>
        </div>
        <span class="service-badge">ICIS</span>
      </div>

      <div class="service-item">
        <span class="service-num">06</span>
        <div class="service-body">
          <div class="service-title">Cluster Co-chair, IS Cluster, <a href="https://www.informs.org/Meetings-Conferences" target="_blank">INFORMS Annual Meeting</a></div>
          <div class="service-meta">
            <span class="service-year">2022, 2021</span>
          </div>
        </div>
        <span class="service-badge">INFORMS</span>
      </div>

      <div class="service-item">
        <span class="service-num">07</span>
        <div class="service-body">
          <div class="service-title">Program Committee Member, Conference on Information Systems and Technology (CIST)</div>
          <div class="service-meta">
            <span class="service-year">2022, 2019, 2018</span>
          </div>
        </div>
        <span class="service-badge">CIST</span>
      </div>

      <div class="service-item">
        <span class="service-num">08</span>
        <div class="service-body">
          <div class="service-title">Session Chair, Digital Platform Design, <a href="https://www.informs.org/Meetings-Conferences" target="_blank">INFORMS Annual Meeting</a></div>
          <div class="service-meta">
            <span class="service-year">2020</span>
          </div>
        </div>
        <span class="service-badge">INFORMS</span>
      </div>

      <div class="service-item">
        <span class="service-num">09</span>
        <div class="service-body">
          <div class="service-title">Session Chair, <a href="https://www.informs.org/Meetings-Conferences" target="_blank">INFORMS Annual Meeting</a></div>
          <div class="service-meta">
            <span class="service-year">2019, 2018</span>
          </div>
        </div>
        <span class="service-badge">INFORMS</span>
      </div>

      <div class="service-item">
        <span class="service-num">10</span>
        <div class="service-body">
          <div class="service-title">Session Chair, Information Systems and Operations Management Track, <a href="https://www.poms.org/conferences" target="_blank">POMS Annual Conference</a></div>
          <div class="service-meta">
            <span class="service-year">2024, 2018</span>
          </div>
        </div>
        <span class="service-badge">POMS</span>
      </div>

      <div class="service-item">
        <span class="service-num">11</span>
        <div class="service-body">
          <div class="service-title">Co-chair, Crowd-based Platform Mini-track, <a href="https://hicss.hawaii.edu/" target="_blank">Hawaii International Conference on System Sciences (HICSS)</a></div>
          <div class="service-meta">
            <span class="service-year">2026, 2025, 2024, 2023, 2022, 2021, 2020, 2019, 2018</span>
          </div>
        </div>
        <span class="service-badge">HICSS</span>
      </div>

      <div class="service-item">
        <span class="service-num">12</span>
        <div class="service-body">
          <div class="service-title">Mentor, 2nd INFORMS-ISS ISR Paper Development Workshop for Early Career Scholars</div>
          <div class="service-meta">
            <span class="service-year">2025</span>
          </div>
        </div>
        <span class="service-badge">Workshop</span>
      </div>

      <div class="service-item">
        <span class="service-num">13</span>
        <div class="service-body">
          <div class="service-title">Co-Chair, Inaugural INFORMS Information Systems Society Doctoral Consortium</div>
          <div class="service-meta">
            <span class="service-year">2024</span>
          </div>
        </div>
        <span class="service-badge">Consortium</span>
      </div>

      <div class="service-item">
        <span class="service-num">14</span>
        <div class="service-body">
          <div class="service-title">Conference Co-chair, China Summer Workshop on Information Management</div>
          <div class="service-meta">
            <span class="service-year">2023</span>
          </div>
        </div>
        <span class="service-badge">Workshop</span>
      </div>

      <div class="service-item">
        <span class="service-num">15</span>
        <div class="service-body">
          <div class="service-title">Mentor, IS Student Presentations Over the Cloud Series, New York University</div>
          <div class="service-meta">
            <span class="service-year">2023</span>
          </div>
        </div>
        <span class="service-badge">Workshop</span>
      </div>

      <div class="service-item">
        <span class="service-num">16</span>
        <div class="service-body">
          <div class="service-title">Mentor and Panelist, AIS SIG DITE Paper Development Workshop on Digital Innovation, Transformation, and Entrepreneurship</div>
          <div class="service-meta">
            <span class="service-year">2023</span>
          </div>
        </div>
        <span class="service-badge">Workshop</span>
      </div>

      <div class="service-item">
        <span class="service-num">17</span>
        <div class="service-body">
          <div class="service-title">Mentor, AMCIS Doctoral Consortium for Early Students</div>
          <div class="service-meta">
            <span class="service-year">2021</span>
          </div>
        </div>
        <span class="service-badge">AMCIS</span>
      </div>

      <div class="service-item">
        <span class="service-num">18</span>
        <div class="service-body">
          <div class="service-title">Session Chair, Information Technology/Information Systems Track, Decision Sciences Institute Annual Conference</div>
          <div class="service-meta">
            <span class="service-year">2021</span>
          </div>
        </div>
        <span class="service-badge">DSI</span>
      </div>

      <div class="service-item">
        <span class="service-num">19</span>
        <div class="service-body">
          <div class="service-title">Associate Editor, Business Analytics and Big Data Track, European Conference on Information Systems</div>
          <div class="service-meta">
            <span class="service-year">2019</span>
          </div>
        </div>
        <span class="service-badge">ECIS</span>
      </div>

      <div class="service-item">
        <span class="service-num">20</span>
        <div class="service-body">
          <div class="service-title">Discussant, Workshop on Experimental and Behavioral Economics in Information Systems</div>
          <div class="service-meta">
            <span class="service-year">2019</span>
          </div>
        </div>
        <span class="service-badge">WEBEIS</span>
      </div>
    </div>
  </div>
</div>

<script>
document.addEventListener("DOMContentLoaded", function () {
  const revealItems = document.querySelectorAll(".nh-reveal, .service-item");

  const observer = new IntersectionObserver(
    (entries) => {
      entries.forEach((entry) => {
        if (entry.isIntersecting) {
          entry.target.classList.add("nh-visible");
          observer.unobserve(entry.target);
        }
      });
    },
    { threshold: 0.08 }
  );

  revealItems.forEach((item, index) => {
    item.style.transitionDelay = `${index * 25}ms`;
    observer.observe(item);
  });
});
</script>
