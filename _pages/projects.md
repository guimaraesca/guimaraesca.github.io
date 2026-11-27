---
layout: page
title: cases
permalink: /projects/
description: Cases e experiências organizados pelas frentes da consultoria.
nav: true
nav_order: 2
---

<style>
.pz-intro{font-size:.93rem;opacity:.82;line-height:1.55;margin:0 0 .8rem}
.orgs{display:grid;grid-template-columns:repeat(auto-fill,minmax(98px,1fr));gap:8px;margin:0 0 1.1rem}
.orgs a{display:flex;flex-direction:column;align-items:center;gap:4px;text-decoration:none;color:inherit}
.orgs .lg{width:100%;height:50px;background:#fff;border:1px solid rgba(127,127,127,.25);border-radius:8px;display:flex;align-items:center;justify-content:center;padding:7px 10px;transition:transform .15s ease,box-shadow .15s ease}
.orgs .lg img{max-width:100%;max-height:100%;object-fit:contain}
.orgs a:hover .lg{transform:translateY(-2px);box-shadow:0 4px 10px rgba(0,0,0,.15)}
.orgs .on{font-size:.6rem;line-height:1.15;text-align:center;opacity:.65}
.olabel{font-family:var(--mono,ui-monospace,monospace);font-size:.62rem;letter-spacing:.09em;text-transform:uppercase;opacity:.55;margin:0 0 6px}
.pz-nav{display:flex;flex-wrap:wrap;gap:7px;margin:0 0 1.2rem}
.pz-nav a{font-family:var(--mono,ui-monospace,monospace);font-size:.66rem;letter-spacing:.06em;text-transform:uppercase;text-decoration:none;color:var(--c);border:1px solid var(--c);border-radius:999px;padding:4px 11px}
.pz-nav a:hover{background:var(--c);color:#fff}
.panels{column-count:2;column-gap:18px}
.tp{break-inside:avoid;-webkit-column-break-inside:avoid;display:inline-block;width:100%;border:1px solid rgba(127,127,127,.25);border-top:4px solid var(--acc);border-radius:12px;padding:14px 16px 10px;margin:0 0 18px}
.tp h2{font-size:1.08rem;font-weight:700;margin:0;color:var(--acc)}
.tp .tg{font-family:var(--mono,ui-monospace,monospace);font-size:.62rem;letter-spacing:.08em;text-transform:uppercase;opacity:.55;margin:2px 0 10px}
.crow{display:grid;grid-template-columns:92px 1fr;gap:13px;align-items:center;text-decoration:none;color:inherit;padding:8px 0;border-top:1px solid rgba(127,127,127,.15);scroll-margin-top:80px}
.crow:first-of-type{border-top:0}
.pz{position:relative;width:92px;aspect-ratio:1/1;display:flex;flex-direction:column;gap:3px;align-items:center;justify-content:center;padding:13px 19px;background:#fff;-webkit-mask:url("/assets/img/piece.svg") center/100% 100% no-repeat;mask:url("/assets/img/piece.svg") center/100% 100% no-repeat;transition:transform .18s ease,filter .2s ease}
.crow:hover .pz{transform:translateY(-5px) rotate(-3deg) scale(1.05);filter:drop-shadow(0 9px 12px rgba(0,0,0,.28))}
.pz .ring{position:absolute;inset:0;pointer-events:none;-webkit-mask:url("/assets/img/piece.svg") center/100% 100% no-repeat;mask:url("/assets/img/piece.svg") center/100% 100% no-repeat;box-shadow:inset 0 0 0 2.5px var(--acc)}
.pz img{max-width:100%;max-height:100%;min-height:0;object-fit:contain}
.pz.duo img{max-height:47%}
.pz.duo i{display:block;width:60%;height:1px;background:rgba(0,0,0,.18);flex:none}
.ctx .ctl{display:block;font-weight:700;font-size:.88rem;line-height:1.2}
.crow:hover .ctl{color:var(--acc)}
.ctx .cd{display:-webkit-box;-webkit-line-clamp:3;-webkit-box-orient:vertical;overflow:hidden;font-size:.76rem;opacity:.74;line-height:1.4;margin-top:3px}
.pub{display:inline-block;font-family:var(--mono,ui-monospace,monospace);font-size:.56rem;letter-spacing:.05em;text-transform:uppercase;color:var(--acc);border:1px solid var(--acc);border-radius:999px;padding:1px 7px;margin-top:4px;white-space:nowrap}
.tp .sub{font-family:var(--mono,ui-monospace,monospace);font-size:.6rem;letter-spacing:.09em;text-transform:uppercase;opacity:.5;margin:10px 0 2px;padding-top:8px;border-top:1px dashed rgba(127,127,127,.3)}
.elist{list-style:none;margin:0;padding:0}
.elist li{scroll-margin-top:80px}
.elist li + li{border-top:1px solid rgba(127,127,127,.12)}
.elist summary{display:grid;grid-template-columns:104px 1fr auto 14px;gap:11px;align-items:center;padding:7px 0;cursor:pointer;list-style:none}
.elist summary::-webkit-details-marker{display:none}
.elist summary::after{content:"+";font-family:var(--mono,ui-monospace,monospace);font-size:.95rem;color:var(--acc);text-align:center;transition:transform .2s ease}
.elist details[open] summary::after{transform:rotate(45deg)}
.syms{display:flex;gap:4px;height:40px}
.sym{flex:1 1 0;min-width:0;height:40px;border-radius:8px;background:#fff;border:1px solid rgba(127,127,127,.25);display:flex;align-items:center;justify-content:center;padding:5px 6px;overflow:hidden}
.sym img{max-width:100%;max-height:100%;object-fit:contain}
.sym i{font-size:1.15rem;color:var(--acc)}
.etx .en{display:block;font-weight:600;font-size:.82rem;line-height:1.2}
.etx .en em{font-style:normal;font-family:var(--mono,ui-monospace,monospace);font-size:.66rem;opacity:.6;margin-left:4px}
.etx .er{display:block;font-size:.74rem;opacity:.72;line-height:1.35;margin-top:1px}
.elist summary:hover .en,.elist details[open] .en{color:var(--acc)}
.ed{margin:0 0 9px 115px;padding:8px 11px;border-left:2px solid var(--acc);background:rgba(127,127,127,.06);border-radius:0 8px 8px 0;font-size:.78rem;line-height:1.5}
.ed p{margin:0 0 4px}
.ed .cvl{font-family:var(--mono,ui-monospace,monospace);font-size:.62rem;letter-spacing:.05em;text-transform:uppercase}
.scale-note{font-size:.74rem;opacity:.6;margin-top:.4rem}
@media(max-width:860px){.panels{column-count:1}}
@media(max-width:520px){.elist summary{grid-template-columns:84px 1fr 14px}.elist summary .pub{display:none}.ed{margin-left:0}.orgs{grid-template-columns:repeat(auto-fill,minmax(80px,1fr))}}
@media(prefers-reduced-motion:reduce){.pz,.orgs .lg{transition:none}}
</style>
{% include accent-dark.liquid %}

{%- assign themes = "t1~Transformação Digital~sistemas, dados e governança~#DC2A17;t2~Educação~política, currículo e formação~#1b1b4d;t3~Inovação~IA, modelagem e cenários~#0E7C86;t4~Base de origem~EAD, docência e jogos digitais~#5A5A72" | split: ";" -%}

<p class="pz-intro">Os cases, em forma de peça, abrem a página completa; clique numa experiência para ver o descritivo. Veja também a <a href="{{ '/consultoria/' | relative_url }}">consultoria</a>.</p>

<p class="olabel">Instituições</p>
<div class="orgs">
{%- for o in site.data.orgs -%}
  {%- assign key = o[0] -%}{%- assign org = o[1] -%}{%- assign target = "" -%}
  {%- for p in site.projects -%}{%- if target == "" and p.orgs contains key -%}{%- assign target = "c-" | append: p.slug -%}{%- endif -%}{%- endfor -%}
  {%- for e in site.data.experiences -%}{%- if target == "" and e.orgs contains key -%}{%- assign target = "e-" | append: e.name | slugify -%}{%- endif -%}{%- endfor -%}
  <a href="#{{ target }}" title="{{ org.name }}"><span class="lg"><img src="{{ org.logo | relative_url }}" alt="{{ org.name }}" loading="lazy"></span><span class="on">{{ org.name }}</span></a>
{%- endfor -%}
</div>

<nav class="pz-nav" aria-label="Frentes">
{%- for tt in themes -%}{%- assign tp = tt | split: "~" -%}
<a href="#{{ tp[0] }}" style="--c:{{ tp[3] }}">{{ tp[1] }}</a>
{%- endfor -%}
</nav>

<div class="panels">
{%- for tt in themes -%}
{%- assign tp = tt | split: "~" -%}{%- assign tid = tp[0] -%}
<section class="tp" id="{{ tid }}" style="--acc:{{ tp[3] }}">
  <h2>{{ tp[1] }}</h2>
  <p class="tg">{{ tp[2] }}</p>
  {%- assign cs = site.projects | where: "theme", tid | sort: "importance" -%}
  {%- for p in cs -%}
  <a class="crow" id="c-{{ p.slug }}" href="{{ p.url | relative_url }}" aria-label="Abrir case: {{ p.title }}">
    <span class="pz{% if p.orgs.size > 1 %} duo{% endif %}"><span class="ring"></span>{%- for k in p.orgs -%}{%- assign org = site.data.orgs[k] -%}{% unless forloop.first %}<i></i>{% endunless %}<img src="{{ org.logo | relative_url }}" alt="{{ org.name }}" loading="lazy">{%- endfor -%}</span>
    <span class="ctx"><span class="ctl">{{ p.title }}</span><span class="cd">{{ p.description }}</span>{% if p.audience and p.audience != "Base de origem" %}<span class="pub">{{ p.audience }}</span>{% endif %}</span>
  </a>
  {%- endfor -%}
  {%- assign es = site.data.experiences | where: "theme", tid -%}
  {%- if es.size > 0 -%}
  <p class="sub">Experiências</p>
  <ul class="elist">
  {%- for e in es -%}
    <li id="e-{{ e.name | slugify }}"><details>
      <summary>
        <span class="syms">{%- if e.orgs -%}{%- for k in e.orgs -%}{%- assign org = site.data.orgs[k] -%}<span class="sym"><img src="{{ org.logo | relative_url }}" alt="{{ org.name }}" loading="lazy"></span>{%- endfor -%}{%- else -%}<span class="sym"><i class="{{ e.icon }}" aria-hidden="true"></i></span>{%- endif -%}</span>
        <span class="etx"><span class="en">{{ e.name }}<em>{{ e.period }}</em></span><span class="er">{{ e.role }}</span></span>
        {% if e.audience %}<span class="pub">{{ e.audience }}</span>{% else %}<span></span>{% endif %}
      </summary>
      <div class="ed"><p>{{ e.details }}</p><a class="cvl" href="{{ '/cv/' | relative_url }}">ver no CV →</a></div>
    </details></li>
  {%- endfor -%}
  </ul>
  {%- endif -%}
</section>
{%- endfor -%}
</div>

<p class="scale-note">Os números de escala citados nos cases descrevem os programas, não resultados individuais.</p>

<script>
(function(){
  function openHash(){var el=location.hash&&document.getElementById(location.hash.slice(1));if(!el)return;var d=el.querySelector('details');if(d){d.open=true;}}
  window.addEventListener('hashchange',openHash);openHash();
})();
</script>
