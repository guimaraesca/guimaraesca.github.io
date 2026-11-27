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
.lead{font-size:1.02rem;line-height:1.68;margin:.2rem 0 .9rem}
.hero-cta{display:flex;flex-wrap:wrap;align-items:center;gap:8px;margin:.2rem 0 1.2rem}
.btn-p,.btn-s{display:inline-block;font-family:var(--mono,ui-monospace,monospace);font-size:.74rem;letter-spacing:.03em;padding:8px 15px;border-radius:999px;text-decoration:none!important}
.btn-p{background:#DC2A17;color:#fff!important}
.btn-s{border:1.5px solid #DC2A17;color:#DC2A17!important}
.btn-p:hover,.btn-s:hover{opacity:.85}
.aud{font-family:var(--mono,ui-monospace,monospace);font-size:.62rem;letter-spacing:.07em;text-transform:uppercase;opacity:.6;margin-left:4px}
.olabel{font-family:var(--mono,ui-monospace,monospace);font-size:.62rem;letter-spacing:.09em;text-transform:uppercase;opacity:.55;margin:0 0 6px}
.orgs{display:grid;grid-template-columns:repeat(auto-fill,minmax(72px,1fr));gap:7px;margin:0 0 1.3rem}
.orgs a{display:block;height:46px;background:#fff;border:1px solid rgba(127,127,127,.25);border-radius:8px;padding:6px 9px;transition:transform .15s ease,box-shadow .15s ease}
.orgs a:hover{transform:translateY(-2px);box-shadow:0 4px 10px rgba(0,0,0,.15)}
.orgs img{width:100%;height:100%;object-fit:contain}
.post article h2.sec{font-size:1.1rem;font-weight:700;margin:1.3rem 0 .6rem;padding-top:.8rem;border-top:1px solid rgba(127,127,127,.18);clear:both}
.axis{margin:.3rem 0 .2rem}
.axis-band{display:flex;justify-content:space-between;align-items:center;background:linear-gradient(90deg,#5A5A72,#DC2A17,#1b1b4d);color:#fff;font-size:.8rem;font-weight:600;padding:8px 14px;border-radius:9px 9px 0 0}
.axis-band small{font-family:var(--mono,ui-monospace,monospace);font-weight:400;font-size:.62rem;letter-spacing:.08em;text-transform:uppercase;opacity:.85}
.axis-cols{display:grid;grid-template-columns:repeat(3,1fr)}
.axis-col{border:1px solid rgba(127,127,127,.25);border-top:5px solid var(--c);padding:11px 14px}
.axis-col b{display:block;font-size:.92rem}
.axis-col em{display:block;font-style:normal;font-family:var(--mono,ui-monospace,monospace);font-size:.6rem;letter-spacing:.06em;text-transform:uppercase;opacity:.6;margin:2px 0 5px}
.axis-col span{display:block;font-size:.79rem;opacity:.78;line-height:1.45}
.traj{list-style:none;margin:.2rem 0 .4rem;padding:0;display:grid;grid-template-columns:repeat(8,1fr);position:relative}
.traj::before{content:"";position:absolute;left:0;right:0;top:27px;height:2px;background:linear-gradient(90deg,#5A5A72 0 45%,#DC2A17 70%,#0E7C86)}
.traj li{position:relative;padding:0 8px 0 0}
.traj .y{display:block;font-family:var(--mono,ui-monospace,monospace);font-size:.66rem;font-weight:700;color:var(--c,#DC2A17);height:20px}
.traj .d{display:block;width:12px;height:12px;border-radius:50%;background:var(--c,#DC2A17);border:2px solid var(--global-bg-color,#fff);margin:0 0 7px;position:relative}
.traj b{display:block;font-size:.78rem;line-height:1.2}
.traj span.t{display:block;font-size:.7rem;opacity:.7;line-height:1.35;margin-top:2px}
.traj a{color:inherit}
.ct-wrap{margin:.9rem 0 .6rem;border:1px solid rgba(127,127,127,.22);border-radius:10px;padding:0 14px}
.ct-wrap summary{cursor:pointer;font-weight:600;font-size:.9rem;padding:10px 0;list-style:none}
.ct-wrap summary::-webkit-details-marker{display:none}
.ct-wrap summary::after{content:" +";color:#DC2A17;font-family:var(--mono,ui-monospace,monospace)}
.ct-wrap[open] summary::after{content:" −"}
.ct{display:grid;grid-template-columns:repeat(auto-fit,minmax(290px,1fr));gap:10px 20px;padding:0 0 12px}
.cx b{font-size:.82rem}
.cx span{display:block;font-size:.75rem;opacity:.72;line-height:1.45;margin-top:2px}
.foot{font-size:.9rem;margin:.6rem 0 0}
@media(max-width:860px){.axis-cols{grid-template-columns:1fr}.axis-band{flex-direction:column;gap:3px;text-align:center}
 .traj{grid-template-columns:1fr;gap:9px;padding-left:20px}.traj::before{left:5px;right:auto;top:4px;bottom:4px;width:2px;height:auto;background:linear-gradient(180deg,#5A5A72,#DC2A17,#0E7C86)}
 .traj .y{height:auto}.traj .d{position:absolute;left:-20px;top:2px;margin:0}}
@media(prefers-reduced-motion:reduce){.orgs a{transition:none}}
</style>

<p class="lead">Comecei em 2009 como professor da rede estadual do Rio Grande do Norte e passei mais de uma década entre sala de aula, tutoria e coordenação de cursos a distância. Hoje uno <strong>Ciência de Dados, governança e IA</strong> para ajudar governos, organismos multilaterais, terceiro setor e empresas a transformar evidência educacional em decisão — e decisão em política que funciona na escala de uma rede de ensino. A premissa: <strong>IA confiável requer dado governado.</strong></p>

<div class="hero-cta">
  <a class="btn-p" href="{{ '/consultoria/' | relative_url }}">Consultoria →</a>
  <a class="btn-s" href="mailto:carlosarturguimaraes@protonmail.com">Contato</a>
  <a class="btn-s" href="{{ '/cv/' | relative_url }}">CV</a>
  <span class="aud">governos · terceiro setor · setor privado</span>
</div>

<p class="olabel">Instituições com quem trabalhei</p>
<div class="orgs">
{%- for o in site.data.orgs -%}
  {%- assign key = o[0] -%}{%- assign org = o[1] -%}{%- assign target = "" -%}
  {%- for p in site.projects -%}{%- if target == "" and p.orgs contains key -%}
    {%- if p.theme == "t4" -%}{%- assign target = p.url | relative_url -%}{%- else -%}{%- assign target = "/consultoria/#c-" | append: p.slug | relative_url -%}{%- endif -%}
  {%- endif -%}{%- endfor -%}
  {%- for e in site.data.experiences -%}{%- if target == "" and e.orgs contains key -%}
    {%- if e.theme == "t4" -%}{%- assign target = "#trajetoria" -%}{%- else -%}{%- assign slug = e.name | slugify: "latin" -%}{%- assign target = "/consultoria/#e-" | append: slug | relative_url -%}{%- endif -%}
  {%- endif -%}{%- endfor -%}
  <a href="{{ target }}" title="{{ org.name }}"><img src="{{ org.logo | relative_url }}" alt="{{ org.name }}" loading="lazy"></a>
{%- endfor -%}
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

<ol class="traj">
  <li style="--c:#5A5A72"><span class="y">2009–2014</span><i class="d"></i><b>CENEP-RN</b><span class="t">Professor da rede estadual (SEEC-RN)</span></li>
  <li style="--c:#5A5A72"><span class="y">2012–2021</span><i class="d"></i><b><a href="{{ '/projects/6_imd/' | relative_url }}">IMD/UFRN</a></b><span class="t">Tutoria, mediadores, GameLab e GamEdu</span></li>
  <li style="--c:#5A5A72"><span class="y">2013–2021</span><i class="d"></i><b>UNIFACEX · IFRN</b><span class="t">Docência superior e coordenação de tutoria EAD</span></li>
  <li style="--c:#1b1b4d"><span class="y">2021–2026</span><i class="d"></i><b>Brasscom</b><span class="t">Escola Digital e Conectada</span></li>
  <li style="--c:#DC2A17"><span class="y">2023–2025</span><i class="d"></i><b>Instituto Unibanco</b><span class="t">Product Owner do SIGAE</span></li>
  <li style="--c:#DC2A17"><span class="y">2025</span><i class="d"></i><b>MEC · UNESCO · PNLD</b><span class="t">SGP 2.0, TRILHA-IA, Goiás 2050 e defesa do mestrado</span></li>
  <li style="--c:#0E7C86"><span class="y">2026–2027</span><i class="d"></i><b>Ceará · RS</b><span class="t">SEPLAG-CE via BID e OEI/SEDUC-RS</span></li>
  <li style="--c:#0E7C86"><span class="y">2026–2027</span><i class="d"></i><b>Residência em IA</b><span class="t">Instituto Eldorado / PUC-Campinas</span></li>
</ol>

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
