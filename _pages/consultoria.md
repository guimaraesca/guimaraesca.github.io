---
layout: page
title: consultoria
permalink: /consultoria/
description: "Três frentes, três públicos: problemas recorrentes, respostas testadas e os projetos que as comprovam."
nav: true
nav_order: 1
---

<style>
.c-lead{font-size:1.01rem;line-height:1.72;margin:0 0 1rem}
.c-front{border-top:1px solid rgba(127,127,127,.2);padding-top:1.3rem;margin-top:2rem}
.c-front h2{font-size:1.25rem;font-weight:700;border-left:5px solid var(--c);padding-left:12px;margin:0 0 .2rem}
.c-front .c-q{font-style:italic;opacity:.72;font-size:.92rem;padding-left:17px;margin:0 0 1rem}
.c-front p.c-txt{font-size:.96rem;line-height:1.72;margin:0 0 .9rem}
.mgrid{display:grid;grid-template-columns:repeat(3,1fr);gap:10px;margin:1rem 0 .4rem}
.mcell{border:1px solid rgba(127,127,127,.28);border-top:3px solid var(--c);border-radius:10px;padding:13px 14px;display:flex;flex-direction:column}
.mcell .pub{font-family:var(--mono,ui-monospace,monospace);font-size:.6rem;letter-spacing:.07em;text-transform:uppercase;color:var(--c)}
.mcell .q{font-style:italic;font-size:.82rem;opacity:.84;margin:4px 0 7px}
.mcell p{font-size:.82rem;opacity:.86;line-height:1.45;margin:0 0 9px}
.mcell a{margin-top:auto;font-family:var(--mono,ui-monospace,monospace);font-size:.68rem;color:var(--c);text-decoration:none;border-top:1px solid rgba(127,127,127,.2);padding-top:7px}
.mcell a:hover{opacity:.75}
.steps{display:grid;grid-template-columns:repeat(4,1fr);gap:12px;margin:1rem 0}
.step{border:1px solid rgba(127,127,127,.28);border-radius:10px;padding:13px 14px}
.step .n{font-family:var(--mono,ui-monospace,monospace);font-size:.7rem;color:#DC2A17;font-weight:700}
.step b{display:block;font-size:.93rem;margin:2px 0 4px}
.step span{font-size:.8rem;opacity:.78;line-height:1.45}
.formats{font-size:.92rem;line-height:1.65}
.exp-groups{display:grid;grid-template-columns:repeat(2,1fr);gap:14px 22px;margin:1rem 0}
.exp-g{border-left:4px solid var(--c);padding:4px 0 4px 13px}
.exp-g b{display:block;font-size:.95rem;margin-bottom:5px}
.exp-g ul{margin:0;padding-left:1rem}
.exp-g li{font-size:.84rem;line-height:1.55;opacity:.88}
.exp-g li a{font-weight:600}
.c-cta{margin-top:1.6rem;font-size:.95rem}
@media(max-width:860px){.mgrid,.steps,.exp-groups{grid-template-columns:1fr}}
</style>

<p class="c-lead">Organizações que lidam com educação enfrentam, cedo ou tarde, o mesmo impasse: informação em abundância, sistemas que não se comunicam e uma pressão crescente por evidência de resultado — agora acrescida da promessa, e do risco, da inteligência artificial. Esta consultoria existe para atravessar esse impasse com método: diagnosticar onde a informação se perde, desenhar a arquitetura e as regras que a tornam confiável, implantar junto de quem opera no dia a dia e medir se a mudança chega ao destino.</p>

<p class="c-lead">Trabalho com governos e organismos multilaterais, organizações do terceiro setor e empresas de tecnologia ou de conteúdo educacional. As necessidades variam; o raciocínio se repete. Por isso a atuação se organiza em três frentes, e em cada cruzamento entre frente e público há um problema típico, uma resposta e um projeto que a comprova.</p>

<section class="c-front" id="transformacao-digital" style="--c:#DC2A17">
  <h2>Transformação Digital</h2>
  <p class="c-q">Seus sistemas conversam entre si? E alguém sabe quem responde por cada dado?</p>
  <p class="c-txt">Na educação, transformação digital raramente é um problema de tecnologia. Na maior parte das vezes, trata-se de responsabilidade: quem responde por cada registro, quais regras garantem sua qualidade, como plataformas distintas trocam informação sem perda nem duplicidade. Sem essas definições, novos sistemas apenas multiplicam planilhas paralelas e relatórios que ninguém consegue reconciliar.</p>
  <p class="c-txt">A entrada costuma ser um diagnóstico de maturidade, ancorado em DAMA-DMBOK e ISO/IEC 38500, que revela lacunas de papéis, de qualidade e de interoperabilidade. A partir dele, desenho a matriz de governança, os critérios de prontidão e a arquitetura — em nuvem, quando faz sentido — e acompanho a implantação até que a rotina se sustente sem consultoria externa.</p>
  <div class="mgrid">
    <div class="mcell"><span class="pub">Terceiro setor</span><span class="q">"O financiador pergunta pelo impacto, e a resposta está espalhada em planilhas."</span><p>Base única, catálogo de indicadores e painéis de monitoramento para conselhos, doadores e prestação de contas — com a rotina de uso que mantém o painel consultado.</p><a href="{{ '/projects/2_sigae/' | relative_url }}">→ Instituto Unibanco · SIGAE</a></div>
    <div class="mcell"><span class="pub">Governos</span><span class="q">"Precisamos migrar um sistema crítico sem parar a operação."</span><p>Fortalecimento de sistemas de informação educacional (EMIS): matriz de governança, critérios de prontidão, interoperabilidade (e-PING) e conformidade com a LGPD, inclusive o RIPD.</p><a href="{{ '/projects/1_mec/' | relative_url }}">→ MEC · UNESCO · SGP 2.0</a></div>
    <div class="mcell"><span class="pub">Setor privado</span><span class="q">"Os dados existem, mas não viram produto."</span><p>Arquitetura em nuvem (BigQuery, Parquet), pipelines ETL/ELT e Product Ownership para produtos escaláveis, com custo previsível e prontos para operar.</p><a href="{{ '/projects/2_sigae/' | relative_url }}">→ Instituto Unibanco · SIGAE</a></div>
  </div>
</section>

<section class="c-front" id="educacao" style="--c:#1b1b4d">
  <h2>Educação</h2>
  <p class="c-q">A política está escrita. Ela está chegando à sala de aula?</p>
  <p class="c-txt">Políticas educacionais costumam nascer bem redigidas e chegar fragmentadas à escola. Entre o documento oficial e a aula há currículo a traduzir, professores a formar, recursos a produzir e resultados a acompanhar — e qualquer elo pode romper a cadeia. A experiência de mais de uma década como docente ajuda a enxergar onde essas rupturas acontecem.</p>
  <p class="c-txt">O trabalho é manter a cadeia íntegra: transformar diretrizes como a BNCC Computação em matrizes curriculares, trilhas formativas e instrumentos de avaliação; desenhar programas de pensamento computacional com foco em equidade de acesso; e apoiar editoras na produção de coleções aprováveis no PNLD, com alinhamento curricular rastreável do início ao fim.</p>
  <div class="mgrid">
    <div class="mcell"><span class="pub">Terceiro setor</span><span class="q">"Queremos levar Computação a mais escolas sem perder qualidade."</span><p>Desenho e escala de programas de pensamento computacional, com formação docente baseada em evidência e atenção à equidade.</p><a href="{{ '/projects/' | relative_url }}">→ Brasscom · Tomara (EPT) · PENSA-RN</a></div>
    <div class="mcell"><span class="pub">Governos</span><span class="q">"Precisamos transformar a BNCC Computação em currículo, formação e indicador."</span><p>Políticas de educação digital, avaliação de programas — inclusive de redução da evasão — e educação profissional (EPT), acompanhadas por evidência.</p><a href="{{ '/projects/4_educacode/' | relative_url }}">→ OEI · Recife · EducaCode</a></div>
    <div class="mcell"><span class="pub">Setor privado</span><span class="q">"Precisamos de uma coleção aprovável no PNLD, dentro do prazo."</span><p>Material didático com produção assistida por IA e governança editorial: aderência à BNCC rastreável, revisão estruturada e agilidade sem perda de qualidade.</p><a href="{{ '/projects/5_trilhaia/' | relative_url }}">→ Hachura · TRILHA-IA</a></div>
  </div>
</section>

<section class="c-front" id="inovacao" style="--c:#0E7C86">
  <h2>Inovação</h2>
  <p class="c-q">Antes de escalar a IA, alguém testou se ela é útil, segura e explicável?</p>
  <p class="c-txt">Inovar com inteligência artificial na educação exige mais prudência do que entusiasmo. Antes de ampliar qualquer solução, é preciso saber se ela resolve um problema real, se protege estudantes e se suas decisões podem ser explicadas a gestores, famílias e órgãos de controle.</p>
  <p class="c-txt">A abordagem combina pilotos enxutos, com evidência desde o primeiro ciclo, e engenharia rigorosa: modelagem preditiva e de cenários para antecipar riscos como a evasão, e motores generativos com recuperação híbrida de documentos, ontologias, rubricas e validação determinística — porque um sistema que não se deixa auditar não deveria entrar na escola.</p>
  <div class="mgrid">
    <div class="mcell"><span class="pub">Terceiro setor</span><span class="q">"Precisamos provar que o piloto funciona antes de pedir mais recursos."</span><p>Pilotos de baixo custo, learning analytics e telemetria (xAPI) que produzem evidência de aprendizagem e de uso já no primeiro ciclo.</p><a href="{{ '/projects/4_educacode/' | relative_url }}">→ EducaCode (índice IPPC) · IMD/UFRN</a></div>
    <div class="mcell"><span class="pub">Governos</span><span class="q">"Precisamos decidir hoje olhando para 2030 ou 2050."</span><p>Modelagem preditiva e de cenários, IA responsável e explicabilidade, para antecipar riscos e sustentar a decisão pública com método defensável.</p><a href="{{ '/projects/3_goias/' | relative_url }}">→ Instituto Sapien · Goiás 2050</a></div>
    <div class="mcell"><span class="pub">Setor privado</span><span class="q">"Nosso produto de IA generativa alucina, e não conseguimos auditar."</span><p>Motores generativos prontos para produção: RAG híbrido, ontologias, rubricas de avaliação e validação determinística de saída.</p><a href="{{ '/projects/5_trilhaia/' | relative_url }}">→ Hachura · TRILHA-IA</a></div>
  </div>
</section>

<section class="c-front" id="modo-de-trabalho" style="--c:#5A5A72">
  <h2>Modo de trabalho</h2>
  <p class="c-txt">Independentemente da frente, cada contratação percorre quatro etapas, ajustadas ao porte e ao prazo do projeto:</p>
  <div class="steps">
    <div class="step"><span class="n">01</span><b>Diagnóstico</b><span>Escuta dos atores, leitura de sistemas e bases, mapa de lacunas e riscos.</span></div>
    <div class="step"><span class="n">02</span><b>Desenho</b><span>Arquitetura, regras de governança, indicadores e teoria da mudança.</span></div>
    <div class="step"><span class="n">03</span><b>Implantação</b><span>Construção com as equipes, formação e transferência de conhecimento.</span></div>
    <div class="step"><span class="n">04</span><b>Avaliação</b><span>Indicadores de uso e de resultado, ajustes e relatório final.</span></div>
  </div>
  <p class="formats"><strong>Formatos:</strong> consultoria individual por produtos e cronograma, no padrão de termos de referência de organismos internacionais; assessoria técnica contínua; bancas, pareceres e revisão especializada.</p>
</section>

<section class="c-front" id="experiencias" style="--c:#DC2A17">
  <h2>Experiências que sustentam a consultoria</h2>
  <p class="c-txt">Cada resposta acima nasce de um projeto real. Os principais estão organizados pelas mesmas frentes; os destacados abrem o case completo.</p>
  <div class="exp-groups">
    <div class="exp-g" style="--c:#DC2A17"><b>Transformação Digital</b><ul>
      <li><a href="{{ '/projects/1_mec/' | relative_url }}">MEC · UNESCO — Gestão Presente / SGP 2.0</a> (2025–2026)</li>
      <li><a href="{{ '/projects/2_sigae/' | relative_url }}">Instituto Unibanco — SIGAE</a> (2023–2025)</li>
      <li>SEPLAG-CE · Ceará Mais Digital, via BID (2026–2027)</li>
      <li>HUB-UnB · Ebserh, via UNESCO (2021–2022)</li></ul></div>
    <div class="exp-g" style="--c:#1b1b4d"><b>Educação</b><ul>
      <li><a href="{{ '/projects/4_educacode/' | relative_url }}">OEI · Recife — EducaCode</a> (2024–2025)</li>
      <li>OEI · SEDUC-RS — redução da evasão escolar (2026–2027)</li>
      <li>MEC · Banco Mundial — STEAM e PNLD (2022)</li>
      <li>Tomara — dados e EPT (2025) · Brasscom — Escola Digital e Conectada (2021–2026)</li></ul></div>
    <div class="exp-g" style="--c:#0E7C86"><b>Inovação</b><ul>
      <li><a href="{{ '/projects/5_trilhaia/' | relative_url }}">Hachura · PNLD 2027 — TRILHA-IA</a> (2025–2026)</li>
      <li><a href="{{ '/projects/3_goias/' | relative_url }}">Instituto Sapien — Goiás 2050</a> (2025–2026)</li></ul></div>
    <div class="exp-g" style="--c:#5A5A72"><b>Base de origem</b><ul>
      <li>CENEP-RN · rede estadual — docência (2009–2014)</li>
      <li><a href="{{ '/projects/6_imd/' | relative_url }}">IMD/UFRN — tecnologia educacional e jogos</a> (2012–2021)</li>
      <li>IFRN · UNIFACEX · GAMEDU · Faculdade Pitágoras</li></ul></div>
  </div>
  <p class="c-cta">Veja todos os <a href="{{ '/projects/' | relative_url }}">cases</a> e o <a href="{{ '/cv/' | relative_url }}">CV</a>. <strong>Disponível para consultorias, assessorias técnicas e bancas:</strong> <a href="mailto:carlosarturguimaraes@protonmail.com">carlosarturguimaraes@protonmail.com</a></p>
</section>
