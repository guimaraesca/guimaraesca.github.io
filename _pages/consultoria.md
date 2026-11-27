---
layout: page
title: consultoria
permalink: /consultoria/
description: "Três frentes, três públicos: problemas recorrentes, respostas testadas e os projetos que as comprovam."
nav: true
nav_order: 1
---

{% include accent-dark.liquid %}

<style>
.c-lead{font-size:1rem;line-height:1.65;margin:0 0 1rem}
/* abas das frentes */
.ftabs{display:grid;grid-template-columns:repeat(3,1fr);gap:8px;margin:0 0 1rem}
.ftab{all:unset;box-sizing:border-box;cursor:pointer;border:1px solid rgba(127,127,127,.3);border-top:4px solid var(--c);border-radius:10px;padding:10px 13px;transition:background .15s ease}
.ftab b{display:block;font-size:.98rem;color:var(--c)}
.ftab span{display:block;font-size:.74rem;opacity:.7;line-height:1.35;margin-top:2px}
.ftab:hover{background:rgba(127,127,127,.07)}
.ftab[aria-selected="true"]{background:var(--c);border-color:var(--c)}
.ftab[aria-selected="true"] b,.ftab[aria-selected="true"] span{color:#fff;opacity:1}
.ftab:focus-visible{outline:2px solid var(--c);outline-offset:2px}
html[data-theme="dark"] .ftab[aria-selected="true"] b,html[data-theme="dark"] .ftab[aria-selected="true"] span{color:#14142b}
.js .fpanel[hidden]{display:none}
.fpanel{border-left:4px solid var(--c);padding:2px 0 4px 16px;margin:0 0 1.4rem;scroll-margin-top:80px}
.js .fpanel h2{position:absolute;width:1px;height:1px;overflow:hidden;clip:rect(0 0 0 0)}
.c-q{font-weight:700;font-size:1.02rem;margin:0 0 .35rem}
.c-txt{font-size:.92rem;line-height:1.62;margin:0 0 .8rem;opacity:.9}
.mgrid{display:grid;grid-template-columns:repeat(3,1fr);gap:10px;margin:0 0 .9rem}
.mcell{border:1px solid rgba(127,127,127,.25);border-top:3px solid var(--c);border-radius:10px;padding:11px 13px}
.mcell .pub{display:block;font-family:var(--mono,ui-monospace,monospace);font-size:.6rem;letter-spacing:.07em;text-transform:uppercase;color:var(--c)}
.mcell .q{display:block;font-style:italic;font-size:.8rem;opacity:.85;margin:4px 0 6px}
.mcell p{font-size:.79rem;opacity:.82;line-height:1.45;margin:0}
/* provas */
.fproof{display:grid;grid-template-columns:1fr 1fr;gap:6px 22px}
.sub{font-family:var(--mono,ui-monospace,monospace);font-size:.6rem;letter-spacing:.09em;text-transform:uppercase;opacity:.55;margin:0 0 2px}
.crow{display:grid;grid-template-columns:84px 1fr;gap:12px;align-items:center;text-decoration:none;color:inherit;padding:7px 0;border-top:1px solid rgba(127,127,127,.15);scroll-margin-top:80px}
.sub + .crow{border-top:0}
.pz{position:relative;width:84px;aspect-ratio:1/1;display:flex;flex-direction:column;gap:3px;align-items:center;justify-content:center;padding:12px 17px;background:#fff;-webkit-mask:url("/assets/img/piece.svg") center/100% 100% no-repeat;mask:url("/assets/img/piece.svg") center/100% 100% no-repeat;transition:transform .18s ease,filter .2s ease}
.crow:hover .pz{transform:translateY(-4px) rotate(-3deg) scale(1.05);filter:drop-shadow(0 8px 11px rgba(0,0,0,.26))}
.pz .ring{position:absolute;inset:0;pointer-events:none;-webkit-mask:url("/assets/img/piece.svg") center/100% 100% no-repeat;mask:url("/assets/img/piece.svg") center/100% 100% no-repeat;box-shadow:inset 0 0 0 2.5px var(--c)}
.pz img{max-width:100%;max-height:100%;min-height:0;object-fit:contain}
.pz.duo img{max-height:47%}
.pz.duo i{display:block;width:60%;height:1px;background:rgba(0,0,0,.18);flex:none}
.ctl{display:block;font-weight:700;font-size:.86rem;line-height:1.2}
.crow:hover .ctl{color:var(--c)}
.cd{display:-webkit-box;-webkit-line-clamp:2;-webkit-box-orient:vertical;overflow:hidden;font-size:.75rem;opacity:.74;line-height:1.4;margin-top:2px}
.ctx .pub{display:inline-block;font-family:var(--mono,ui-monospace,monospace);font-size:.55rem;letter-spacing:.05em;text-transform:uppercase;color:var(--c);border:1px solid var(--c);border-radius:999px;padding:1px 7px;margin-top:4px}
.elist{list-style:none;margin:0;padding:0}
.elist li{scroll-margin-top:80px}
.elist li + li{border-top:1px solid rgba(127,127,127,.12)}
.elist summary{display:grid;grid-template-columns:96px 1fr 14px;gap:10px;align-items:center;padding:6px 0;cursor:pointer;list-style:none}
.elist summary::-webkit-details-marker{display:none}
.elist summary::after{content:"+";font-family:var(--mono,ui-monospace,monospace);color:var(--c);text-align:center;transition:transform .2s ease}
.elist details[open] summary::after{transform:rotate(45deg)}
.syms{display:flex;gap:4px;height:38px}
.sym{flex:1 1 0;min-width:0;height:38px;border-radius:8px;background:#fff;border:1px solid rgba(127,127,127,.25);display:flex;align-items:center;justify-content:center;padding:5px 6px;overflow:hidden}
.sym img{max-width:100%;max-height:100%;object-fit:contain}
.sym i{font-size:1.1rem;color:var(--c)}
.en{display:block;font-weight:600;font-size:.8rem;line-height:1.2}
.en em{font-style:normal;font-family:var(--mono,ui-monospace,monospace);font-size:.64rem;opacity:.6;margin-left:4px}
.er{display:block;font-size:.72rem;opacity:.72;line-height:1.35;margin-top:1px}
.er b{font-weight:600;color:var(--c)}
.elist summary:hover .en,.elist details[open] .en{color:var(--c)}
.ed{margin:0 0 8px 106px;padding:7px 10px;border-left:2px solid var(--c);background:rgba(127,127,127,.06);border-radius:0 8px 8px 0;font-size:.76rem;line-height:1.5}
.ed p{margin:0 0 3px}
.cvl{font-family:var(--mono,ui-monospace,monospace);font-size:.6rem;letter-spacing:.05em;text-transform:uppercase}
/* modo de trabalho */
.how{border-top:1px solid rgba(127,127,127,.2);padding-top:1rem}
.how h2{font-size:1.02rem;font-weight:700;margin:0 0 .6rem}
.steps{display:grid;grid-template-columns:repeat(4,1fr);gap:0;counter-reset:s;margin:0 0 .7rem}
.step{position:relative;padding:0 12px 0 0}
.step::before{counter-increment:s;content:"0" counter(s);font-family:var(--mono,ui-monospace,monospace);font-size:.68rem;font-weight:700;color:#DC2A17}
.step b{display:block;font-size:.88rem;margin:1px 0 2px}
.step span{font-size:.76rem;opacity:.75;line-height:1.4}
.formats{font-size:.84rem;line-height:1.55;opacity:.88;margin:0 0 .4rem}
.c-cta{font-size:.9rem;margin:0}
@media(max-width:860px){.ftabs{gap:6px}.ftab{padding:8px 9px}.ftab b{font-size:.8rem;line-height:1.2}.ftab span{display:none}.mgrid,.fproof{grid-template-columns:1fr}.steps{grid-template-columns:1fr 1fr;gap:10px}}
@media(max-width:520px){.ed{margin-left:0}.elist summary{grid-template-columns:80px 1fr 14px}}
@media(prefers-reduced-motion:reduce){.pz{transition:none}}
</style>

<p class="c-lead">Organizações que lidam com educação vivem o mesmo impasse: informação em abundância, sistemas que não se comunicam e pressão crescente por evidência — agora somada à promessa, e ao risco, da inteligência artificial. Atuo em três frentes, para governos e organismos multilaterais, terceiro setor e setor privado. Em cada uma, os problemas típicos por público e os projetos que comprovam a resposta.</p>

<div class="ftabs" role="tablist" aria-label="Frentes da consultoria">
  <button class="ftab" role="tab" id="tab-td" aria-controls="transformacao-digital" style="--c:#DC2A17"><b>Transformação Digital</b><span>sistemas, dados e governança</span></button>
  <button class="ftab" role="tab" id="tab-ed" aria-controls="educacao" style="--c:#1b1b4d"><b>Educação</b><span>política, currículo e formação</span></button>
  <button class="ftab" role="tab" id="tab-in" aria-controls="inovacao" style="--c:#0E7C86"><b>Inovação</b><span>IA, modelagem e cenários</span></button>
</div>

<section class="fpanel" id="transformacao-digital" role="tabpanel" aria-labelledby="tab-td" style="--c:#DC2A17">
  <h2>Transformação Digital</h2>
  <p class="c-q">Seus sistemas conversam entre si? E alguém sabe quem responde por cada dado?</p>
  <p class="c-txt">Na educação, transformação digital é menos tecnologia e mais responsabilidade: quem responde por cada registro, que regras garantem sua qualidade, como plataformas distintas trocam informação sem perda nem duplicidade. Parto de um diagnóstico de maturidade (DAMA-DMBOK, ISO/IEC 38500), desenho matriz de governança, critérios de prontidão e arquitetura, e acompanho a implantação até a rotina se sustentar sem apoio externo.</p>
  <div class="mgrid">
    <div class="mcell"><span class="pub">Terceiro setor</span><span class="q">"O financiador pergunta pelo impacto, e a resposta está espalhada em planilhas."</span><p>Base única, catálogo de indicadores e painéis de monitoramento para conselhos, doadores e prestação de contas.</p></div>
    <div class="mcell"><span class="pub">Governos</span><span class="q">"Precisamos migrar um sistema crítico sem parar a operação."</span><p>Fortalecimento de sistemas de informação educacional (EMIS): governança, prontidão, interoperabilidade (e-PING) e LGPD.</p></div>
    <div class="mcell"><span class="pub">Setor privado</span><span class="q">"Os dados existem, mas não viram produto."</span><p>Arquitetura em nuvem (BigQuery, Parquet), pipelines ETL/ELT e Product Ownership para produtos escaláveis.</p></div>
  </div>
  {% include fproof.liquid tid="t1" %}
</section>

<section class="fpanel" id="educacao" role="tabpanel" aria-labelledby="tab-ed" style="--c:#1b1b4d">
  <h2>Educação</h2>
  <p class="c-q">A política está escrita. Ela está chegando à sala de aula?</p>
  <p class="c-txt">Entre o documento oficial e a aula há currículo a traduzir, professores a formar, recursos a produzir e resultados a acompanhar — e qualquer elo pode romper a cadeia. Mantenho essa cadeia íntegra: da BNCC Computação a matrizes curriculares, trilhas formativas e instrumentos de avaliação; programas de pensamento computacional com equidade de acesso; coleções do PNLD com alinhamento curricular rastreável.</p>
  <div class="mgrid">
    <div class="mcell"><span class="pub">Terceiro setor</span><span class="q">"Queremos levar Computação a mais escolas sem perder qualidade."</span><p>Desenho e escala de programas de pensamento computacional, com formação docente baseada em evidência.</p></div>
    <div class="mcell"><span class="pub">Governos</span><span class="q">"Precisamos transformar a BNCC Computação em currículo, formação e indicador."</span><p>Políticas de educação digital, avaliação de programas — inclusive de redução da evasão — e EPT.</p></div>
    <div class="mcell"><span class="pub">Setor privado</span><span class="q">"Precisamos de uma coleção aprovável no PNLD, dentro do prazo."</span><p>Produção assistida por IA com governança editorial: aderência à BNCC rastreável e revisão estruturada.</p></div>
  </div>
  {% include fproof.liquid tid="t2" %}
</section>

<section class="fpanel" id="inovacao" role="tabpanel" aria-labelledby="tab-in" style="--c:#0E7C86">
  <h2>Inovação</h2>
  <p class="c-q">Antes de escalar a IA, alguém testou se ela é útil, segura e explicável?</p>
  <p class="c-txt">Pilotos enxutos, com evidência desde o primeiro ciclo, e engenharia rigorosa: modelagem preditiva e de cenários para antecipar riscos como a evasão, e motores generativos com recuperação híbrida de documentos, ontologias, rubricas e validação determinística — porque um sistema que não se deixa auditar não deveria entrar na escola.</p>
  <div class="mgrid">
    <div class="mcell"><span class="pub">Terceiro setor</span><span class="q">"Precisamos provar que o piloto funciona antes de pedir mais recursos."</span><p>Pilotos de baixo custo, learning analytics e telemetria (xAPI) com evidência já no primeiro ciclo.</p></div>
    <div class="mcell"><span class="pub">Governos</span><span class="q">"Precisamos decidir hoje olhando para 2030 ou 2050."</span><p>Modelagem preditiva e de cenários, IA responsável e explicabilidade para a decisão pública.</p></div>
    <div class="mcell"><span class="pub">Setor privado</span><span class="q">"Nosso produto de IA generativa alucina, e não conseguimos auditar."</span><p>Motores generativos prontos para produção: RAG híbrido, ontologias, rubricas e validação de saída.</p></div>
  </div>
  {% include fproof.liquid tid="t3" %}
</section>

<section class="how" id="modo-de-trabalho">
  <h2>Modo de trabalho</h2>
  <div class="steps">
    <div class="step"><b>Diagnóstico</b><span>Escuta dos atores, leitura de sistemas e bases, mapa de lacunas e riscos.</span></div>
    <div class="step"><b>Desenho</b><span>Arquitetura, regras de governança, indicadores e teoria da mudança.</span></div>
    <div class="step"><b>Implantação</b><span>Construção com as equipes, formação e transferência de conhecimento.</span></div>
    <div class="step"><b>Avaliação</b><span>Indicadores de uso e de resultado, ajustes e relatório final.</span></div>
  </div>
  <p class="formats"><strong>Formatos:</strong> consultoria individual por produtos, no padrão de termos de referência de organismos internacionais; assessoria técnica contínua; bancas, pareceres e revisão especializada. Os números de escala citados nos cases descrevem os programas, não resultados individuais.</p>
  <p class="c-cta"><strong>Vamos conversar:</strong> <a href="mailto:carlosarturguimaraes@protonmail.com">carlosarturguimaraes@protonmail.com</a></p>
</section>

<script>
(function(){
  var tabs=[].slice.call(document.querySelectorAll('.ftab'));
  var panels=tabs.map(function(t){return document.getElementById(t.getAttribute('aria-controls'));});
  document.documentElement.classList.add('js');
  function select(i,focus){
    tabs.forEach(function(t,j){var on=i===j;t.setAttribute('aria-selected',on);t.tabIndex=on?0:-1;panels[j].hidden=!on;});
    if(focus)tabs[i].focus();
  }
  tabs.forEach(function(t,i){
    t.addEventListener('click',function(){select(i);history.replaceState(null,'','#'+panels[i].id);});
    t.addEventListener('keydown',function(e){var k=e.key==='ArrowRight'?1:e.key==='ArrowLeft'?-1:0;if(k){e.preventDefault();select((i+k+tabs.length)%tabs.length,true);}});
  });
  function fromHash(){
    var id=decodeURIComponent(location.hash.slice(1));var el=id&&document.getElementById(id);var idx=0;
    if(el){panels.forEach(function(p,j){if(p===el||p.contains(el))idx=j;});}
    select(idx);
    if(el&&panels.indexOf(el)<0){var d=el.querySelector('details');if(d)d.open=true;setTimeout(function(){el.scrollIntoView({block:'center'});},60);}
  }
  window.addEventListener('hashchange',fromHash);fromHash();
})();
</script>
