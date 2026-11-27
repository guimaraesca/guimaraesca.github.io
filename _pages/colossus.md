---
layout: page
title: colossus
permalink: /colossus/
description: Colossus — memorial pedagógico sobre pensamento computacional na Educação Básica (BNCC-Computação).
nav: false
nav_order: 4
---

<style>
.col-hero{display:grid;grid-template-columns:150px 1fr;gap:20px;align-items:center;margin:.3rem 0 1rem}
.col-hero img{width:100%;border:1px solid rgba(127,127,127,.25);border-radius:8px}
.col-dl{display:flex;flex-wrap:wrap;gap:8px;margin:.4rem 0}
.col-dl a{font-family:var(--mono,ui-monospace,monospace);font-size:.72rem;letter-spacing:.03em;border:1px solid #DC2A17;color:#DC2A17;border-radius:999px;padding:6px 13px;text-decoration:none}
.col-dl a:hover{background:#DC2A17;color:#fff}
.col-figs{display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:12px;margin:1rem 0}
.col-figs figure{margin:0}
.col-figs img{width:100%;background:#fff;border:1px solid rgba(127,127,127,.25);border-radius:8px}
.col-figs figcaption{font-size:.72rem;opacity:.68;margin-top:5px;text-align:center}
.col-meta{font-size:.8rem;opacity:.75}
@media(max-width:620px){.col-hero{grid-template-columns:1fr}}
</style>

<div class="col-hero">
  <img src="{{ '/assets/img/colossus/capa.svg' | relative_url }}" alt="Capa do livro Colossus">
  <div>
    <p><strong>Colossus</strong> é um <strong>memorial pedagógico sobre pensamento computacional na Educação Básica</strong>, aberto e colaborativo, alinhado à <strong>BNCC-Computação</strong> (Resolução CNE/CEB nº 1/2022). O nome homenageia o computador britânico Colossus (Bletchley Park, 1943–1945) e os "colossos invisíveis" — estudantes e professoras da escola pública.</p>
    <div class="col-dl">
      <a href="https://github.com/guimaraesca/colossus-livro/releases/latest/download/Colossus.pdf" target="_blank" rel="noopener">📘 PDF</a>
      <a href="https://github.com/guimaraesca/colossus-livro/releases/latest/download/Colossus.epub" target="_blank" rel="noopener">📗 EPUB</a>
      <a href="https://github.com/guimaraesca/colossus-livro/releases/latest/download/Colossus.html" target="_blank" rel="noopener">🌐 HTML</a>
      <a href="https://github.com/guimaraesca/colossus-livro" target="_blank" rel="noopener">⌨ repositório</a>
    </div>
  </div>
</div>

Reúne **36 capítulos** cobrindo toda a Educação Básica — dos anos iniciais do Ensino Fundamental (1º ao 5º) aos anos finais (6º ao 9º) e ao Ensino Médio —, combinando **atividades desplugadas e plugadas**, projetos integradores, orientações ao professor, glossário e um roteiro de implementação curricular. Nasce do grupo de estudos do **CENEP-RN** e dialoga diretamente com a minha dissertação de mestrado (PPGITE/UFRN, 2025), *Integrando o pensamento computacional ao currículo por meio de formação docente baseada no desenvolvimento de jogos digitais*, e com o **PENSA-RN**.

### Alguns desenhos do livro

Cada conceito do pensamento computacional vira figura simples e desplugada — algoritmos, decomposição, padrões, abstração — pensada para a sala de aula:

<div class="col-figs">
  <figure><img src="{{ '/assets/img/colossus/cap-ai-04.png' | relative_url }}" alt="Rotina da sala como algoritmo"><figcaption>Rotina da sala como algoritmo (anos iniciais)</figcaption></figure>
  <figure><img src="{{ '/assets/img/colossus/cap-ef-03.png' | relative_url }}" alt="Padrões — anos finais"><figcaption>Padrões (anos finais do Fundamental)</figcaption></figure>
  <figure><img src="{{ '/assets/img/colossus/cap-ai-13.png' | relative_url }}" alt="Histórias com Scratch"><figcaption>Autoria com Scratch (anos iniciais)</figcaption></figure>
</div>

<p class="col-meta"><strong>Autor:</strong> Carlos Artur Guimarães · <strong>Licença:</strong> texto CC BY-SA 4.0 · código MIT · Volume 1 (v1.3.0, abr/2026), com Volumes 2 e 3 em preparação. Veja também as <a href="{{ '/publications/' | relative_url }}">publicações</a>.</p>
