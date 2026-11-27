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

selected_papers: false
social: true
announcements:
  enabled: false
latest_posts:
  enabled: false
---

{% include accent-dark.liquid %}

<style>
.lead{font-size:1.02rem;line-height:1.66;margin:.2rem 0 .9rem}
.svc{display:grid;grid-template-columns:1fr 1fr;gap:9px 16px;margin:0 0 1rem}
.svc div{display:grid;grid-template-columns:30px 1fr;gap:9px;align-items:start}
.svc i{font-size:1.05rem;color:#DC2A17;text-align:center;padding-top:3px}
.svc p,.ph li p{margin:0}
.svc b{display:block;font-size:.86rem;line-height:1.25}
.svc span{display:block;font-size:.76rem;opacity:.75;line-height:1.4;margin-top:1px}
.hero-cta{display:flex;flex-wrap:wrap;align-items:center;gap:8px;margin:0 0 .4rem}
.btn-p,.btn-s{display:inline-block;font-family:var(--mono,ui-monospace,monospace);font-size:.74rem;letter-spacing:.03em;padding:8px 15px;border-radius:999px;text-decoration:none!important}
.btn-p{background:#DC2A17;color:#fff!important}
.btn-s{border:1.5px solid #DC2A17;color:#DC2A17!important}
.btn-p:hover,.btn-s:hover{opacity:.85}
.fmt{font-size:.74rem;opacity:.65;margin:0}
.post article h2.sec{font-size:1.1rem;font-weight:700;margin:1.4rem 0 .7rem;padding-top:.9rem;border-top:1px solid rgba(127,127,127,.18);clear:both}
/* instituições agrupadas */
.ogrid{display:grid;grid-template-columns:repeat(12,1fr);gap:10px}
.og{grid-column:span var(--span);border:1px solid rgba(127,127,127,.22);border-radius:11px;padding:8px 9px 9px}
.og p{font-family:var(--mono,ui-monospace,monospace);font-size:.6rem;letter-spacing:.08em;text-transform:uppercase;opacity:.6;margin:0 0 6px}
.og .tiles{display:grid;grid-template-columns:repeat(var(--span),1fr);gap:7px}
.og a{display:flex;align-items:center;justify-content:center;height:74px;background:#fff;border:1px solid rgba(127,127,127,.2);border-radius:9px;padding:6px 8px;transition:transform .15s ease,box-shadow .15s ease}
.og a.w{grid-column:span 2}
.og a:hover{transform:translateY(-2px);box-shadow:0 5px 12px rgba(0,0,0,.16)}
.og img{height:calc(70px / var(--sq,1));width:auto;max-width:100%;max-height:100%;object-fit:contain}
.og.cta{display:flex;flex-direction:column;justify-content:center;gap:6px;border-style:dashed;padding:12px 14px}
.og.cta b{font-size:.9rem}
.og.cta span{font-size:.76rem;opacity:.72;line-height:1.4}
.og.cta a{all:unset;cursor:pointer;font-family:var(--mono,ui-monospace,monospace);font-size:.72rem;color:#DC2A17}
/* formação */
.axis{margin:.3rem 0 .2rem}
.axis-band{display:flex;justify-content:space-between;align-items:center;background:linear-gradient(90deg,#5A5A72,#DC2A17,#1b1b4d);color:#fff;font-size:.8rem;font-weight:600;padding:8px 14px;border-radius:9px 9px 0 0}
.axis-band small{font-family:var(--mono,ui-monospace,monospace);font-weight:400;font-size:.62rem;letter-spacing:.08em;text-transform:uppercase;opacity:.85}
.axis-cols{display:grid;grid-template-columns:repeat(3,1fr)}
.axis-col{border:1px solid rgba(127,127,127,.25);border-top:5px solid var(--c);padding:11px 14px}
.axis-col b{display:block;font-size:.92rem}
.axis-col em{display:block;font-style:normal;font-family:var(--mono,ui-monospace,monospace);font-size:.6rem;letter-spacing:.06em;text-transform:uppercase;opacity:.6;margin:2px 0 5px}
.axis-col span{display:block;font-size:.79rem;opacity:.78;line-height:1.45}
/* trajetória por fases */
.phases{display:grid;grid-template-columns:repeat(3,1fr);gap:0}
.ph{position:relative;padding:0 14px 0 0}
.ph + .ph{padding-left:14px;border-left:1px dashed rgba(127,127,127,.3)}
.ph .bar{height:8px;background:var(--c);border-radius:4px;margin:0 0 8px}
.ph:first-child .bar{border-radius:4px 0 0 4px}.ph:last-child .bar{border-radius:0 4px 4px 0}
.ph .yr{font-family:var(--mono,ui-monospace,monospace);font-size:.66rem;font-weight:700;color:var(--c);letter-spacing:.04em}
.ph h3{font-size:.95rem;font-weight:700;margin:1px 0 7px}
.ph ul{list-style:none;margin:0;padding:0}
.ph li{display:grid;grid-template-columns:74px 1fr;gap:8px;font-size:.78rem;line-height:1.35;padding:4px 0;border-top:1px solid rgba(127,127,127,.12)}
.ph li em{font-style:normal;font-family:var(--mono,ui-monospace,monospace);font-size:.66rem;opacity:.65;padding-top:1px}
.ph li b{font-weight:600}
.ph li span{opacity:.75}
.ph li a{color:inherit;text-decoration:underline;text-decoration-color:var(--c);text-underline-offset:2px}
/* competências */
.ct-wrap{margin:1rem 0 .6rem;border:1px solid rgba(127,127,127,.22);border-radius:10px;padding:0 14px}
.ct-wrap summary{cursor:pointer;font-weight:600;font-size:.9rem;padding:10px 0;list-style:none}
.ct-wrap summary::-webkit-details-marker{display:none}
.ct-wrap summary::after{content:" +";color:#DC2A17;font-family:var(--mono,ui-monospace,monospace)}
.ct-wrap[open] summary::after{content:" −"}
.ct{display:grid;grid-template-columns:repeat(auto-fit,minmax(290px,1fr));gap:10px 20px;padding:0 0 12px}
.cx b{font-size:.82rem}
.cx span{display:block;font-size:.75rem;opacity:.72;line-height:1.45;margin-top:2px}
.foot{font-size:.9rem;margin:.6rem 0 0}
@media(max-width:991px){.og{grid-column:span 12}.og .tiles{grid-template-columns:repeat(auto-fill,minmax(92px,1fr))}.og.cta{grid-column:span 12}}
@media(max-width:860px){.svc{grid-template-columns:1fr}.axis-cols,.phases{grid-template-columns:1fr}.axis-band{flex-direction:column;gap:3px;text-align:center}
 .ph,.ph + .ph{padding:0 0 12px;border-left:0}.ph .bar{border-radius:4px!important}}
@media(max-width:520px){.og .tiles{grid-template-columns:repeat(4,1fr);gap:5px}.og a{height:56px;padding:4px 5px}.og img{height:calc(52px / var(--sq,1))}}
@media(prefers-reduced-motion:reduce){.og a{transition:none}}
</style>

<p class="lead">Consultor técnico em <strong>Ciência de Dados, governança de dados e IA aplicadas à educação pública</strong>. Apoio governos, organismos multilaterais, terceiro setor e empresas em projetos que precisam transformar dado educacional em decisão — com arquitetura confiável, responsabilidade clara sobre cada dado e indicadores que mostram se a mudança chega à escola.</p>

<div class="svc">
  <div><i class="fa-solid fa-sitemap" aria-hidden="true"></i><p><b>Governança de dados e EMIS</b><span>Diagnóstico de maturidade (DAMA-DMBOK, ISO/IEC 38500), papéis e responsabilidades, LGPD e interoperabilidade.</span></p></div>
  <div><i class="fa-solid fa-database" aria-hidden="true"></i><p><b>Engenharia e analytics</b><span>Pipelines ETL/ELT em nuvem, painéis executivos e modelos preditivos de risco, como evasão.</span></p></div>
  <div><i class="fa-solid fa-cubes" aria-hidden="true"></i><p><b>Produto de dados</b><span>Product Ownership de sistemas educacionais: backlog, critérios de prontidão e transição técnica.</span></p></div>
  <div><i class="fa-solid fa-robot" aria-hidden="true"></i><p><b>IA generativa auditável</b><span>RAG híbrido, ontologias, rubricas de avaliação e validação determinística de saída.</span></p></div>
  <div><i class="fa-solid fa-chalkboard-user" aria-hidden="true"></i><p><b>Currículo e formação</b><span>BNCC Computação, pensamento computacional, formação docente e coleções do PNLD.</span></p></div>
  <div><i class="fa-solid fa-chart-line" aria-hidden="true"></i><p><b>Avaliação de programas</b><span>Teoria da mudança, indicadores e monitoramento de resultados.</span></p></div>
</div>

<div class="hero-cta">
  <a class="btn-p" href="{{ '/consultoria/' | relative_url }}">Frentes e cases →</a>
  <a class="btn-s" href="mailto:carlosarturguimaraes@protonmail.com">Contato</a>
  <a class="btn-s" href="{{ '/cv/' | relative_url }}">CV</a>
</div>
<p class="fmt">Consultoria por produtos (padrão de termos de referência) · assessoria técnica contínua · bancas e pareceres</p>

<h2 class="sec">Instituições com quem trabalhei</h2>

<div class="ogrid">
{%- for g in site.data.orggroups -%}
  <div class="og" style="--span:{{ g.span }}">
    <p>{{ g.label }}</p>
    <div class="tiles">
    {%- for o in site.data.orgs -%}{%- assign key = o[0] -%}{%- assign org = o[1] -%}
      {%- if org.group == g.key -%}
      {%- assign target = "" -%}
      {%- for p in site.projects -%}{%- if target == "" and p.orgs contains key -%}
        {%- if p.theme == "t4" -%}{%- assign target = p.url | relative_url -%}{%- else -%}{%- assign target = "/consultoria/#c-" | append: p.slug | relative_url -%}{%- endif -%}
      {%- endif -%}{%- endfor -%}
      {%- for e in site.data.experiences -%}{%- if target == "" and e.orgs contains key -%}
        {%- if e.theme == "t4" -%}{%- assign target = "#trajetoria" -%}{%- else -%}{%- assign slug = e.name | slugify: "latin" -%}{%- assign target = "/consultoria/#e-" | append: slug | relative_url -%}{%- endif -%}
      {%- endif -%}{%- endfor -%}
      {%- if target == "" -%}{%- assign target = "#trajetoria" -%}{%- endif -%}
      <a href="{{ target }}" title="{{ org.name }}" style="--sq:{{ org.sq }}"{% if org.sq >= 1.75 or g.wide %} class="w"{% endif %}><img src="{{ org.logo | relative_url }}" alt="{{ org.name }}" loading="lazy"></a>
      {%- endif -%}
    {%- endfor -%}
    </div>
  </div>
{%- endfor -%}
  <div class="og cta" style="--span:4"><b>Projetos por frente</b><span>Transformação Digital, Educação e Inovação: cada logo leva ao case ou à experiência correspondente.</span><a href="{{ '/consultoria/' | relative_url }}">ver consultoria →</a></div>
</div>

<h2 class="sec">Formação</h2>

<div class="axis">
  <div class="axis-band"><span>Educação pública · evidência · ética · governança</span><small>eixo transversal</small></div>
  <div class="axis-cols">
    <div class="axis-col" style="--c:#5A5A72"><b>Filosofia</b><em>Licenciatura · UFRN</em><span>Epistemologia e ética aplicadas à tecnologia: critérios de evidência, explicabilidade e limites de uso que se tornam salvaguardas em projetos de IA.</span></div>
    <div class="axis-col" style="--c:#DC2A17"><b>Gestão de Políticas Públicas</b><em>Bacharelado · UFRN</em><span>Teoria da mudança, indicadores, arranjos institucionais, avaliação de programas e fortalecimento de capacidades no setor público.</span></div>
    <div class="axis-col" style="--c:#1b1b4d"><b>Tecnologia, Dados e IA</b><em>Mestrado PPGITE · Ciência de Dados UNIVESP · Residência em IA · MBA</em><span>Engenharia de dados, modelagem estatística, analytics e IA generativa aplicados a sistemas educacionais.</span></div>
  </div>
</div>

<h2 class="sec" id="trajetoria">Trajetória</h2>

<div class="phases">
  <div class="ph" style="--c:#5A5A72">
    <div class="bar"></div><span class="yr">2009 — 2021</span>
    <h3>Docência e educação a distância</h3>
    <ul>
      <li><em>2009–2014</em><p><b>CENEP-RN</b> <span>· professor da rede estadual</span></p></li>
      <li><em>2012–2021</em><p><b><a href="{{ '/projects/6_imd/' | relative_url }}">IMD/UFRN</a></b> <span>· coordenação de tutoria e de mediadores; GameLab e Desafio GamEdu</span></p></li>
      <li><em>2013–2015</em><p><b>UNIFACEX</b> <span>· docência em TI e Computação</span></p></li>
      <li><em>2018–2021</em><p><b>IFRN</b> <span>· mediação e coordenação de tutoria EAD</span></p></li>
      <li><em>2019</em><p><b>Kroton · Pitágoras</b> <span>· coordenação geral de polo</span></p></li>
    </ul>
  </div>
  <div class="ph" style="--c:#1b1b4d">
    <div class="bar"></div><span class="yr">2021 — 2025</span>
    <h3>Dados, produto e política educacional</h3>
    <ul>
      <li><em>2021–2022</em><p><b>HUB-UnB · Ebserh</b> <span>· TIC e ensino, via UNESCO</span></p></li>
      <li><em>2021–2026</em><p><b>Brasscom</b> <span>· Escola Digital e Conectada</span></p></li>
      <li><em>2022</em><p><b>MEC · Banco Mundial</b> <span>· STEAM e avaliação do PNLD</span></p></li>
      <li><em>2023–2025</em><p><b><a href="{{ '/projects/2_sigae/' | relative_url }}">Instituto Unibanco</a></b> <span>· Product Owner do SIGAE</span></p></li>
      <li><em>2024–2025</em><p><b><a href="{{ '/projects/4_educacode/' | relative_url }}">OEI · Recife</a></b> <span>· EducaCode</span></p></li>
    </ul>
  </div>
  <div class="ph" style="--c:#DC2A17">
    <div class="bar"></div><span class="yr">2025 — hoje</span>
    <h3>Consultoria em governança e IA</h3>
    <ul>
      <li><em>2025–2026</em><p><b><a href="{{ '/projects/1_mec/' | relative_url }}">MEC · UNESCO</a></b> <span>· governança de dados e SGP 2.0</span></p></li>
      <li><em>2025</em><p><b><a href="{{ '/projects/5_trilhaia/' | relative_url }}">Hachura · ImagiMaker</a></b> <span>· TRILHA-IA, PNLD 2027</span></p></li>
      <li><em>2025</em><p><b>Tomara</b> <span>· dados educacionais e EPT</span></p></li>
      <li><em>2025–2026</em><p><b><a href="{{ '/projects/3_goias/' | relative_url }}">Instituto Sapien</a></b> <span>· Goiás 2050</span></p></li>
      <li><em>2026–2027</em><p><b>SEPLAG-CE · OEI/SEDUC-RS</b> <span>· BID e redução da evasão</span></p></li>
    </ul>
  </div>
</div>

<details class="ct-wrap">
<summary>Competências técnicas</summary>
<div class="ct">
  <div class="cx"><b>Engenharia de dados</b><span>Python (Pandas) · SQL avançado · R · GCP BigQuery · Apache Parquet · pipelines ETL/ELT · microdados governamentais · migração de sistemas legados</span></div>
  <div class="cx"><b>Estatística, modelagem e avaliação</b><span>Scikit-learn · modelagem preditiva (risco de evasão) · séries temporais (Holt, ARIMA) · cenários de longo prazo · learning analytics · indicadores compostos</span></div>
  <div class="cx"><b>Visualização e BI</b><span>Looker · Power BI · painéis executivos para secretarias · painéis territoriais · catálogo de indicadores</span></div>
  <div class="cx"><b>Fontes e bases</b><span>IBGE · PNAD · CAGED · RAIS · IDEB · IPEA · OCDE/PISA · PNUD · Banco Mundial · análise por município e região</span></div>
  <div class="cx"><b>IA generativa e LLMs</b><span>modelos open-weight · pipelines multietapa · RAG híbrido (BGE-m3, BM25, Cross-Encoder) · sqlite-vec · ontologias · LoRA/QLoRA · Pydantic · JSON Schema · IA responsável</span></div>
  <div class="cx"><b>Governança de dados e de TI</b><span>DAMA-DMBOK · ISO/IEC 38500 · COBIT 2019 · ITIL 4 · LGPD/RIPD · e-PING · EMIS · matriz de riscos · critérios de prontidão</span></div>
  <div class="cx"><b>Produto e projetos</b><span>Product Ownership · backlog e priorização · PMBOK 7 · sprints · BPMN 2.0 · formação de gestores</span></div>
  <div class="cx"><b>Currículo e plataformas</b><span>BNCC Computação · pensamento computacional · EPT · STEAM · PNLD · Moodle · H5P · SCORM · cmi5 · xAPI · Scratch · micro:bit · Arduino</span></div>
</div>
</details>

<p class="foot"><strong>Disponível para consultorias, assessorias técnicas e bancas.</strong> <a href="mailto:carlosarturguimaraes@protonmail.com">carlosarturguimaraes@protonmail.com</a> · <a href="{{ '/en/' | relative_url }}">🌐 English</a></p>
