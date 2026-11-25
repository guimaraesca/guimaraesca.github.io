---
layout: page
title: cases
permalink: /projects/
description: Um quebra-cabeça das experiências e parcerias. Passe o mouse sobre uma peça para o detalhe; clique para abrir.
nav: true
nav_order: 1
---

<style>
.pz-legend{display:flex;gap:14px;flex-wrap:wrap;align-items:center;margin:0 0 1.1rem;font-family:var(--mono,ui-monospace,monospace);font-size:.68rem;letter-spacing:.06em;text-transform:uppercase;opacity:.78}
.pz-legend .dot{display:inline-block;width:10px;height:10px;border-radius:2px;margin-right:6px;vertical-align:-1px}
.pz-legend .gov{background:#DC2A17}.pz-legend .edu{background:#1b1b4d}
.pz-head{font-family:var(--mono,ui-monospace,monospace);font-size:.7rem;letter-spacing:.09em;text-transform:uppercase;opacity:.65;margin:1.6rem 0 .5rem}
.puzzle{display:grid;gap:5px;padding:2px 0}
.puzzle.big{grid-template-columns:repeat(auto-fill,minmax(200px,1fr))}
.puzzle.small{grid-template-columns:repeat(auto-fill,minmax(132px,1fr))}
.pz{position:relative;aspect-ratio:1/1;display:flex;flex-direction:column;align-items:center;justify-content:center;gap:5px;text-align:center;padding:14px 30px;text-decoration:none;color:inherit;overflow:hidden;background:var(--face,#fbfaf6);
  -webkit-mask:url("/assets/img/piece.svg") center/100% 100% no-repeat;mask:url("/assets/img/piece.svg") center/100% 100% no-repeat;
  transition:transform .17s ease,filter .2s ease}
.pz.gov{--face:#fceeeb;--edge:#DC2A17}.pz.edu{--face:#eceef6;--edge:#1b1b4d}
.pz.case{--face:#ffffff}
@media (prefers-color-scheme: dark){.pz{--face:#211f1a}.pz.gov{--face:#2b1a16}.pz.edu{--face:#191b27}.pz.case{--face:#2a2822}}
.pz:hover{transform:translateY(-8px) scale(1.06) rotate(-2deg);filter:drop-shadow(0 12px 16px rgba(0,0,0,.32));z-index:6}
.pz .ring{position:absolute;inset:0;pointer-events:none;-webkit-mask:url("/assets/img/piece.svg") center/100% 100% no-repeat;mask:url("/assets/img/piece.svg") center/100% 100% no-repeat;box-shadow:inset 0 0 0 2.5px var(--edge,rgba(127,127,127,.35))}
.pz.case img{max-width:72%;max-height:56%}
.pz img{max-width:66%;max-height:46%;object-fit:contain;z-index:1}
.pz .nm{font-weight:700;font-size:.72rem;line-height:1.08;letter-spacing:-.01em;word-break:break-word;z-index:1}
.pz .yr{font-family:var(--mono,ui-monospace,monospace);font-size:.6rem;letter-spacing:.05em;color:#DC2A17;z-index:1}
.pz .det{position:absolute;inset:0;background:rgba(8,8,8,.95);color:#f2efe8;display:flex;flex-direction:column;justify-content:center;padding:18px 26px;opacity:0;transition:opacity .18s ease}
.pz:hover .det{opacity:1}
.pz .det b{font-size:.78rem;line-height:1.15}
.pz .det span{font-size:.66rem;margin-top:5px;line-height:1.3;color:#d9d6ce}
.pz .det em{font-size:.62rem;margin-top:7px;font-style:normal;font-family:var(--mono,ui-monospace,monospace);color:#fff;border-top:1px solid #DC2A17;padding-top:4px;align-self:flex-start}
@media (prefers-reduced-motion: reduce){.pz,.pz .det{transition:none}}
</style>

<div class="pz-legend">
  <span><span class="dot gov"></span>governança de dados</span>
  <span><span class="dot edu"></span>educação digital</span>
</div>

<p class="pz-head">Cases — clique para abrir</p>
<div class="puzzle big">
{%- for p in site.projects -%}
  {%- if p.category == "governança de dados" -%}{%- assign cl = "gov" -%}{%- else -%}{%- assign cl = "edu" -%}{%- endif -%}
  <a class="pz case {{ cl }}" href="{{ p.url | relative_url }}" aria-label="Abrir case: {{ p.title }}">
    <span class="ring"></span>
    <img src="{{ p.logo | relative_url }}" alt="{{ p.title }}">
    <div class="det"><b>{{ p.title }}</b><span>{{ p.description }}</span><em>abrir case &rarr;</em></div>
  </a>
{%- endfor -%}
</div>

<p class="pz-head">Experiências &amp; parcerias — ver no CV</p>
<div class="puzzle small">
{%- assign exps = "SEPLAG-CE|2026–2027|gov|Consultor — Tecnologias Digitais e Educação Digital (via BID/EGPCE);OEI · SEDUC-RS|2026–2027|gov|Consultor — Redução da Evasão Escolar (Proteção à Trajetória);Brasscom|2021–2026|edu|Escola Digital e Conectada (patrocínio Intuit);HUB-UnB · Ebserh|2021–2022|gov|Consultor em TIC e ensino (via UNESCO);Tomara|2025|gov|Analista de Dados e Especialista em EPT;MEC · Banco Mundial|2022|gov|Consultor e avaliador — STEAM e PNLD;IFRN|2018–2021|edu|Professor Mediador e Coordenador de tutoria (EAD);Kroton · Pitágoras|2019|edu|Coordenador Geral de Polo (Natal/RN);UNIFACEX|2013–2015|edu|Professor de ensino superior (TI/Computação);GAMEDU|2014–2017|edu|Coordenador de Projetos — jogos digitais" | split: ";" -%}
{%- for e in exps -%}
  {%- assign f = e | split: "|" -%}
  <a class="pz {{ f[2] }}" href="{{ '/cv/' | relative_url }}" aria-label="{{ f[0] }} — ver no CV">
    <span class="ring"></span>
    <span class="nm">{{ f[0] }}</span>
    <span class="yr">{{ f[1] }}</span>
    <div class="det"><b>{{ f[0] }}</b><span>{{ f[3] }}</span><em>ver no CV &rarr;</em></div>
  </a>
{%- endfor -%}
</div>
