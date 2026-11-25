---
layout: page
title: cases
permalink: /projects/
description: Um quebra-cabeça das experiências e parcerias. Passe o mouse sobre uma peça para o detalhe; clique para abrir.
nav: true
nav_order: 1
---

<style>
.pz-legend{display:flex;gap:14px;flex-wrap:wrap;align-items:center;margin:0 0 1rem;font-family:var(--mono,ui-monospace,monospace);font-size:.68rem;letter-spacing:.06em;text-transform:uppercase;opacity:.75}
.pz-legend .dot{display:inline-block;width:10px;height:10px;border-radius:2px;margin-right:6px;vertical-align:-1px}
.pz-legend .gov{background:#DC2A17}.pz-legend .edu{background:#1b1b4d}
.puzzle{display:grid;grid-template-columns:repeat(auto-fill,minmax(148px,1fr));gap:7px;background:repeating-linear-gradient(45deg,rgba(127,127,127,.06),rgba(127,127,127,.06) 12px,rgba(127,127,127,.11) 12px,rgba(127,127,127,.11) 24px);padding:9px;border-radius:16px;border:1px solid rgba(127,127,127,.2)}
.pz{position:relative;aspect-ratio:1/1;border-radius:9px;background:var(--pz-face,#fbfaf6);border:1px solid rgba(127,127,127,.3);display:flex;flex-direction:column;align-items:center;justify-content:center;gap:6px;text-align:center;padding:10px;text-decoration:none;color:inherit;overflow:hidden;transition:transform .16s ease,box-shadow .2s ease,border-color .16s ease}
@media (prefers-color-scheme: dark){.pz{--pz-face:#201f1a}}
.pz:hover{transform:translateY(-7px) scale(1.06);box-shadow:0 16px 34px rgba(0,0,0,.28);border-color:#DC2A17;z-index:6}
.pz.gov{border-top:3px solid #DC2A17}.pz.edu{border-top:3px solid #1b1b4d}
/* jigsaw knobs: aparecem no hover */
.pz .knob{position:absolute;width:15px;height:15px;background:#DC2A17;border-radius:50%;opacity:0;transition:opacity .16s ease,transform .16s ease}
.pz .knob.t{top:-8px;left:calc(50% - 7px)}.pz .knob.r{right:-8px;top:calc(50% - 7px)}
.pz:hover .knob{opacity:1}
.pz img{max-width:78%;max-height:52%;object-fit:contain}
.pz .nm{font-weight:700;font-size:.82rem;line-height:1.1;letter-spacing:-.01em}
.pz .yr{font-family:var(--mono,ui-monospace,monospace);font-size:.6rem;letter-spacing:.05em;color:#DC2A17}
.pz .face{display:flex;flex-direction:column;align-items:center;justify-content:center;gap:6px;height:100%}
.pz .det{position:absolute;inset:0;background:rgba(8,8,8,.94);color:#f2efe8;display:flex;flex-direction:column;justify-content:center;padding:12px;opacity:0;transform:scale(.95);transition:opacity .18s ease,transform .18s ease}
.pz:hover .det{opacity:1;transform:scale(1)}
.pz .det b{font-size:.78rem;line-height:1.15}
.pz .det span{font-size:.66rem;margin-top:5px;line-height:1.3;color:#d9d6ce}
.pz .det em{font-size:.62rem;margin-top:7px;font-style:normal;font-family:var(--mono,ui-monospace,monospace);color:#fff;border-top:1px solid #DC2A17;padding-top:4px;align-self:flex-start}
@media (prefers-reduced-motion: reduce){.pz,.pz .knob,.pz .det{transition:none}}
</style>

<div class="pz-legend">
  <span><span class="dot gov"></span>governança de dados</span>
  <span><span class="dot edu"></span>educação digital</span>
  <span style="opacity:.6">16 peças · clique as com logo para abrir o case</span>
</div>

<div class="puzzle">
{%- assign order = "1_mec,2_sigae,3_goias,4_educacode,5_trilhaia,6_imd" | split: "," -%}
{%- comment -%} peças-case (com logo, clicáveis) {%- endcomment -%}
{%- for p in site.projects -%}
  {%- if p.category == "governança de dados" -%}{%- assign cl = "gov" -%}{%- else -%}{%- assign cl = "edu" -%}{%- endif -%}
  <a class="pz {{ cl }}" href="{{ p.url | relative_url }}" aria-label="Abrir case: {{ p.title }}">
    <span class="knob t"></span><span class="knob r"></span>
    <div class="face">
      <img src="{{ p.logo | relative_url }}" alt="{{ p.title }}">
    </div>
    <div class="det"><b>{{ p.title }}</b><span>{{ p.description }}</span><em>abrir case &rarr;</em></div>
  </a>
{%- endfor -%}
{%- comment -%} peças-experiência (texto, levam ao CV) {%- endcomment -%}
{%- assign exps = "SEPLAG-CE|2026–2027|gov|Consultor — Tecnologias Digitais e Educação Digital (via BID/EGPCE);OEI · SEDUC-RS|2026–2027|gov|Consultor — Redução da Evasão Escolar (Proteção à Trajetória);Brasscom|2021–2026|edu|Escola Digital e Conectada (patrocínio Intuit);HUB-UnB · Ebserh|2021–2022|gov|Consultor em TIC e ensino (via UNESCO);Tomara|2025|gov|Analista de Dados e Especialista em EPT;MEC · Banco Mundial|2022|gov|Consultor e avaliador — STEAM e PNLD;IFRN|2018–2021|edu|Professor Mediador e Coordenador de tutoria (EAD);Kroton · Pitágoras|2019|edu|Coordenador Geral de Polo (Natal/RN);UNIFACEX|2013–2015|edu|Professor de ensino superior (TI/Computação);GAMEDU|2014–2017|edu|Coordenador de Projetos — jogos digitais" | split: ";" -%}
{%- for e in exps -%}
  {%- assign f = e | split: "|" -%}
  <a class="pz {{ f[2] }}" href="{{ '/cv/' | relative_url }}" aria-label="{{ f[0] }} — ver no CV">
    <span class="knob t"></span><span class="knob r"></span>
    <div class="face">
      <span class="nm">{{ f[0] }}</span>
      <span class="yr">{{ f[1] }}</span>
    </div>
    <div class="det"><b>{{ f[0] }}</b><span>{{ f[3] }}</span><em>ver no CV &rarr;</em></div>
  </a>
{%- endfor -%}
</div>
