---
layout: page
permalink: /publications/
title: produção
description: Pesquisa, ensino e extensão — artigos, o livro aberto Colossus e a base docente.
nav: true
nav_order: 2
---

<style>
.gs{display:flex;flex-wrap:wrap;align-items:center;gap:16px;border:1px solid rgba(127,127,127,.28);border-radius:10px;padding:10px 16px;margin:.2rem 0 1rem}
.gsn{text-align:center;line-height:1.1}
.gsn b{display:block;font-size:1.3rem;color:#DC2A17}
.gsn span{font-size:.64rem;font-family:var(--mono,ui-monospace,monospace);letter-spacing:.05em;text-transform:uppercase;opacity:.7}
.gs .lk{margin-left:auto;display:flex;flex-wrap:wrap;gap:8px}
.gs .lk a{font-family:var(--mono,ui-monospace,monospace);font-size:.7rem;border-bottom:1.5px solid #DC2A17;text-decoration:none;color:inherit;padding-bottom:1px}
.gs .lk a:hover{color:#DC2A17}
.pgrid{display:grid;grid-template-columns:1.15fr 1fr;gap:16px;margin:0 0 1.1rem}
.col-card{display:grid;grid-template-columns:96px 1fr;gap:14px;border:1px solid rgba(127,127,127,.28);border-top:4px solid #DC2A17;border-radius:10px;padding:13px 15px}
.col-card img{width:96px;border-radius:4px;box-shadow:0 3px 10px rgba(0,0,0,.18)}
.col-card b{display:block;font-size:1rem}
.col-card p{font-size:.8rem;opacity:.82;line-height:1.5;margin:4px 0 8px}
.col-card .lk{display:flex;flex-wrap:wrap;gap:6px}
.col-card .lk a{font-family:var(--mono,ui-monospace,monospace);font-size:.64rem;letter-spacing:.04em;border:1px solid #DC2A17;color:#DC2A17;border-radius:999px;padding:2px 9px;text-decoration:none}
.col-card .lk a:hover{background:#DC2A17;color:#fff}
.epe{display:grid;gap:9px;align-content:start}
.ep{border-left:4px solid var(--c);padding:2px 0 2px 12px}
.ep b{display:block;font-size:.88rem}
.ep span{font-size:.78rem;opacity:.8;line-height:1.45}
.post article h2.sec{font-size:1.05rem;font-weight:700;margin:0 0 .3rem;padding-top:.8rem;border-top:1px solid rgba(127,127,127,.18)}
.publications h2.bibliography{display:none}
.publications ol.bibliography li{padding:.55rem 0;border-top:1px solid rgba(127,127,127,.12)}
.publications ol.bibliography{margin-bottom:0}
@media(max-width:860px){.pgrid{grid-template-columns:1fr}}
@media(max-width:480px){.col-card{grid-template-columns:70px 1fr}.col-card img{width:70px}}
</style>

{% include accent-dark.liquid %}

<div class="gs">
  <div class="gsn"><b>14</b><span>citações</span></div>
  <div class="gsn"><b>2</b><span>índice-h</span></div>
  <div class="gsn"><b>5</b><span>artigos</span></div>
  <div class="lk">
    <a href="https://scholar.google.com/citations?user=XfzydjwAAAAJ" target="_blank" rel="noopener">Google Acadêmico ↗</a>
    <a href="https://orcid.org/0000-0003-0885-3916" target="_blank" rel="noopener">ORCID ↗</a>
    <a href="http://lattes.cnpq.br/8972138029785555" target="_blank" rel="noopener">Lattes ↗</a>
  </div>
</div>

<div class="pgrid">
  <div class="col-card">
    <a href="{{ '/colossus/' | relative_url }}"><img src="{{ '/assets/img/colossus/capa.svg' | relative_url }}" alt="Capa do livro Colossus"></a>
    <div>
      <b>Colossus <span style="font-weight:400;opacity:.6;font-size:.8rem">· livro aberto</span></b>
      <p>Memorial pedagógico sobre pensamento computacional na Educação Básica, alinhado à BNCC Computação: 36 capítulos com atividades desplugadas e plugadas. Nasceu do grupo de estudos do CENEP-RN.</p>
      <div class="lk">
        <a href="https://github.com/guimaraesca/colossus-livro/releases/latest/download/Colossus.pdf">PDF</a>
        <a href="https://github.com/guimaraesca/colossus-livro/releases/latest/download/Colossus.epub">EPUB</a>
        <a href="https://github.com/guimaraesca/colossus-livro/releases/latest/download/Colossus.html">HTML</a>
        <a href="https://github.com/guimaraesca/colossus-livro">repositório</a>
        <a href="{{ '/colossus/' | relative_url }}">sobre o livro →</a>
      </div>
    </div>
  </div>
  <div class="epe">
    <div class="ep" style="--c:#5A5A72"><b>Ensino</b><span>Rede estadual (CENEP-RN), tutoria e mediação no IMD/UFRN, docência no IFRN e na UNIFACEX, coordenação de polo na Faculdade Pitágoras.</span></div>
    <div class="ep" style="--c:#DC2A17"><b>Pesquisa</b><span>Mestrado no PPGITE/UFRN sobre pensamento computacional e jogos digitais; PENSA-RN, programa estadual de formação docente.</span></div>
    <div class="ep" style="--c:#1b1b4d"><b>Extensão</b><span>EducaCode (Recife), Escola Digital e Conectada (Brasscom), Desafio GamEdu e o Colossus.</span></div>
  </div>
</div>

<h2 class="sec">Artigos</h2>

<div class="publications">

{% bibliography %}

</div>
