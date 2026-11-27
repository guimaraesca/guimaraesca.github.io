---
layout: page
title: cases
permalink: /projects/
description: Cases e experiências organizados pelas frentes da consultoria. Cada item indica o público atendido.
nav: true
nav_order: 2
---

<style>
.pz-intro{font-size:.93rem;opacity:.82;line-height:1.55;margin:0 0 .8rem}
.pz-nav{display:flex;flex-wrap:wrap;gap:7px;margin:0 0 1.2rem}
.pz-nav a{font-family:var(--mono,ui-monospace,monospace);font-size:.66rem;letter-spacing:.06em;text-transform:uppercase;text-decoration:none;color:var(--c);border:1px solid var(--c);border-radius:999px;padding:4px 11px}
.pz-nav a:hover{background:var(--c);color:#fff}
.panels{column-count:2;column-gap:18px}
.tp{break-inside:avoid;-webkit-column-break-inside:avoid;display:inline-block;width:100%;border:1px solid rgba(127,127,127,.25);border-top:4px solid var(--acc);border-radius:12px;padding:14px 16px 10px;margin:0 0 18px}
.tp h2{font-size:1.08rem;font-weight:700;margin:0;color:var(--acc)}
.tp .tg{font-family:var(--mono,ui-monospace,monospace);font-size:.62rem;letter-spacing:.08em;text-transform:uppercase;opacity:.55;margin:2px 0 10px}
.crow{display:grid;grid-template-columns:92px 1fr;gap:13px;align-items:center;text-decoration:none;color:inherit;padding:8px 0;border-top:1px solid rgba(127,127,127,.15)}
.crow:first-of-type{border-top:0}
.pz{position:relative;width:92px;aspect-ratio:1/1;display:flex;align-items:center;justify-content:center;padding:12px 18px;background:#fff;-webkit-mask:url("/assets/img/piece.svg") center/100% 100% no-repeat;mask:url("/assets/img/piece.svg") center/100% 100% no-repeat;transition:transform .18s ease,filter .2s ease}
.crow:hover .pz{transform:translateY(-5px) rotate(-3deg) scale(1.05);filter:drop-shadow(0 9px 12px rgba(0,0,0,.28))}
.pz .ring{position:absolute;inset:0;pointer-events:none;-webkit-mask:url("/assets/img/piece.svg") center/100% 100% no-repeat;mask:url("/assets/img/piece.svg") center/100% 100% no-repeat;box-shadow:inset 0 0 0 2.5px var(--acc)}
.pz img{max-width:100%;max-height:100%;object-fit:contain}
.ctx .ctl{display:block;font-weight:700;font-size:.88rem;line-height:1.2}
.crow:hover .ctl{color:var(--acc)}
.ctx .cd{display:-webkit-box;-webkit-line-clamp:3;-webkit-box-orient:vertical;overflow:hidden;font-size:.76rem;opacity:.74;line-height:1.4;margin-top:3px}
.pub{display:inline-block;font-family:var(--mono,ui-monospace,monospace);font-size:.56rem;letter-spacing:.05em;text-transform:uppercase;color:var(--acc);border:1px solid var(--acc);border-radius:999px;padding:1px 7px;margin-top:4px;white-space:nowrap}
.tp .sub{font-family:var(--mono,ui-monospace,monospace);font-size:.6rem;letter-spacing:.09em;text-transform:uppercase;opacity:.5;margin:10px 0 2px;padding-top:8px;border-top:1px dashed rgba(127,127,127,.3)}
.elist{list-style:none;margin:0;padding:0}
.elist li a{display:grid;grid-template-columns:44px 1fr auto;gap:11px;align-items:center;text-decoration:none;color:inherit;padding:6px 0}
.elist li + li a{border-top:1px solid rgba(127,127,127,.12)}
.sym{width:44px;height:44px;border-radius:9px;background:#fff;border:1px solid rgba(127,127,127,.25);display:flex;align-items:center;justify-content:center;padding:5px;overflow:hidden}
.sym img{max-width:100%;max-height:100%;object-fit:contain}
.sym i{font-size:1.15rem;color:var(--acc)}
.etx .en{display:block;font-weight:600;font-size:.82rem;line-height:1.2}
.etx .en em{font-style:normal;font-family:var(--mono,ui-monospace,monospace);font-size:.66rem;opacity:.6;margin-left:4px}
.etx .er{display:block;font-size:.74rem;opacity:.72;line-height:1.35;margin-top:1px}
.elist li a:hover .en{color:var(--acc)}
.scale-note{font-size:.74rem;opacity:.6;margin-top:.4rem}
@media(max-width:860px){.panels{column-count:1}}
@media(prefers-reduced-motion:reduce){.pz{transition:none}}
</style>

{%- assign themes = "t1~Transformação Digital~sistemas, dados e governança~#DC2A17;t2~Educação~política, currículo e formação~#1b1b4d;t3~Inovação~IA, modelagem e cenários~#0E7C86;t4~Base de origem~EAD, docência e jogos digitais~#5A5A72" | split: ";" -%}

<p class="pz-intro">Projetos e vínculos agrupados pelas frentes da <a href="{{ '/consultoria/' | relative_url }}">consultoria</a>. Os cases, em forma de peça, abrem a página completa; as experiências levam ao CV. Cada item indica o público atendido.</p>

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
  <a class="crow" href="{{ p.url | relative_url }}" aria-label="Abrir case: {{ p.title }}">
    <span class="pz"><span class="ring"></span><img src="{{ p.logo | relative_url }}" alt="" loading="lazy"></span>
    <span class="ctx"><span class="ctl">{{ p.title }}</span><span class="cd">{{ p.description }}</span>{% if p.audience and p.audience != "Base de origem" %}<span class="pub">{{ p.audience }}</span>{% endif %}</span>
  </a>
  {%- endfor -%}
  {%- assign es = site.data.experiences | where: "theme", tid -%}
  {%- if es.size > 0 -%}
  <p class="sub">Experiências</p>
  <ul class="elist">
  {%- for e in es -%}
    <li><a href="{{ '/cv/' | relative_url }}" aria-label="{{ e.name }} — ver no CV">
      <span class="sym">{% if e.logo %}<img src="{{ e.logo | relative_url }}" alt="" loading="lazy">{% else %}<i class="{{ e.icon }}" aria-hidden="true"></i>{% endif %}</span>
      <span class="etx"><span class="en">{{ e.name }}<em>{{ e.period }}</em></span><span class="er">{{ e.role }}</span></span>
      {% if e.audience %}<span class="pub">{{ e.audience }}</span>{% else %}<span></span>{% endif %}
    </a></li>
  {%- endfor -%}
  </ul>
  {%- endif -%}
</section>
{%- endfor -%}
</div>

<p class="scale-note">Os números de escala citados nos cases descrevem os programas, não resultados individuais.</p>
