---
permalink: /collaborators/
title: "Collaborators"
author_profile: true
collaborators:
  - name: "Chuye Hong"
    url: "https://chuye03.github.io/"
    affiliation: "UC Berkeley"
    logo: "ucberkeley_logo.svg"
  - name: "Rishi Veerapaneni"
    url: "https://rishi-v.github.io/"
    affiliation: "Carnegie Mellon University"
    logo: "cmu_logo.png"
  - name: "Wei Ding"
    url: "https://weiding99.github.io/"
    affiliation: "Tsinghua University"
    logo: "tsinghua_logo.png"
  - name: "Yiyang Shao"
    url: "https://yiyangshao2003.github.io/"
    affiliation: "UC Berkeley"
    logo: "ucberkeley_logo.svg"
---

<style>
  .collab-intro {
    font-size: 1rem;
    line-height: 1.65;
    color: #333;
    background: #f8f9fa;
    border-left: 4px solid #003262;
    padding: 1rem 1.25rem;
    border-radius: 0 8px 8px 0;
    margin-bottom: 1.75rem;
  }
  .collab-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
    gap: 1rem;
  }
  .collab-card {
    position: relative;
    display: flex;
    align-items: center;
    gap: 1rem;
    background: #fff;
    border: 1px solid #e5e7eb;
    border-radius: 10px;
    padding: 1rem 2.5rem 1rem 1.25rem;
    color: inherit !important;
    text-decoration: none !important;
    transition: box-shadow 0.15s ease, border-color 0.15s ease, transform 0.15s ease;
  }
  .collab-card:hover {
    box-shadow: 0 6px 18px rgba(0, 0, 0, 0.08);
    border-color: #003262;
    transform: translateY(-2px);
  }
  .collab-avatar {
    flex: 0 0 48px;
    height: 48px;
    border-radius: 50%;
    background: #003262;
    color: #fff;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 1.05rem;
    font-weight: 600;
    letter-spacing: 0.03em;
  }
  .collab-body { flex: 1; min-width: 0; }
  .collab-name {
    font-size: 1rem;
    font-weight: 600;
    color: #1a1a1a;
    margin-bottom: 0.25rem;
    line-height: 1.3;
  }
  .collab-card:hover .collab-name { color: #003262; }
  .collab-affil {
    font-size: 0.85rem;
    color: #555;
    line-height: 1.35;
    display: flex;
    align-items: center;
    gap: 0.45rem;
  }
  .collab-logo {
    width: 20px;
    height: 20px;
    object-fit: contain;
    flex: 0 0 20px;
  }
  .collab-arrow {
    position: absolute;
    top: 0.85rem;
    right: 0.9rem;
    color: #bbb;
    font-size: 0.75rem;
    transition: color 0.15s ease, transform 0.15s ease;
  }
  .collab-card:hover .collab-arrow {
    color: #003262;
    transform: translateX(2px);
  }
</style>

<div class="collab-intro">
I am deeply grateful to have worked with these wonderful collaborators (sorted in alphabetical order).
</div>

<div class="collab-grid">
{% assign people = page.collaborators | sort: "name" %}
{% for c in people %}
  {% assign parts = c.name | split: " " %}
  <a class="collab-card" href="{{ c.url }}" target="_blank" rel="noopener">
    <div class="collab-avatar" aria-hidden="true">{{ parts.first | slice: 0 }}{{ parts.last | slice: 0 }}</div>
    <div class="collab-body">
      <div class="collab-name">{{ c.name }}</div>
      <div class="collab-affil">{% if c.logo %}<img class="collab-logo" src="{{ c.logo | prepend: '/images/' | prepend: site.baseurl }}" alt="">{% endif %}<span>{{ c.affiliation }}</span></div>
    </div>
    <i class="fas fa-arrow-up-right-from-square collab-arrow" aria-hidden="true"></i>
  </a>
{% endfor %}
</div>
