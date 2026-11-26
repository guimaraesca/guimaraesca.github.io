---
layout: about
title: sobre
permalink: /
subtitle: <strong>Ciência de Dados e IA para a educação pública</strong>, com governança desde a origem do dado

profile:
  align: right
  image: prof_pic.png
  image_circular: false
  more_info: >
    <p>Ciência de Dados · IA aplicada · Governança (EMIS)</p>
    <p>Consultorias · assessorias técnicas · bancas</p>
    <p>MEC · UNESCO · Banco Mundial · BID · OEI</p>

selected_papers: false
social: true

announcements:
  enabled: false

latest_posts:
  enabled: false
---

<style>
.vlist{display:grid;gap:11px;margin:.3rem 0 .4rem}
.v{border-left:4px solid var(--c);padding:7px 0 7px 13px}
.v b{display:block;font-size:.95rem}
.v span{font-size:.86rem;opacity:.78}
.mintro{font-size:.9rem;opacity:.82;margin:.2rem 0 .1rem}
.mintro small{font-family:var(--mono,ui-monospace,monospace);font-size:.64rem;letter-spacing:.05em;text-transform:uppercase;opacity:.6;display:block;margin-top:3px}
.mq{font-size:.98rem;font-weight:700;border-left:4px solid var(--c);padding-left:11px;margin:1.3rem 0 .05rem}
.mqq{font-style:italic;opacity:.72;font-size:.86rem;padding-left:15px;margin:0 0 .5rem}
.mgrid{display:grid;grid-template-columns:repeat(3,1fr);gap:8px}
.mcell{border:1px solid rgba(127,127,127,.28);border-top:3px solid var(--c);border-radius:9px;padding:12px 13px;display:flex;flex-direction:column}
.mcell .pub{font-family:var(--mono,ui-monospace,monospace);font-size:.58rem;letter-spacing:.06em;text-transform:uppercase;color:var(--c)}
.mcell .q{font-style:italic;font-size:.79rem;opacity:.82;margin:3px 0 6px}
.mcell p{font-size:.78rem;opacity:.84;line-height:1.35;margin:0 0 7px}
.mcell a{margin-top:auto;font-family:var(--mono,ui-monospace,monospace);font-size:.66rem;color:var(--c);text-decoration:none;border-top:1px solid rgba(127,127,127,.2);padding-top:6px}
.mcell a:hover{opacity:.75}
.ct{display:grid;grid-template-columns:repeat(auto-fit,minmax(290px,1fr));gap:10px 18px;margin:.3rem 0}
.cx b{font-size:.83rem}
.cx span{display:block;font-size:.74rem;opacity:.7;line-height:1.4;margin-top:1px}
@media(max-width:820px){.mgrid{grid-template-columns:1fr}}
</style>

Ajudo governos, organismos multilaterais, organizações do terceiro setor e empresas a transformar **dados educacionais em decisão**, e a decisão em política que funciona na escala de uma rede de ensino. São mais de **15 anos** entre tecnologia educacional, governança de dados e políticas públicas: comecei na coordenação de EAD do IMD/UFRN, passei por produtos de dados para seis redes estaduais e pela transição técnica de um sistema nacional de gestão escolar no MEC, e hoje construo motores de IA generativa para material didático.

Meu método parte de uma premissa: **IA confiável depende de dado governado, e dado governado depende de saber quem decide, com qual evidência e sob quais salvaguardas.** Por isso cada projeto articula três camadas. A **engenharia** cobre pipelines, modelos e painéis. A **governança** cobre papéis, qualidade, interoperabilidade e LGPD. A **avaliação** cobre os indicadores que mostram se a política chega à escola.

## Três formações, um método

<div class="vlist">
  <div class="v" style="--c:#5A5A72">
    <b>Filosofia · Licenciatura, UFRN</b>
    <span>Epistemologia e ética aplicadas à tecnologia: critérios de evidência, explicabilidade e limites de uso, que viram <strong>salvaguardas concretas</strong> em projetos de IA.</span>
  </div>
  <div class="v" style="--c:#DC2A17">
    <b>Gestão de Políticas Públicas · Bacharelado, UFRN</b>
    <span>Desenho, governança e avaliação de programas: teoria da mudança, indicadores, arranjos institucionais e <strong>fortalecimento de capacidades</strong> no setor público.</span>
  </div>
  <div class="v" style="--c:#1b1b4d">
    <b>Tecnologia, Dados e IA</b>
    <span>Mestrado em Inovação em Tecnologias Educacionais (PPGITE/UFRN, 2025) · Tecnologia em Ciência de Dados (UNIVESP, em curso) · Residência em IA (Instituto Eldorado/PUC-Campinas · PBIA) · MBA em Redes de Computadores (ESAB). A base técnica: <strong>engenharia de dados, modelagem estatística, analytics e IA generativa</strong> aplicados a sistemas educacionais.</span>
  </div>
</div>

## Consultoria: onde posso ajudar

<p class="mintro">Três frentes, três públicos. Cada célula parte de um problema recorrente e aponta um projeto em que já resolvi algo parecido.<small>linhas = frentes · colunas = terceiro setor · governos · indústria/setor privado</small></p>

<div style="--c:#DC2A17">
  <p class="mq">Transformação Digital</p>
  <p class="mqq">Seus sistemas conversam entre si? E alguém sabe quem responde por cada dado?</p>
  <div class="mgrid">
    <div class="mcell"><span class="pub">Terceiro setor</span><span class="q">"O financiador pergunta pelo impacto, e a resposta está espalhada em planilhas."</span><p>Base única, catálogo de indicadores e painéis de monitoramento para conselhos, doadores e prestação de contas — com a rotina de uso que faz o painel ser consultado.</p><a href="{{ '/projects/2_sigae/' | relative_url }}">→ Instituto Unibanco · SIGAE</a></div>
    <div class="mcell"><span class="pub">Governos</span><span class="q">"Precisamos migrar um sistema crítico sem parar a operação."</span><p>Fortalecimento de sistemas de informação educacional (EMIS): matriz de governança, critérios de prontidão, interoperabilidade (e-PING) e conformidade com a LGPD, inclusive o RIPD.</p><a href="{{ '/projects/1_mec/' | relative_url }}">→ MEC · UNESCO · SGP 2.0</a></div>
    <div class="mcell"><span class="pub">Indústria / privado</span><span class="q">"Os dados existem, mas não viram produto."</span><p>Arquitetura de dados em nuvem (BigQuery, Parquet), pipelines ETL/ELT e Product Ownership para produtos de dados escaláveis, com custo previsível e prontos para operar.</p><a href="{{ '/projects/2_sigae/' | relative_url }}">→ Instituto Unibanco · SIGAE</a></div>
  </div>
</div>

<div style="--c:#1b1b4d">
  <p class="mq">Educação</p>
  <p class="mqq">A política está escrita. Ela está chegando à sala de aula?</p>
  <div class="mgrid">
    <div class="mcell"><span class="pub">Terceiro setor</span><span class="q">"Queremos levar Computação a mais escolas sem perder qualidade."</span><p>Desenho e escala de programas de pensamento computacional, com formação docente baseada em evidência e foco em equidade de acesso.</p><a href="{{ '/projects/' | relative_url }}">→ Brasscom · Tomara (EPT) · PENSA-RN</a></div>
    <div class="mcell"><span class="pub">Governos</span><span class="q">"Precisamos transformar a BNCC Computação em currículo, formação e indicador."</span><p>Políticas de educação digital, avaliação de programas (inclusive de redução da evasão) e educação profissional (EPT), com acompanhamento por dados.</p><a href="{{ '/projects/4_educacode/' | relative_url }}">→ OEI · Recife · EducaCode</a></div>
    <div class="mcell"><span class="pub">Indústria / privado</span><span class="q">"Precisamos de uma coleção aprovável no PNLD, dentro do prazo."</span><p>Material didático com produção assistida por IA e governança editorial: alinhamento à BNCC rastreável, revisão estruturada e velocidade sem abrir mão da qualidade.</p><a href="{{ '/projects/5_trilhaia/' | relative_url }}">→ Hachura · TRILHA-IA</a></div>
  </div>
</div>

<div style="--c:#0E7C86">
  <p class="mq">Inovação</p>
  <p class="mqq">Antes de escalar a IA, alguém testou se ela é útil, segura e explicável?</p>
  <div class="mgrid">
    <div class="mcell"><span class="pub">Terceiro setor</span><span class="q">"Precisamos provar que o piloto funciona antes de pedir mais recursos."</span><p>Pilotos de IA de baixo custo, learning analytics e telemetria (xAPI) que geram evidência de aprendizagem e de uso desde o primeiro ciclo.</p><a href="{{ '/projects/4_educacode/' | relative_url }}">→ EducaCode (índice IPPC) · IMD/UFRN</a></div>
    <div class="mcell"><span class="pub">Governos</span><span class="q">"Precisamos decidir hoje olhando para 2030 ou 2050."</span><p>Modelagem preditiva e de cenários, IA responsável e explicabilidade, para antecipar riscos (como a evasão) e sustentar a decisão pública com método defensável.</p><a href="{{ '/projects/3_goias/' | relative_url }}">→ Instituto Sapien · Goiás 2050</a></div>
    <div class="mcell"><span class="pub">Indústria / privado</span><span class="q">"Nosso produto de IA generativa alucina, e não conseguimos auditar."</span><p>Motores de IA generativa prontos para produto: RAG híbrido, ontologias, rubricas de avaliação e validação determinística de saída.</p><a href="{{ '/projects/5_trilhaia/' | relative_url }}">→ Hachura · TRILHA-IA</a></div>
  </div>
</div>

Veja os **[cases]({{ '/projects/' | relative_url }})**, as **[publicações]({{ '/publications/' | relative_url }})** e o **[CV]({{ '/cv/' | relative_url }})**.

## Competências técnicas

<div class="ct">
  <div class="cx"><b>Engenharia de dados</b><span>Python (Pandas) · SQL avançado · R · GCP BigQuery · Apache Parquet · pipelines ETL/ELT · integração de microdados governamentais · migração de sistemas legados · prontidão operacional</span></div>
  <div class="cx"><b>Estatística, modelagem e avaliação</b><span>Scikit-learn · modelagem preditiva (risco de evasão) · séries temporais (Holt, ARIMA, combinação ponderada) · cenários de longo prazo · learning analytics · índices e indicadores compostos · avaliação de programas e políticas</span></div>
  <div class="cx"><b>Visualização e BI</b><span>Looker · Power BI · painéis executivos para secretarias e redes · painéis territoriais (município · região · dimensão) · catálogo de indicadores</span></div>
  <div class="cx"><b>Fontes e bases</b><span>IBGE · PNAD · CAGED · RAIS · IDEB · IPEA · IMB-GO · OCDE/PISA · PNUD · Banco Mundial · análise territorial por município e região de planejamento</span></div>
  <div class="cx"><b>IA generativa e engenharia de LLMs</b><span>LLMs open-weight · pipelines multietapa multimodelo · RAG híbrido (BGE-m3, denso + esparso BM25, reranking Cross-Encoder) · sqlite-vec · ontologias controladas · LoRA/QLoRA · prompt engineering · Pydantic · JSON Schema (validação determinística) · rubricas de saída · mitigação de alucinações · IA responsável</span></div>
  <div class="cx"><b>Governança de dados e de TI</b><span>DAMA-DMBOK · ISO/IEC 38500 · COBIT 2019 · ITIL 4 · LGPD · Relatório de Impacto (RIPD) · e-PING · interoperabilidade · EMIS · matriz de riscos · critérios de prontidão · pontos de controle</span></div>
  <div class="cx"><b>Produto e gestão de projetos</b><span>Product Ownership · backlog e priorização · PMBOK 7 · gestão por sprints · BPMN 2.0 · tradução de demanda de gestão em requisito técnico · formação de gestores em dados e indicadores</span></div>
  <div class="cx"><b>Educação digital e currículo</b><span>BNCC Computação · pensamento computacional · formação docente · EPT · STEAM · PNLD · desenho curricular · rubricas e portfólio digital</span></div>
  <div class="cx"><b>Tecnologia educacional e plataformas</b><span>Moodle · H5P · SCORM · cmi5 · xAPI · Scratch · Scratch Jr · micro:bit · Arduino · Tinkercad · Fritzing · Teachable Machine · jogos digitais educacionais · EAD em larga escala</span></div>
</div>

**Disponível para consultorias individuais, assessorias técnicas e bancas.** [carlosarturguimaraes@protonmail.com](mailto:carlosarturguimaraes@protonmail.com)
