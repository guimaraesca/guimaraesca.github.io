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
.kicker{font-size:1.28rem;font-weight:700;line-height:1.3;margin:.1rem 0 .55rem;letter-spacing:-.01em}
.kicker em{font-style:normal;color:#DC2A17}
.lead{font-size:.98rem;line-height:1.65;margin:0 0 .65rem}
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
.og .tiles{display:flex;gap:7px}
.og a{flex:1 1 0;min-width:0;display:flex;flex-direction:column;align-items:center;justify-content:center;gap:2px;height:78px;background:#fff;border:1px solid rgba(127,127,127,.2);border-radius:9px;padding:6px 8px;text-decoration:none;transition:transform .15s ease,box-shadow .15s ease}
.og a.w{flex-grow:2}
.og a:hover{transform:translateY(-2px);box-shadow:0 5px 12px rgba(0,0,0,.16)}
.og img{height:calc(72px / var(--sq,1));width:auto;max-width:100%;max-height:100%;min-height:0;object-fit:contain}
.og a.t img{max-height:calc(100% - 15px)}
.og a .tg{font-family:var(--mono,ui-monospace,monospace);font-size:.6rem;font-weight:700;letter-spacing:.06em;color:#1b1b4d;line-height:1}
.olink{font-size:.78rem;opacity:.75;margin:.5rem 0 0}
/* formação */
.edu{display:grid;grid-template-columns:repeat(3,1fr);gap:12px}
.ec{border:1px solid rgba(127,127,127,.22);border-radius:12px;padding:14px 15px 13px;display:flex;flex-direction:column;gap:7px;position:relative;overflow:hidden}
.ec::before{content:"";position:absolute;inset:0 0 auto 0;height:4px;background:var(--c)}
.ec .hd{display:flex;align-items:center;gap:10px}
.ec .ic{flex:none;width:38px;height:38px;border-radius:10px;display:flex;align-items:center;justify-content:center;background:var(--c);color:#fff;font-size:1rem}
.ec h3{font-size:.98rem;font-weight:700;margin:0;line-height:1.2}
.ec h3 small{display:block;font-family:var(--mono,ui-monospace,monospace);font-weight:400;font-size:.6rem;letter-spacing:.07em;text-transform:uppercase;opacity:.6;margin-top:2px}
.ec ul{list-style:none;margin:0;padding:0;display:grid;gap:4px}
.ec li{display:flex;justify-content:space-between;gap:8px;font-size:.76rem;line-height:1.3;padding:4px 8px;border-radius:6px;background:rgba(127,127,127,.08)}
.ec li em{font-style:normal;font-family:var(--mono,ui-monospace,monospace);font-size:.64rem;opacity:.7;white-space:nowrap}
.ec .gv{margin-top:auto!important}
.ec .gv{font-size:.78rem;line-height:1.45;opacity:.82;margin:0;padding-top:6px;border-top:1px dashed rgba(127,127,127,.3)}
.ec .gv b{color:var(--c)}
.axis-note{display:flex;align-items:center;gap:10px;margin:10px 0 0;font-size:.78rem}
.axis-note::before,.axis-note::after{content:"";flex:1;height:2px;background:linear-gradient(90deg,#5A5A72,#DC2A17,#1b1b4d);border-radius:2px;opacity:.55}
.axis-note span{font-family:var(--mono,ui-monospace,monospace);font-size:.64rem;letter-spacing:.07em;text-transform:uppercase;opacity:.75;white-space:nowrap}
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
@media(max-width:991px){.og{grid-column:span 12}.og .tiles{flex-wrap:wrap}.og a{flex:1 0 84px}.og a.w{flex:2 0 172px}}
@media(max-width:860px){.svc{grid-template-columns:1fr}.edu,.phases{grid-template-columns:1fr}.axis-note span{white-space:normal;text-align:center}
 .ph,.ph + .ph{padding:0 0 12px;border-left:0}.ph .bar{border-radius:4px!important}}
@media(max-width:520px){.og .tiles{gap:5px}.og a{flex:1 0 70px;height:60px;padding:4px 5px}.og a.w{flex:2 0 145px}.og img{height:calc(56px / var(--sq,1))}}
@media(prefers-reduced-motion:reduce){.og a{transition:none}}
</style>

<p class="kicker">Dados educacionais confiáveis, decisões defensáveis e <em>IA que pode ser auditada</em>.</p>

<p class="lead">Sou consultor técnico em <strong>Ciência de Dados, governança de dados e IA aplicadas à educação pública</strong>. Atuo no ponto que costuma ficar sem dono — entre quem desenha a política, quem opera o sistema e quem presta contas do resultado: diagnostico onde a informação se perde, desenho a arquitetura e as regras de responsabilidade sobre cada dado, implanto junto das equipes e defino os indicadores que mostram se a mudança chegou à escola.</p>

<p class="lead">Esse método foi testado em projetos com <strong>MEC, UNESCO, Banco Mundial, BID e OEI</strong>, redes estaduais e municipais, terceiro setor e coleções do PNLD — e apoiado em mais de uma década de atuação dentro da educação pública, que segue sendo a régua do que é viável.</p>

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
      {%- capture cls -%}{% if org.sq >= 1.75 or g.wide %}w{% endif %}{% if org.tag %} t{% endif %}{%- endcapture -%}
      <a href="{{ target }}" title="{{ org.name }}" style="--sq:{{ org.sq }}" class="{{ cls | strip }}"><img src="{{ org.logo | relative_url }}" alt="{{ org.name }}" loading="lazy">{% if org.tag %}<span class="tg">{{ org.tag }}</span>{% endif %}</a>
      {%- endif -%}
    {%- endfor -%}
    </div>
  </div>
{%- endfor -%}
</div>
<p class="olink">Cada logo leva ao case, à experiência ou ao período correspondente. Projetos por frente na <a href="{{ '/consultoria/' | relative_url }}">consultoria</a>.</p>

<h2 class="sec">Formação</h2>

<div class="edu">
  <div class="ec" style="--c:#5A5A72">
    <div class="hd"><span class="ic"><i class="fa-solid fa-scale-balanced" aria-hidden="true"></i></span><h3>Filosofia<small>evidência e ética</small></h3></div>
    <ul><li>Licenciatura · UFRN <em>2005–2008</em></li></ul>
    <p class="gv"><b>Na consultoria:</b> critérios de evidência, explicabilidade e limites de uso que viram salvaguardas em projetos de IA.</p>
  </div>
  <div class="ec" style="--c:#DC2A17">
    <div class="hd"><span class="ic"><i class="fa-solid fa-landmark" aria-hidden="true"></i></span><h3>Políticas Públicas<small>desenho e avaliação</small></h3></div>
    <ul><li>Bacharelado em Gestão de Políticas Públicas · UFRN <em>2012–2018</em></li></ul>
    <p class="gv"><b>Na consultoria:</b> teoria da mudança, indicadores, arranjos institucionais e avaliação de programas.</p>
  </div>
  <div class="ec" style="--c:#1b1b4d">
    <div class="hd"><span class="ic"><i class="fa-solid fa-microchip" aria-hidden="true"></i></span><h3>Tecnologia, Dados e IA<small>engenharia e modelagem</small></h3></div>
    <ul>
      <li>Mestrado · PPGITE/UFRN <em>2025</em></li>
      <li>Residência em IA · Eldorado/PUC-Campinas <em>em curso</em></li>
      <li>Bacharelado em Ciência de Dados · UNIVESP <em>em curso</em></li>
      <li>MBA em Redes de Computadores · ESAB <em>2013</em></li>
    </ul>
    <p class="gv"><b>Na consultoria:</b> engenharia de dados, modelagem estatística, analytics e IA generativa.</p>
  </div>
</div>
<p class="axis-note"><span>Eixo comum: educação pública · evidência · ética · governança</span></p>

<h2 class="sec" id="trajetoria">Trajetória</h2>

<div class="phases">
  <div class="ph" style="--c:#5A5A72">
    <div class="bar"></div><span class="yr">2009 — 2021</span>
    <h3>Sala de aula, EAD e gestão pública</h3>
    <ul>
      <li><em>2009–2014</em><p><b>CENEP-RN</b> <span>· professor da rede estadual</span></p></li>
      <li><em>2012–2021</em><p><b><a href="{{ '/projects/6_imd/' | relative_url }}">IMD/UFRN</a></b> <span>· coordenação de tutoria e de mediadores; GameLab e Desafio GamEdu</span></p></li>
      <li><em>2013–2015</em><p><b>UNIFACEX</b> <span>· docência em TI e Computação</span></p></li>
      <li><em>2014</em><p><b>SMS Natal</b> <span>· bolsista em gestão de políticas públicas (Mesa do SUS)</span></p></li>
      <li><em>2018–2021</em><p><b>IFRN</b> <span>· mediação e coordenação de tutoria EAD</span></p></li>
      <li><em>2019</em><p><b>Kroton · Pitágoras</b> <span>· coordenação geral de polo</span></p></li>
    </ul>
  </div>
  <div class="ph" style="--c:#1b1b4d">
    <div class="bar"></div><span class="yr">2020 — 2025</span>
    <h3>Dados, produto e política educacional</h3>
    <ul>
      <li><em>2020–2021</em><p><b>SmartMetropolis · IMD</b> <span>· analista de dados educacionais (índice IEST)</span></p></li>
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
      <li><em>2026–2027</em><p><b>SEPLAG-CE · BID</b> <span>· Ceará Mais Digital</span></p></li>
      <li><em>2026–2027</em><p><b>OEI · SEDUC-RS</b> <span>· redução da evasão escolar</span></p></li>
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
