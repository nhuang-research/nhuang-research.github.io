---
layout: page
permalink: /talks/
title: Talks
description:
nav: true
nav_order: 2
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

.pub-list {
  display: flex;
  flex-direction: column;
}

.pub-item {
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

.pub-item:first-child {
  border-top: 1px solid var(--line);
}

.pub-item::before {
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

.pub-item:hover {
  padding-left: 12px;
}

.pub-item:hover::before {
  transform: scaleY(1);
}

.pub-item.nh-visible {
  opacity: 1;
  transform: translateY(0);
}

.pub-num {
  font-size: 0.8rem;
  font-weight: 500;
  letter-spacing: 0.06em;
  color: var(--text-lo);
  padding-top: 4px;
  transition: color 0.2s;
}

.pub-item:hover .pub-num {
  color: #F47321;
}

.pub-body {
  display: flex;
  flex-direction: column;
  gap: 0.35rem;
}

.pub-title {
  font-size: 1rem;
  font-weight: 400;
  color: var(--text-hi);
  line-height: 1.5;
  text-decoration: none;
  transition: color 0.2s;
}

.pub-title:hover {
  color: #00a060;
}

.pub-meta {
  display: flex;
  align-items: center;
  gap: 0.75rem;
  flex-wrap: wrap;
  margin-top: 0.15rem;
}

.pub-journal {
  font-size: 0.85rem;
  font-weight: 300;
  color: var(--text-mid);
  line-height: 1.5;
}

.pub-year {
  font-size: 0.9rem;
  font-weight: 300;
  color: var(--text-lo);
  letter-spacing: 0.05em;
}

.pub-badge {
  width: 76px;
  min-width: 76px;
  padding-top: 3px;
  display: flex;
  justify-content: center;
  align-items: flex-start;
}

.talk-logo {
  display: block;
  width: 58px;
  height: 40px;
  object-fit: contain;
  padding: 0;
  background: transparent;
  transition: transform 0.2s ease;
}

.talk-logo.logo-wide {
  width: 66px;
}

.talk-logo.logo-wide-md {
  width: 62px;
}

.talk-logo.logo-wide-plus {
  width: 72px;
}

.talk-logo.logo-wide-lg {
  width: 66px;
}

.talk-logo.logo-wide-xl {
  width: 70px;
}

.talk-logo.logo-wide-2xl {
  width: 74px;
}

.talk-logo.logo-wide-3xl {
  width: 78px;
}

.talk-logo.logo-wide-4xl {
  width: 82px;
}

.talk-logo.logo-square {
  width: 50px;
}

.talk-logo.logo-square-md {
  width: 54px;
}

.talk-logo.logo-square-lg {
  width: 58px;
}

.talk-logo.logo-square-xl {
  width: 62px;
}

.talk-logo.logo-square-2xl {
  width: 66px;
}

.talk-logo.logo-square-3xl {
  width: 70px;
}

.talk-logo.logo-square-4xl {
  width: 74px;
}

.talk-logo.logo-square-sm {
  width: 46px;
}

.pub-item:hover .talk-logo {
  transform: translateY(-1px);
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

  .pub-item {
    grid-template-columns: 32px 1fr;
  }

  .pub-badge {
    display: none;
  }
}
</style>

<div class="nh-research">
  <div class="nh-section nh-reveal" style="padding-bottom: 4rem;">
    <div class="nh-section-label">Invited<br>Talks</div>
    <div class="pub-list">
      <div class="pub-item">
        <span class="pub-num">01</span>
        <div class="pub-body">
          <a class="pub-title" href="https://freeman.tulane.edu//" target="_blank">A.B. Freeman School of Business, Tulane University</a>
          <div class="pub-meta">
            <span class="pub-year">April 2026</span>
          </div>
        </div>
        <span class="pub-badge" data-logo-label="Tulane University" data-logo-src="/assets/img/talk-logos/tulane.png"></span>
      </div>

      <div class="pub-item">
        <span class="pub-num">02</span>
        <div class="pub-body">
          <a class="pub-title" href="https://www.depts.ttu.edu/rawlsbusiness//" target="_blank">Rawls College of Business, Texas Tech University</a>
          <div class="pub-meta">
            <span class="pub-year">December 2025</span>
          </div>
        </div>
        <span class="pub-badge" data-logo-label="Texas Tech University" data-logo-src="/assets/img/talk-logos/texas-tech.png"></span>
      </div>

      <div class="pub-item">
        <span class="pub-num">03</span>
        <div class="pub-body">
          <a class="pub-title" href="https://fisher.osu.edu///" target="_blank">Fisher College of Business, Ohio State University</a>
          <div class="pub-meta">
            <span class="pub-year">November 2025</span>
          </div>
        </div>
        <span class="pub-badge" data-logo-label="Ohio State University" data-logo-src="/assets/img/talk-logos/ohio-state.png"></span>
      </div>

      <div class="pub-item">
        <span class="pub-num">04</span>
        <div class="pub-body">
          <a class="pub-title" href="https://www.bu.edu/questrom///" target="_blank">Questrom School of Business, Boston University</a>
          <div class="pub-meta">
            <span class="pub-year">October 2025</span>
          </div>
        </div>
        <span class="pub-badge" data-logo-label="Boston University" data-logo-class="logo-wide" data-logo-src="/assets/img/talk-logos/boston-university.png"></span>
      </div>

      <div class="pub-item">
        <span class="pub-num">05</span>
        <div class="pub-body">
          <a class="pub-title" href="https://english.ckgsb.edu.cn/" target="_blank">Cheung Kong Graduate School of Business</a>
          <div class="pub-meta">
            <span class="pub-year">June 2025</span>
          </div>
        </div>
        <span class="pub-badge" data-logo-label="Cheung Kong Graduate School of Business" data-logo-class="logo-wide" data-logo-src="/assets/img/talk-logos/ckgsb.png"></span>
      </div>

      <div class="pub-item">
        <span class="pub-num">06</span>
        <div class="pub-body">
          <a class="pub-title" href="https://www.kellogg.northwestern.edu/" target="_blank">Kellogg School of Management, Northwestern University</a>
          <div class="pub-meta">
            <span class="pub-year">May 2025</span>
          </div>
        </div>
        <span class="pub-badge" data-logo-label="Northwestern University" data-logo-src="/assets/img/talk-logos/northwestern.png"></span>
      </div>

      <div class="pub-item">
        <span class="pub-num">07</span>
        <div class="pub-body">
          <a class="pub-title" href="https://www.smeal.psu.edu/" target="_blank">Smeal College of Business, Pennsylvania State University</a>
          <div class="pub-meta">
            <span class="pub-year">April 2025</span>
          </div>
        </div>
        <span class="pub-badge" data-logo-label="Pennsylvania State University" data-logo-src="/assets/img/talk-logos/penn-state.png"></span>
      </div>

      <div class="pub-item">
        <span class="pub-num">08</span>
        <div class="pub-body">
          <a class="pub-title" href="https://www.mccombs.utexas.edu/" target="_blank">McCombs School of Business, University of Texas at Austin</a>
          <div class="pub-meta">
            <span class="pub-year">November 2024</span>
          </div>
        </div>
        <span class="pub-badge" data-logo-label="University of Texas at Austin" data-logo-src="/assets/img/talk-logos/texas-austin.png"></span>
      </div>

      <div class="pub-item">
        <span class="pub-num">09</span>
        <div class="pub-body">
          <a class="pub-title" href="https://www.marshall.usc.edu/" target="_blank">Marshall School of Business, University of Southern California</a>
          <div class="pub-meta">
            <span class="pub-year">November 2024, February 2025</span>
          </div>
        </div>
        <span class="pub-badge" data-logo-label="University of Southern California" data-logo-src="/assets/img/talk-logos/usc.png"></span>
      </div>

      <div class="pub-item">
        <span class="pub-num">10</span>
        <div class="pub-body">
          <a class="pub-title" href="https://www.unibocconi.it/en" target="_blank">School of Management, Bocconi University, Italy</a>
          <div class="pub-meta">
            <span class="pub-year">May 2023</span>
          </div>
        </div>
        <span class="pub-badge" data-logo-label="Bocconi University" data-logo-class="logo-wide" data-logo-src="/assets/img/talk-logos/bocconi.svg"></span>
      </div>

      <div class="pub-item">
        <span class="pub-num">11</span>
        <div class="pub-body">
          <a class="pub-title" href="https://business.gmu.edu/" target="_blank">School of Business, George Mason University</a>
          <div class="pub-meta">
            <span class="pub-year">April 2023</span>
          </div>
        </div>
        <span class="pub-badge" data-logo-label="George Mason University" data-logo-class="logo-wide" data-logo-src="/assets/img/talk-logos/george-mason.png"></span>
      </div>

      <div class="pub-item">
        <span class="pub-num">12</span>
        <div class="pub-body">
          <a class="pub-title" href="https://warrington.ufl.edu/" target="_blank">Warrington College of Business, University of Florida</a>
          <div class="pub-meta">
            <span class="pub-year">April 2023</span>
          </div>
        </div>
        <span class="pub-badge" data-logo-label="University of Florida" data-logo-src="/assets/img/talk-logos/florida.png"></span>
      </div>

      <div class="pub-item">
        <span class="pub-num">13</span>
        <div class="pub-body">
          <a class="pub-title" href="https://www.simon.rochester.edu/" target="_blank">Simon Business School, University of Rochester</a>
          <div class="pub-meta">
            <span class="pub-year">March 2023</span>
          </div>
        </div>
        <span class="pub-badge" data-logo-label="University of Rochester" data-logo-class="logo-wide" data-logo-src="/assets/img/talk-logos/rochester.png"></span>
      </div>

      <div class="pub-item">
        <span class="pub-num">14</span>
        <div class="pub-body">
          <a class="pub-title" href="https://www.business.rutgers.edu/" target="_blank">Rutgers Business School, Rutgers, The State University of New Jersey</a>
          <div class="pub-meta">
            <span class="pub-year">October 2022</span>
          </div>
        </div>
        <span class="pub-badge" data-logo-label="Rutgers University" data-logo-src="/assets/img/talk-logos/rutgers.png"></span>
      </div>

      <div class="pub-item">
        <span class="pub-num">15</span>
        <div class="pub-body">
          <a class="pub-title" href="http://en.som.zju.edu.cn/" target="_blank">School of Management, Zhejiang University</a>
          <div class="pub-meta">
            <span class="pub-year">September 2022</span>
          </div>
        </div>
        <span class="pub-badge" data-logo-label="Zhejiang University" data-logo-class="logo-wide" data-logo-src="/assets/img/talk-logos/zhejiang.png"></span>
      </div>

      <div class="pub-item">
        <span class="pub-num">16</span>
        <div class="pub-body">
          <a class="pub-title" href="https://herbert.miami.edu/" target="_blank">Miami Herbert Business School, University of Miami</a>
          <div class="pub-meta">
            <span class="pub-year">November 2021</span>
          </div>
        </div>
        <span class="pub-badge" data-logo-label="University of Miami" data-logo-src="/assets/img/talk-logos/miami.png"></span>
      </div>

      <div class="pub-item">
        <span class="pub-num">17</span>
        <div class="pub-body">
          <a class="pub-title" href="https://zicklin.baruch.cuny.edu/" target="_blank">Baruch College, City University of New York</a>
          <div class="pub-meta">
            <span class="pub-year">September 2021</span>
          </div>
        </div>
        <span class="pub-badge" data-logo-label="City University of New York" data-logo-class="logo-square" data-logo-src="/assets/img/talk-logos/cuny.png"></span>
      </div>

      <div class="pub-item">
        <span class="pub-num">18</span>
        <div class="pub-body">
          <a class="pub-title" href="https://giesbusiness.illinois.edu/" target="_blank">Gies College of Business, University of Illinois at Urbana-Champaign</a>
          <div class="pub-meta">
            <span class="pub-year">July 2021</span>
          </div>
        </div>
        <span class="pub-badge" data-logo-label="University of Illinois Urbana-Champaign" data-logo-src="/assets/img/talk-logos/illinois.png"></span>
      </div>

      <div class="pub-item">
        <span class="pub-num">19</span>
        <div class="pub-body">
          <a class="pub-title" href="https://www.fdsm.fudan.edu.cn/" target="_blank">School of Management, Fudan University</a>
          <div class="pub-meta">
            <span class="pub-year">March 2021</span>
          </div>
        </div>
        <span class="pub-badge" data-logo-label="Fudan University" data-logo-class="logo-square" data-logo-src="/assets/img/talk-logos/fudan.svg"></span>
      </div>

      <div class="pub-item">
        <span class="pub-num">20</span>
        <div class="pub-body">
          <a class="pub-title" href="https://kelley.iu.edu/" target="_blank">Kelley School of Business, Indiana University</a>
          <div class="pub-meta">
            <span class="pub-year">June 2020</span>
          </div>
        </div>
        <span class="pub-badge" data-logo-label="Indiana University" data-logo-src="/assets/img/talk-logos/indiana.png"></span>
      </div>

      <div class="pub-item">
        <span class="pub-num">21</span>
        <div class="pub-body">
          <a class="pub-title" href="https://www.bauer.uh.edu/" target="_blank">C.T. Bauer College of Business, University of Houston</a>
          <div class="pub-meta">
            <span class="pub-year">March 2020</span>
          </div>
        </div>
        <span class="pub-badge" data-logo-label="University of Houston" data-logo-src="/assets/img/talk-logos/houston.png"></span>
      </div>

      <div class="pub-item">
        <span class="pub-num">22</span>
        <div class="pub-body">
          <a class="pub-title" href="https://www.sem.tsinghua.edu.cn/" target="_blank">School of Economics and Management, Tsinghua University</a>
          <div class="pub-meta">
            <span class="pub-year">July 2019</span>
          </div>
        </div>
        <span class="pub-badge" data-logo-label="Tsinghua University" data-logo-class="logo-square-sm" data-logo-src="/assets/img/talk-logos/tsinghua.png"></span>
      </div>

      <div class="pub-item">
        <span class="pub-num">23</span>
        <div class="pub-body">
          <a class="pub-title" href="https://www.polyu.edu.hk/en/fb/" target="_blank">Faculty of Business, Hong Kong Polytechnic University</a>
          <div class="pub-meta">
            <span class="pub-year">June 2019</span>
          </div>
        </div>
        <span class="pub-badge" data-logo-label="Hong Kong Polytechnic University" data-logo-class="logo-wide-plus" data-logo-src="/assets/img/talk-logos/hk-polyu.png"></span>
      </div>

      <div class="pub-item">
        <span class="pub-num">24</span>
        <div class="pub-body">
          <a class="pub-title" href="https://www.lsu.edu/business/" target="_blank">EJ Ourso College of Business, Louisiana State University</a>
          <div class="pub-meta">
            <span class="pub-year">March 2019</span>
          </div>
        </div>
        <span class="pub-badge" data-logo-label="Louisiana State University" data-logo-class="logo-wide-3xl" data-logo-src="/assets/img/talk-logos/lsu.png"></span>
      </div>

      <div class="pub-item">
        <span class="pub-num">25</span>
        <div class="pub-body">
          <a class="pub-title" href="https://www.bentley.edu/graduate/mccallum-graduate-school-business" target="_blank">McCallum Graduate School of Business, Bentley University</a>
          <div class="pub-meta">
            <span class="pub-year">May 2018</span>
          </div>
        </div>
        <span class="pub-badge" data-logo-label="Bentley University" data-logo-class="logo-square-4xl" data-logo-src="/assets/img/talk-logos/bentley.png"></span>
      </div>

      <div class="pub-item">
        <span class="pub-num">26</span>
        <div class="pub-body">
          <a class="pub-title" href="https://wpcarey.asu.edu/" target="_blank">W. P. Carey School of Business, Arizona State University</a>
          <div class="pub-meta">
            <span class="pub-year">January 2017</span>
          </div>
        </div>
        <span class="pub-badge" data-logo-label="Arizona State University" data-logo-class="logo-wide-4xl" data-logo-src="/assets/img/talk-logos/asu.png"></span>
      </div>

      <div class="pub-item">
        <span class="pub-num">27</span>
        <div class="pub-body">
          <a class="pub-title" href="http://netinst.org/" target="_blank">NET Institute, New York University</a>
          <div class="pub-meta">
            <span class="pub-year">November 2015</span>
          </div>
        </div>
        <span class="pub-badge" data-logo-label="New York University" data-logo-class="logo-wide-plus" data-logo-src="/assets/img/talk-logos/nyu.png"></span>
      </div>
    </div>
  </div>
</div>

<script>
document.addEventListener("DOMContentLoaded", function () {
  const revealItems = document.querySelectorAll(".nh-reveal, .pub-item");
  const logoService = "https://www.google.com/s2/favicons?sz=512&domain_url=";
  const preferredIconPaths = [
    "/favicon.svg",
    "/icon.svg",
    "/logo.svg",
    "/safari-pinned-tab.svg",
    "/apple-touch-icon.png",
    "/apple-touch-icon-precomposed.png",
    "/android-chrome-512x512.png",
    "/android-chrome-192x192.png",
    "/mstile-310x310.png",
    "/favicon-512x512.png",
    "/favicon-196x196.png",
    "/favicon-192x192.png",
    "/favicon-180x180.png",
    "/favicon-152x152.png",
    "/favicon-144x144.png",
    "/favicon-128x128.png",
    "/favicon-96x96.png",
    "/favicon.png",
    "/favicon.ico"
  ];

  document.querySelectorAll(".pub-item").forEach((item) => {
    const link = item.querySelector(".pub-title");
    const badge = item.querySelector(".pub-badge");
    if (!link || !badge) return;

    const img = document.createElement("img");
    img.className = "talk-logo";
    img.alt = `${badge.dataset.logoLabel || link.textContent.trim()} logo`;
    img.loading = "lazy";
    img.decoding = "async";
    img.referrerPolicy = "no-referrer";
    if (badge.dataset.logoClass) {
      img.classList.add(...badge.dataset.logoClass.split(" ").filter(Boolean));
    }

    let origin;
    try {
      const url = new URL(link.href);
      origin = `${url.protocol === "https:" ? "https:" : "http:"}//${url.host}`;
    } catch (err) {
      origin = link.href;
    }

    const preferredSource = badge.dataset.logoSrc;
    const preferredDomain = badge.dataset.logoDomain || origin;
    const candidates = preferredSource
      ? [preferredSource]
      : [
          ...preferredIconPaths.map((path) => `${preferredDomain}${path}`),
          `${logoService}${encodeURIComponent(preferredDomain)}`
        ];

    let candidateIndex = 0;
    const tryNextLogo = () => {
      if (candidateIndex >= candidates.length) return;
      img.src = candidates[candidateIndex];
      candidateIndex += 1;
    };

    img.onerror = () => {
      tryNextLogo();
    };

    tryNextLogo();

    badge.replaceChildren(img);
  });

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
