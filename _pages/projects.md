---
layout: page
title: cases
permalink: /projects/
description: Destaques por ator, organizados por categoria. Passe o mouse para o detalhe; clique para abrir o case completo.
nav: true
nav_order: 1
---

<style>
.case-cats{display:flex;gap:8px;flex-wrap:wrap;margin:0 0 1.6rem}
.case-cats a{font-family:var(--mono,ui-monospace,monospace);font-size:.72rem;letter-spacing:.07em;text-transform:uppercase;border:1px solid currentColor;padding:5px 12px;border-radius:999px;opacity:.65;text-decoration:none;color:inherit}
.case-cats a:hover{opacity:1;border-color:#DC2A17;color:#DC2A17}
.case-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(290px,1fr));gap:18px;margin:0 0 2.6rem}
.case-card{position:relative;display:block;border:1px solid rgba(127,127,127,.28);border-radius:12px;overflow:hidden;text-decoration:none;color:inherit;background:rgba(127,127,127,.05);transition:transform .18s ease,box-shadow .22s ease,border-color .18s ease}
.case-card:hover{transform:translateY(-5px);box-shadow:0 14px 32px rgba(0,0,0,.20);border-color:#DC2A17}
.case-card .cover{width:100%;aspect-ratio:11/7;object-fit:cover;display:block}
.case-card .meta{padding:13px 15px 15px}
.case-card .cat{font-family:var(--mono,ui-monospace,monospace);font-size:.66rem;letter-spacing:.09em;text-transform:uppercase;color:#DC2A17}
.case-card h3{margin:.3rem 0 0;font-size:1.04rem;line-height:1.18;letter-spacing:-.01em}
.case-card .pixel{position:absolute;top:9px;right:9px;width:34px;height:34px;image-rendering:pixelated;image-rendering:crisp-edges;filter:drop-shadow(0 1px 2px rgba(0,0,0,.35));transition:transform .18s ease,filter .18s ease;z-index:3}
.case-card:hover .pixel{transform:scale(1.3) rotate(-7deg);filter:drop-shadow(0 0 7px #DC2A17)}
.case-card .detail{position:absolute;left:0;right:0;bottom:0;background:linear-gradient(to top,rgba(8,8,8,.94),rgba(8,8,8,.80) 72%,transparent);color:#f2efe8;padding:20px 15px 13px;transform:translateY(101%);opacity:0;transition:transform .24s ease,opacity .2s ease}
.case-card:hover .detail{transform:translateY(0);opacity:1}
.case-card .detail p{margin:0;font-size:.82rem;line-height:1.45}
.case-card .detail .open{display:inline-block;margin-top:9px;font-family:var(--mono,ui-monospace,monospace);font-size:.68rem;letter-spacing:.07em;color:#fff;border-bottom:1.5px solid #DC2A17;padding-bottom:1px}
@media (prefers-reduced-motion: reduce){.case-card,.case-card .pixel,.case-card .detail{transition:none}}
</style>

{% assign cats = "governança de dados,educação digital" | split: "," %}

<nav class="case-cats" aria-label="Categorias">
{% for c in cats %}<a href="#{{ c | slugify }}">{{ c }}</a>{% endfor %}
</nav>

{% for c in cats %}
<h2 id="{{ c | slugify }}" class="category">{{ c }}</h2>
<div class="case-grid">
{% assign items = site.projects | where: "category", c | sort: "importance" %}
{% for p in items %}
{% if c == "governança de dados" %}{% assign px = "/assets/img/pixel_gov.png" %}{% else %}{% assign px = "/assets/img/pixel_edu.png" %}{% endif %}
<a class="case-card" href="{{ p.url | relative_url }}" aria-label="Abrir case: {{ p.title }}">
  <img class="cover" src="{{ p.img | relative_url }}" alt="{{ p.title }}" loading="lazy">
  <img class="pixel" src="{{ px | relative_url }}" alt="" aria-hidden="true">
  <div class="meta">
    <span class="cat">{{ p.category }}</span>
    <h3>{{ p.title }}</h3>
  </div>
  <div class="detail">
    <p>{{ p.description }}</p>
    <span class="open">abrir case &rarr;</span>
  </div>
</a>
{% endfor %}
</div>
{% endfor %}
