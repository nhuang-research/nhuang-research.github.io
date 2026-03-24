---
layout: about
title: About
permalink: /
subtitle: <a href='https://people.miami.edu/profile/7abce556c6974d74e71c89fb865e4553' style='color:#F47321;'>University of Miami Herbert Business School</a>

profile:
  align: right
  image: prof_pic.jpg
  image_circular: true # crops the image to make it circular
  more_info: >

news: false # includes a list of news items
selected_papers: false # includes a list of papers marked as "selected={true}"
social: false # includes social icons at the bottom of the page
---

<style>
.nh-spin-wrap {
  position: relative;
  display: inline-block;
  border-radius: 50%;
}
.nh-spin-wrap::before {
  content: '';
  position: absolute;
  inset: -6px;
  border-radius: 50%;
  background: conic-gradient(
    from 0deg,
    #F47321 0deg 60deg,
    transparent 60deg 180deg,
    #005030 180deg 270deg,
    transparent 270deg 360deg
  );
  animation: nhSpin 12s linear infinite;
  z-index: 0;
}
.nh-spin-wrap::after {
  content: '';
  position: absolute;
  inset: -2px;
  border-radius: 50%;
  background: #1a1a1a;
  z-index: 1;
}
.nh-spin-wrap img {
  position: relative;
  z-index: 2;
  display: block;
}
@keyframes nhSpin { to { transform: rotate(360deg); } }

/* ── SUBTITLE LINK COLOR ── */
.page-description a, .post-description a {
  color: #F47321 !important;
}

/* ── NAV ACTIVE + UNDERLINE ── */
.nav-item.active > .nav-link {
  color: #00a060 !important;
}
header.sticky-top {
  border-bottom: 1px solid #00a060 !important;
}

/* ── BOTTOM SECTIONS ── */
.nh-about-bottom {
  --line:     rgba(255,255,255,0.06);
  --line-hi:  rgba(255,255,255,0.12);
  --text:     #aaaaaa;
  --text-hi:  #f0f0f0;
  --text-lo:  #3a3a3a;
  --text-mid: #666;
  --orange:   #F47321;
  --green:    #00a060;
  margin-top: 2rem;
  font-size: 16px;
  overflow-x: hidden;
}

.nh-section {
  border-top: 1px solid var(--line);
  padding-top: 2rem;
  margin-bottom: 0;
  display: grid;
  grid-template-columns: 100px 1fr;
  gap: 4rem;
}

.nh-section-label {
  font-size: 0.85em; font-weight: 500;
  letter-spacing: 0.18em; text-transform: uppercase;
  color: #3a3a3a; padding-top: 0.2rem;
  position: sticky; top: 72px; height: fit-content;
}

/* ── JOURNAL GROUP ── */
.nh-journal-group {
  display: flex; flex-direction: column;
  padding: 0 0 1rem;
  min-width: 0;
}
.nh-desc {
  font-size: 16px; font-weight: 300;
  color: var(--text); line-height: 1.6; padding-bottom: 0.2rem;
  overflow-wrap: anywhere;
}
.nh-desc a { color: var(--green); text-decoration: none; }
.nh-desc a:hover { color: var(--orange); }

.nh-journal-category {
  display: grid;
  grid-template-columns: 160px 1fr;
  gap: 1.5rem; align-items: start;
  padding: 0.85rem 0;
  border-bottom: 1px solid var(--line);
}
.nh-journal-category:first-of-type { border-top: none; }
.nh-journal-category:last-of-type { border-bottom: none;}

.nh-cat-label {
  font-size: 16px; font-weight: 300;
  letter-spacing: 0.05em; color: var(--text-lo);
  padding-top: 0.15rem;
  overflow-wrap: anywhere;
}
.nh-journals { display: flex; flex-direction: column; gap: 0.3rem; min-width: 0; }
.nh-journal-entry {
  font-size: 16px; font-weight: 300; font-style: italic;
  color: var(--text-hi); text-decoration: none; transition: color 0.2s;
  overflow-wrap: anywhere;
}
.nh-journal-entry:hover { color: var(--orange); }

/* ── AWARDS ── */
.nh-awards {
  padding: 0 0 2rem;
  font-size: 16px; font-weight: 300;
  color: var(--text); line-height: 1.6;
}
.nh-awards a { color: var(--green); text-decoration: none; }
.nh-awards a:hover { color: var(--orange); }
.nh-awards em { font-style: italic; }

/* ── CONNECT — same as research page filter-btn ── */
.nh-connect {
  display: flex; flex-wrap: wrap; gap: 0.5rem;
  padding: 0 0 1rem;
}
.nh-connect-btn {
  font-size: 14px; font-weight: 400; letter-spacing: 0.1em;
  text-transform: none !important; padding: 0.4rem 1rem;
  border: 1px solid var(--line); color: var(--text-hi);
  text-decoration: none;
  clip-path: polygon(6px 0%, 100% 0%, calc(100% - 6px) 100%, 0% 100%);
  transition: all 0.2s ease; font-family: inherit;
}
.nh-connect-btn:hover {
  border-color: var(--orange); color: var(--orange);
  background: rgba(244,115,33,0.08);
}

/* ── LOGO ── */
.nh-logo-wrap { padding: 0 0 1rem; }
.nh-logo-wrap img { height: 48px; opacity: 0.7; transition: opacity 0.2s; }
.nh-logo-wrap img:hover { opacity: 1; }

/* ── REVEAL ── */
.nh-reveal { opacity: 0; transform: translateY(14px); transition: opacity 0.65s ease, transform 0.65s ease; }
.nh-reveal.nh-visible { opacity: 1; transform: none; }

/* ── RESPONSIVE ── */
@media (max-width: 760px) {
  .nh-section { grid-template-columns: 1fr; gap: 1rem; padding-top: 2rem; }
  .nh-section-label { position: static; padding-bottom: 0.25rem; }
  .nh-journal-category { grid-template-columns: 1fr; gap: 0.5rem; }
  .nh-journal-group,
  .nh-awards,
  .nh-logo-wrap,
  .nh-connect { min-width: 0; }
  .nh-logo-wrap img { max-width: 100%; height: auto; }
}

@media (max-width: 560px) {
  .nh-section { gap: 0.8rem; }
  .nh-section-label {
    font-size: 0.75rem;
    letter-spacing: 0.14em;
    padding-bottom: 0.15rem;
  }
  .nh-desc,
  .nh-awards,
  .nh-cat-label,
  .nh-journal-entry { font-size: 0.95rem; line-height: 1.5; }
  .nh-journal-category { padding: 0.65rem 0; }
  .nh-connect { gap: 0.45rem; }
  .nh-connect-btn {
    width: 100%;
    text-align: center;
    padding: 0.55rem 0.9rem;
    font-size: 0.78rem;
  }
}
</style>


<script>
(function() {
  function init() {
    var img = document.querySelector('.profile img');
    if (!img || img.parentNode.classList.contains('nh-spin-wrap')) return;
    var wrap = document.createElement('span');
    wrap.className = 'nh-spin-wrap';
    img.parentNode.insertBefore(wrap, img);
    wrap.appendChild(img);
  }
  if (document.readyState === 'loading') {
    document.addEventListener('DOMContentLoaded', init);
  } else {
    init();
  }
})();
</script>

<p> <a href="https://people.miami.edu/profile/nxh558@miami.edu/" style="color:#00a060;"> Nina Huang </a> is the Dennis & Smith Family Endowed Chair Professor of Business Technology at the Miami Herbert Business School, University of Miami, Florida. </p>

<p> Dr. Huang's expertise centers on understanding how digital technology can enhance user experiences and improve business outcomes. Her research program covers a range of digital contexts, including live streaming, online dating, online learning, online healthcare, mobile applications, and digital commerce.</p> 

<p> Nina currently serves as a Senior Editor at <em>Production and Operations Management</em> and an Associate Editor at <em>Information Systems Research</em>. She previously served as the Vice President of INFORMS Information Systems Society from 2023 to 2025 and an Associate Editor at <em>MIS Quarterly</em> from 2021 to 2024.</p>

<!-- ── STYLED BOTTOM SECTIONS ── -->
<div class="nh-about-bottom">

  <!-- RESEARCH OUTPUT -->
  <div class="nh-section nh-reveal">
    <div class="nh-section-label">Research<br>Output</div>
    <div class="nh-journal-group">
      <p class="nh-desc">Dr. Huang's research has been published in premier journals (listed in
        <a href="https://www.ft.com/content/3405a512-5cbb-11e1-8f1f-00144feabdc0" target="_blank">Financial Times Top 50 Journals</a> and
        <a href="https://jsom.utdallas.edu/the-utd-top-100-business-school-research-rankings" target="_blank">UTD24 Journals</a>)
        across multiple disciplines:
      </p>
      <div class="nh-journal-category">
        <span class="nh-cat-label">Interdisciplinary</span>
        <div class="nh-journals">
          <a class="nh-journal-entry" href="https://pubsonline.informs.org/journal/mnsc" target="_blank">Management Science (MS)</a>
        </div>
      </div>
      <div class="nh-journal-category">
        <span class="nh-cat-label">Information Systems</span>
        <div class="nh-journals">
          <a class="nh-journal-entry" href="https://pubsonline.informs.org/journal/isre" target="_blank">Information Systems Research (ISR)</a>
          <a class="nh-journal-entry" href="https://misq.umn.edu" target="_blank">MIS Quarterly (MISQ)</a>
          <a class="nh-journal-entry" href="https://www.jmis-web.org" target="_blank">Journal of Management Information Systems (JMIS)</a>
          <a class="nh-journal-entry" href="https://aisel.aisnet.org/jais/" target="_blank">Journal of the Association for Information Systems (JAIS)</a>
        </div>
      </div>
      <div class="nh-journal-category">
        <span class="nh-cat-label">Operations Management</span>
        <div class="nh-journals">
          <a class="nh-journal-entry" href="https://www.poms.org/journal" target="_blank">Production and Operations Management (POM)</a>
        </div>
      </div>
      <div class="nh-journal-category">
        <span class="nh-cat-label">Marketing</span>
        <div class="nh-journals">
          <a class="nh-journal-entry" href="https://myscp.onlinelibrary.wiley.com/journal/15327663" target="_blank">Journal of Consumer Psychology (JCP)</a>
        </div>
      </div>
    </div>
  </div>

  <!-- AWARDS -->
  <div class="nh-section nh-reveal">
    <div class="nh-section-label">Awards &amp;<br>Recognition</div>
    <div class="nh-awards">
      Nina has received many awards and recognitions, including
      <a href="https://pubsonline.informs.org/do/10.1287/orms.2024.01.25n" target="_blank">a Senior Member of Institute for Operations Research and the Management Sciences (INFORMS)</a>,
      <a href="https://aisnet.org/page/DistinguishedMemberList" target="_blank">a Distinguished Member of the Association for Information Systems (AIS)</a>,
      <a href="https://www.informs.org/Recognizing-Excellence/Community-Prizes/Information-Systems-Society/ISS-Sandra-A.-Slaughter-Early-Career-Award" target="_blank">the INFORMS Sandra A. Slaughter Early Career Award</a>,
      <a href="https://ishistory.aisnet.org/awards/earlycareeraward/" target="_blank">the AIS Early Career Award</a>,
      <a href="https://misq.umn.edu/awards-reviewer" target="_blank">an Outstanding Reviewer of the Year at <em>MIS Quarterly</em></a>, and
      <a href="https://pubsonline.informs.org/page/isre/awards" target="_blank">the Best Reviewer of the Year at <em>Information Systems Research</em></a>.
    </div>
  </div>

  <!-- CONNECT -->
  <div class="nh-section nh-reveal">
    <div class="nh-section-label">Connect</div>
    <div>
      <div class="nh-connect">
        <a class="nh-connect-btn" href="https://www.linkedin.com/in/nina-huang" target="_blank">💼 &nbsp;LinkedIn</a>
        <a class="nh-connect-btn" href="https://scholar.google.com/citations?user=pTNPXbMAAAAJ&hl=en" target="_blank">🎓 &nbsp;Google Scholar</a>
        <a class="nh-connect-btn" href="mailto:nhuang@miami.edu">✉️ &nbsp;Contact Me</a>
      </div>
    </div>
  </div>

</div>

<script>
var reveals = document.querySelectorAll('.nh-reveal');
var obs = new IntersectionObserver(function(e) {
  e.forEach(function(x) {
    if (x.isIntersecting) { x.target.classList.add('nh-visible'); obs.unobserve(x.target); }
  });
}, { threshold: 0.05 });
reveals.forEach(function(r) { obs.observe(r); });
</script>

<!-- ADD LOGO HERE -->
<div style="text-align:left; margin-top:30px; padding-left:5px;">
  <a href="https://www.herbert.miami.edu" target="_blank" rel="noopener">
    <img src="/assets/img/UM-H-BUS-miami Herbert business school-RGB.png" 
         alt="Miami Herbert Business School logo" 
         width="160" 
         style="height:auto; opacity:0.9;">
  </a>
</div>
