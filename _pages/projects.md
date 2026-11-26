---
layout: page
title: cases
permalink: /projects/
description: Experiências e parcerias em três frentes temáticas. Passe o mouse para levantar a peça; clique para abrir.
nav: true
nav_order: 1
---

<style>
.theme{margin:1.4rem 0 2.1rem}
.theme-h{font-size:1.02rem;font-weight:700;border-left:4px solid var(--acc);padding-left:11px;margin:0 0 .3rem;letter-spacing:-.01em}
.theme-s{font-family:var(--mono,ui-monospace,monospace);font-size:.64rem;letter-spacing:.08em;text-transform:uppercase;opacity:.55;margin:0 0 1rem;padding-left:15px}
.pzgrid{display:grid;grid-template-columns:repeat(auto-fill,minmax(146px,1fr));gap:18px 11px}
.cell{display:flex;flex-direction:column;align-items:center;text-decoration:none;color:inherit}
.pz{position:relative;width:100%;aspect-ratio:1/1;display:flex;flex-direction:column;align-items:center;justify-content:center;gap:3px;padding:15px 26px;background:#fff;overflow:hidden;
  -webkit-mask:url("/assets/img/piece.svg") center/100% 100% no-repeat;mask:url("/assets/img/piece.svg") center/100% 100% no-repeat;
  transition:transform .18s ease,filter .2s ease}
.cell:hover .pz{transform:translateY(-9px) scale(1.05) rotate(-2deg);filter:drop-shadow(0 13px 17px rgba(0,0,0,.30))}
.pz .ring{position:absolute;inset:0;pointer-events:none;-webkit-mask:url("/assets/img/piece.svg") center/100% 100% no-repeat;mask:url("/assets/img/piece.svg") center/100% 100% no-repeat;box-shadow:inset 0 0 0 2.5px var(--acc)}
.pz img{max-width:74%;max-height:62%;object-fit:contain}
.pz .nm{font-weight:700;font-size:.78rem;line-height:1.08;letter-spacing:-.01em;color:#16150f;word-break:break-word}
.cap{margin-top:9px;text-align:center;max-width:168px}
.cap .t{display:block;font-weight:600;font-size:.78rem;line-height:1.16}
.cap .d{display:block;font-size:.67rem;opacity:.68;margin-top:3px;line-height:1.3}
.cell:hover .cap .t{color:var(--acc)}
@media (prefers-reduced-motion: reduce){.pz{transition:none}}
</style>

{%- assign exps = "SEPLAG-CE|2026–2027|t1|Consultor — Tecnologias Digitais e Educação Digital (via BID/EGPCE);OEI · SEDUC-RS|2026–2027|t1|Consultor — Redução da Evasão Escolar;Tomara|2025|t1|Analista de Dados e Especialista em EPT;MEC · Banco Mundial|2022|t1|Consultor e avaliador — STEAM e PNLD;HUB-UnB · Ebserh|2021–2022|t2|Consultor em TIC e ensino (via UNESCO);Brasscom|2021–2026|t2|Escola Digital e Conectada (patrocínio Intuit);IFRN|2018–2021|t3|Professor Mediador e Coordenador de tutoria (EAD);Kroton · Pitágoras|2019|t3|Coordenador Geral de Polo (Natal/RN);UNIFACEX|2013–2015|t3|Professor de ensino superior (TI/Computação);GAMEDU|2014–2017|t3|Coordenador de Projetos — jogos digitais" | split: ";" -%}
{%- assign themes = "t1~Governança de dados e política pública educacional~#DC2A17;t2~Educação digital e tecnologia educacional~#1b1b4d;t3~Trajetória de origem — EAD, docência e jogos digitais~#5A5A72" | split: ";" -%}

{%- for tt in themes -%}
{%- assign tp = tt | split: "~" -%}{%- assign tid = tp[0] -%}
<section class="theme" style="--acc:{{ tp[2] }}">
  <h2 class="theme-h">{{ tp[1] }}</h2>
  <p class="theme-s">cases + experiências</p>
  <div class="pzgrid">
  {%- assign cs = site.projects | where: "theme", tid | sort: "importance" -%}
  {%- for p in cs -%}
    <a class="cell" href="{{ p.url | relative_url }}" aria-label="Abrir case: {{ p.title }}">
      <span class="pz"><span class="ring"></span><img src="{{ p.logo | relative_url }}" alt="{{ p.title }}"></span>
      <span class="cap"><span class="t">{{ p.title }}</span><span class="d">{{ p.description }}</span></span>
    </a>
  {%- endfor -%}
  {%- for e in exps -%}{%- assign f = e | split: "|" -%}{%- if f[2] == tid -%}
    <a class="cell" href="{{ '/cv/' | relative_url }}" aria-label="{{ f[0] }} — ver no CV">
      <span class="pz"><span class="ring"></span><span class="nm">{{ f[0] }}</span></span>
      <span class="cap"><span class="t">{{ f[0] }} · {{ f[1] }}</span><span class="d">{{ f[3] }}</span></span>
    </a>
  {%- endif -%}{%- endfor -%}
  </div>
</section>
{%- endfor -%}
