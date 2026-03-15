---
layout: page
permalink: /media/
title: Media
description:
nav: true
nav_order: 4
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
  <div class="nh-section nh-reveal" style="padding-bottom: 4rem;">
    <div class="nh-section-label">Media Mentions<br>&amp; Reports</div>
    <div class="service-list">
      <div class="service-item">
        <span class="service-num">01</span>
        <div class="service-body">
          <div class="service-title"><a href="https://app.sciencesays.com/p/ask-users-to-register-at-the-start-not-the-end" target="_blank">Ask Users to Register at the Start (Not the End)</a></div>
          <div class="service-meta">
            <span class="service-role"><em>Science Says</em></span>
            <span class="service-year">January 27, 2026</span>
          </div>
        </div>
        <span class="service-badge"></span>
      </div>

      <div class="service-item">
        <span class="service-num">02</span>
        <div class="service-body">
          <div class="service-title"><a href="https://news.miami.edu/miamiherbert/stories/2025/10/how-livestream-sellers-turn-data-into-split-second-decisions.html" target="_blank">How Livestream Sellers Turn Data into Split-Second Decisions</a></div>
          <div class="service-meta">
            <span class="service-role"><em>News@TheU, University of Miami</em></span>
            <span class="service-year">October 8, 2025</span>
          </div>
        </div>
        <span class="service-badge"></span>
      </div>

      <div class="service-item">
        <span class="service-num">03</span>
        <div class="service-body">
          <div class="service-title"><a href="https://news.miami.edu/stories/2025/08/ai-assistant-for-online-shopping.html" target="_blank">AI Assistant for Online Shopping</a></div>
          <div class="service-meta">
            <span class="service-role"><em>News@TheU, University of Miami</em></span>
            <span class="service-year">August 12, 2025</span>
          </div>
        </div>
        <span class="service-badge"></span>
      </div>

      <div class="service-item">
        <span class="service-num">04</span>
        <div class="service-body">
          <div class="service-title"><a href="https://news.miami.edu/stories/2025/06/labor-feeling-the-squeeze-from-ais-advance.html" target="_blank">Labor Feeling the Squeeze From AI’s Advance</a></div>
          <div class="service-meta">
            <span class="service-role"><em>News@TheU, University of Miami</em></span>
            <span class="service-year">June 11, 2025</span>
          </div>
        </div>
        <span class="service-badge"></span>
      </div>

      <div class="service-item">
        <span class="service-num">05</span>
        <div class="service-body">
          <div class="service-title"><a href="https://www.futurity.org/disappearing-photos-dating-apps-3203092-2/?utm_source=rss&utm_medium=rss&utm_campaign=disappearing-photos-dating-apps-3203092-2" target="_blank">Disappearing Photos Increase Dating App Matches</a></div>
          <div class="service-meta">
            <span class="service-role"><em>Futurity</em></span>
            <span class="service-year">April 5, 2024</span>
          </div>
        </div>
        <span class="service-badge"></span>
      </div>

      <div class="service-item">
        <span class="service-num">06</span>
        <div class="service-body">
          <div class="service-title"><a href="https://www.eurekalert.org/news-releases/1040017" target="_blank">Study: Vanishing Photos Make Dating App Matches Multiply</a></div>
          <div class="service-meta">
            <span class="service-role"><em>EurekAlert!, Science News Releases</em></span>
            <span class="service-year">April 3, 2024</span>
          </div>
        </div>
        <span class="service-badge"></span>
      </div>

      <div class="service-item">
        <span class="service-num">07</span>
        <div class="service-body">
          <div class="service-title"><a href="https://phys.org/news/2024-04-photos-dating-app.html" target="_blank">Study: Vanishing Photos Make Dating App Matches Multiply</a></div>
          <div class="service-meta">
            <span class="service-role"><em>Phys.org, Science X</em></span>
            <span class="service-year">April 3, 2024</span>
          </div>
        </div>
        <span class="service-badge"></span>
      </div>

      <div class="service-item">
        <span class="service-num">08</span>
        <div class="service-body">
          <div class="service-title"><a href="https://news.miami.edu/miamiherbert/stories/2023/08/miami-herbert-professors-shine-in-global-information-systems-rankings.html" target="_blank">Miami Herbert Professors Shine in Global Information Systems Rankings</a></div>
          <div class="service-meta">
            <span class="service-role"><em>Miami Herbert Stories, University of Miami Herbert Business School</em></span>
            <span class="service-year">August 8, 2023</span>
          </div>
        </div>
        <span class="service-badge"></span>
      </div>

      <div class="service-item">
        <span class="service-num">09</span>
        <div class="service-body">
          <div class="service-title"><a href="https://www.businessinsider.com/recession-outlook-laid-off-workers-turn-to-gig-work-2023-1" target="_blank">Get Ready for a Gig-Worker Boom That Could Make It Harder for Contractors to Earn a Living</a></div>
          <div class="service-meta">
            <span class="service-role"><em>Business Insider, Insider Inc.</em></span>
            <span class="service-year">January 22, 2023</span>
          </div>
        </div>
        <span class="service-badge"></span>
      </div>

      <div class="service-item">
        <span class="service-num">10</span>
        <div class="service-body">
          <div class="service-title"><a href="https://poetsandquantsforundergrads.com/news/2022-best-undergraduate-professors-nina-ni-huang-university-of-miami-herbert-business-school/" target="_blank">2022 Best Undergraduate Professors: Nina (Ni) Huang, University of Miami Herbert Business School</a></div>
          <div class="service-meta">
            <span class="service-role"><em>Poets&amp;Quants for Undergrads, Poets&amp;Quants</em></span>
            <span class="service-year">December 11, 2022</span>
          </div>
        </div>
        <span class="service-badge"></span>
      </div>

      <div class="service-item">
        <span class="service-num">11</span>
        <div class="service-body">
          <div class="service-title"><a href="https://open.spotify.com/episode/2ztG1Ird6LCmTNFf4YdRfp?si=409b886f89b146e0" target="_blank">Causality Meets Diversity</a></div>
          <div class="service-meta">
            <span class="service-role"><em>This IS Research Podcast, Spotify</em></span>
            <span class="service-year">November 23, 2022</span>
          </div>
        </div>
        <span class="service-badge"></span>
      </div>

      <div class="service-item">
        <span class="service-num">12</span>
        <div class="service-body">
          <div class="service-title"><a href="https://news.miami.edu/stories/2022/08/university-researchers-help-level-the-playing-field-of-online-dating.html" target="_blank">University Researchers Help Level the Playing Field of Online Dating</a></div>
          <div class="service-meta">
            <span class="service-role"><em>News@TheU, University of Miami</em></span>
            <span class="service-year">August 25, 2022</span>
          </div>
        </div>
        <span class="service-badge"></span>
      </div>

      <div class="service-item">
        <span class="service-num">13</span>
        <div class="service-body">
          <div class="service-title"><a href="https://www.bauer.uh.edu/news/2021/bauer-professor-recognized-by-information-systems-society/?utm_source=bauer.uh.edu&utm_medium=referral&utm_campaign=Homepage+Latest+News" target="_blank">Bauer Professor Recognized by Information Systems Society</a></div>
          <div class="service-meta">
            <span class="service-role"><em>UH Today, University of Houston</em></span>
            <span class="service-year">December 8, 2021</span>
          </div>
        </div>
        <span class="service-badge"></span>
      </div>

      <div class="service-item">
        <span class="service-num">14</span>
        <div class="service-body">
          <div class="service-title"><a href="https://www.houstonpublicmedia.org/articles/shows/bauer-business-focus/2021/02/22/391996/online-shopping-register-purchase-repeat/" target="_blank">Online Shopping: Register. Purchase. Repeat.</a></div>
          <div class="service-meta">
            <span class="service-role"><em>Bauer Business Focus, Houston Public Media</em></span>
            <span class="service-year">February 22, 2021</span>
          </div>
        </div>
        <span class="service-badge"></span>
      </div>

      <div class="service-item">
        <span class="service-num">15</span>
        <div class="service-body">
          <div class="service-title"><a href="https://wpcareymagazine.com/issue/autumn-2020/words-to-sell-by-word-of-mouth-systems-can-raise-online-profits/" target="_blank">Words to Sell By: Word-of-Mouth Systems Can Raise Online Profits</a></div>
          <div class="service-meta">
            <span class="service-role"><em>W. P. Carey Magazine, Arizona State University</em></span>
            <span class="service-year">2020</span>
          </div>
        </div>
        <span class="service-badge"></span>
      </div>

      <div class="service-item">
        <span class="service-num">16</span>
        <div class="service-body">
          <div class="service-title"><a href="https://cloudapps.uh.edu/sendit/w/dTQKORPHoei6cuJWjexjjw/YnMQUW1VLUcjNrID5m0zPA/K7tlW4BPkWTFGLrAjYkerg" target="_blank">Bauer Researcher Examines Effectiveness of Promotional Incentives</a></div>
          <div class="service-meta">
            <span class="service-role"><em>University of Houston</em></span>
            <span class="service-year">2020</span>
          </div>
        </div>
        <span class="service-badge"></span>
      </div>

      <div class="service-item">
        <span class="service-num">17</span>
        <div class="service-body">
          <div class="service-title"><a href="https://asunow.asu.edu/20170913-discoveries-how-can-apps-get-users-generate-content-asu-study-finds-gender-differences" target="_blank">How Can Apps Get Users to Generate Content? ASU Study Finds Gender Differences</a></div>
          <div class="service-meta">
            <span class="service-role"><em>Arizona State University</em></span>
            <span class="service-year">2017</span>
          </div>
        </div>
        <span class="service-badge"></span>
      </div>

      <div class="service-item">
        <span class="service-num">18</span>
        <div class="service-body">
          <div class="service-title"><a href="https://asunow.asu.edu/20170307-discoveries-posting-yelp-reviews-facebook-changes-their-nature-asu-study-shows" target="_blank">Posting Yelp Reviews to Facebook Changes Their Nature, ASU Study Shows</a></div>
          <div class="service-meta">
            <span class="service-role"><em>Arizona State University</em></span>
            <span class="service-year">2017</span>
          </div>
        </div>
        <span class="service-badge"></span>
      </div>

      <div class="service-item">
        <span class="service-num">19</span>
        <div class="service-body">
          <div class="service-title"><a href="http://www.dinero.com/opinion/columnistas/articulo/como-saber-si-es-falso-u-original-pregunte-a-los-reviewers-por-maria-gonzalez/231308" target="_blank">How Can You Tell if It Is Fake or Original? Ask the Reviewers</a></div>
          <div class="service-meta">
            <span class="service-role"><em>Publicaciones Semana S.A.</em></span>
            <span class="service-year">2016</span>
          </div>
        </div>
        <span class="service-badge"></span>
      </div>

      <div class="service-item">
        <span class="service-num">20</span>
        <div class="service-body">
          <div class="service-title"><a href="https://www.sciencedaily.com/releases/2016/05/160511080731.htm" target="_blank">How to Boost Online Ratings</a></div>
          <div class="service-meta">
            <span class="service-role"><em>Society for Consumer Psychology</em></span>
            <span class="service-year">2016</span>
          </div>
        </div>
        <span class="service-badge"></span>
      </div>

      <div class="service-item">
        <span class="service-num">21</span>
        <div class="service-body">
          <div class="service-title"><a href="http://zeenews.india.com/news/net-news/long-wait-for-feedback-can-boost-service-ratings-online_1884161.html" target="_blank">Long Wait for Feedback Can Boost Service Ratings Online</a></div>
          <div class="service-meta">
            <span class="service-role"><em>Zee Media Bureau</em></span>
            <span class="service-year">2016</span>
          </div>
        </div>
        <span class="service-badge"></span>
      </div>

      <div class="service-item">
        <span class="service-num">22</span>
        <div class="service-body">
          <div class="service-title"><a href="http://www.business-standard.com/article/news-ians/wait-longer-for-feedback-to-boost-service-ratings-online-116051100427_1.html" target="_blank">Wait Longer for Feedback to Boost Service Ratings Online</a></div>
          <div class="service-meta">
            <span class="service-role"><em>Business Standard Ltd</em></span>
            <span class="service-year">2016</span>
          </div>
        </div>
        <span class="service-badge"></span>
      </div>

      <div class="service-item">
        <span class="service-num">23</span>
        <div class="service-body">
          <div class="service-title"><a href="http://www.spektrum.de/news/weiter-weg-und-laenger-her-gefaellt-uns-besser/1409908" target="_blank">Psychology: Further Away and Longer Ago Feels Better</a></div>
          <div class="service-meta">
            <span class="service-role"><em>Spektrum.de</em></span>
            <span class="service-year">2016</span>
          </div>
        </div>
        <span class="service-badge"></span>
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
