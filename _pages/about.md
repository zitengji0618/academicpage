---
permalink: /
title: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<style>
  .about-intro p {
    font-size: 1rem;
    line-height: 1.65;
    color: #333;
    margin-bottom: 1rem;
  }
  .about-section-title {
    font-size: 1.5rem;
    font-weight: 600;
    margin: 2rem 0 1rem;
    padding-bottom: 0.5rem;
    border-bottom: 2px solid #003262;
    color: #003262;
    display: flex;
    align-items: center;
    gap: 0.6rem;
  }
  .about-section-title i { font-size: 1.25rem; }
  .timeline-card {
    display: flex;
    align-items: center;
    gap: 1.25rem;
    background: #fff;
    border: 1px solid #e5e7eb;
    border-radius: 10px;
    padding: 1rem 1.25rem;
    margin-bottom: 1rem;
    transition: box-shadow 0.15s ease, border-color 0.15s ease, transform 0.15s ease;
  }
  .timeline-card:hover {
    box-shadow: 0 6px 18px rgba(0, 0, 0, 0.08);
    border-color: #003262;
    transform: translateY(-2px);
  }
  .timeline-logo {
    flex: 0 0 100px;
    height: 100px;
    display: flex;
    align-items: center;
    justify-content: center;
  }
  .timeline-logo img {
    max-width: 100%;
    max-height: 100%;
    object-fit: contain;
  }
  .timeline-body { flex: 1; min-width: 0; }
  .timeline-title {
    font-size: 1.05rem;
    font-weight: 600;
    color: #1a1a1a;
    margin: 0 0 0.25rem 0;
    line-height: 1.3;
  }
  .timeline-sub {
    font-size: 0.92rem;
    color: #444;
    margin: 0.15rem 0;
  }
  .timeline-meta {
    font-size: 0.85rem;
    color: #888;
    margin-top: 0.35rem;
    display: flex;
    flex-wrap: wrap;
    gap: 0.75rem;
  }
  .timeline-meta span { display: inline-flex; align-items: center; gap: 0.3rem; }
  .research-blurb {
    font-size: 1rem;
    line-height: 1.65;
    color: #333;
    background: #f8f9fa;
    border-left: 4px solid #003262;
    padding: 1rem 1.25rem;
    border-radius: 0 8px 8px 0;
  }
  @media (max-width: 600px) {
    .timeline-card { flex-direction: column; align-items: flex-start; }
    .timeline-logo { flex: 0 0 80px; height: 80px; align-self: center; }
  }
</style>

<div class="about-intro" markdown="1">
I am an incoming master's student in Robotics at the **University of Pennsylvania**.

Previously, I received my bachelor's degree in Computer Science at **UC Berkeley**, where I was fortunate to be advised by Professor [Koushil Sreenath](https://hybrid-robotics.berkeley.edu/koushil/) and Professor [Trevor Darrell](https://people.eecs.berkeley.edu/~trevor/) at [Berkeley Artificial Intelligence Research (BAIR)](https://bair.berkeley.edu/).

I have also conducted research at the [Search-based Planning Lab](https://www.ri.cmu.edu/robotics-groups/search-based-planning-laboratory/), [Carnegie Mellon University Robotics Institute](https://www.ri.cmu.edu/), under Professor [Maxim Likhachev](https://www.cs.cmu.edu/~maxim/). Prior to that, I worked as a research assistant at Tsinghua University.

I am also grateful to collaborate with all my graduate and undergraduate [collaborators](/academicpage/collaborators/), whose support and shared curiosity have shaped both my research and my growth as a researcher.
</div>

<h2 class="about-section-title"><i class="fas fa-lightbulb" aria-hidden="true"></i>Research Interests</h2>
<div class="research-blurb">
My research interests lie in robotics and robot learning, with a focus on enabling robots to acquire sophisticated skills through learning. To that end, I'm interested in both generalizable robots that adapt across environments and expert robots tuned for high-performance tasks.
</div>

<h2 class="about-section-title"><i class="fas fa-graduation-cap" aria-hidden="true"></i>Education</h2>

<div class="timeline-card">
  <div class="timeline-logo"><img src="/academicpage/images/upenn_logo.png" alt="University of Pennsylvania"></div>
  <div class="timeline-body">
    <h3 class="timeline-title">University of Pennsylvania</h3>
    <p class="timeline-sub">M.S. in Robotics</p>
    <div class="timeline-meta">
      <span><i class="fas fa-calendar" aria-hidden="true"></i>2026 – Present</span>
      <span><i class="fas fa-map-marker-alt" aria-hidden="true"></i>Philadelphia, PA, USA</span>
    </div>
  </div>
</div>

<div class="timeline-card">
  <div class="timeline-logo"><img src="/academicpage/images/ucberkeley_logo.svg" alt="UC Berkeley"></div>
  <div class="timeline-body">
    <h3 class="timeline-title">University of California, Berkeley</h3>
    <p class="timeline-sub">B.A. in Computer Science</p>
    <div class="timeline-meta">
      <span><i class="fas fa-calendar" aria-hidden="true"></i>2022 – 2026</span>
      <span><i class="fas fa-map-marker-alt" aria-hidden="true"></i>Berkeley, CA, USA</span>
    </div>
  </div>
</div>

<h2 class="about-section-title"><i class="fas fa-robot" aria-hidden="true"></i>Research Experience</h2>

<div class="timeline-card">
  <div class="timeline-logo"><img src="/academicpage/images/bair_logo.png" alt="BAIR"></div>
  <div class="timeline-body">
    <h3 class="timeline-title">Berkeley Artificial Intelligence Research Lab (BAIR)</h3>
    <p class="timeline-sub">Hybrid Robotics · Advisor: Koushil Sreenath</p>
    <div class="timeline-meta">
      <span><i class="fas fa-calendar" aria-hidden="true"></i>Sep. 2025 – Present</span>
      <span><i class="fas fa-map-marker-alt" aria-hidden="true"></i>Berkeley, CA, USA</span>
    </div>
  </div>
</div>

<div class="timeline-card">
  <div class="timeline-logo"><img src="/academicpage/images/cmu_ri_logo.png" alt="CMU RI"></div>
  <div class="timeline-body">
    <h3 class="timeline-title">Robotics Institute, Carnegie Mellon University</h3>
    <p class="timeline-sub">Search-based Planning Lab · Advisor: Maxim Likhachev</p>
    <div class="timeline-meta">
      <span><i class="fas fa-calendar" aria-hidden="true"></i>May 2025 – Sep. 2025</span>
      <span><i class="fas fa-map-marker-alt" aria-hidden="true"></i>Pittsburgh, PA, USA</span>
    </div>
  </div>
</div>

<div class="timeline-card">
  <div class="timeline-logo"><img src="/academicpage/images/bair_logo.png" alt="BAIR"></div>
  <div class="timeline-body">
    <h3 class="timeline-title">Berkeley Artificial Intelligence Research Lab (BAIR)</h3>
    <p class="timeline-sub">Darrell Group · Advisor: Trevor Darrell</p>
    <div class="timeline-meta">
      <span><i class="fas fa-calendar" aria-hidden="true"></i>Sep. 2024 – May 2025</span>
      <span><i class="fas fa-map-marker-alt" aria-hidden="true"></i>Berkeley, CA, USA</span>
    </div>
  </div>
</div>

<div class="timeline-card">
  <div class="timeline-logo"><img src="/academicpage/images/tsinghua_logo.png" alt="Tsinghua University"></div>
  <div class="timeline-body">
    <h3 class="timeline-title">Tsinghua University</h3>
    <p class="timeline-sub">Advisor: Jia Liu</p>
    <div class="timeline-meta">
      <span><i class="fas fa-calendar" aria-hidden="true"></i>May 2024 – Aug. 2024</span>
      <span><i class="fas fa-map-marker-alt" aria-hidden="true"></i>Beijing, China</span>
    </div>
  </div>
</div>
