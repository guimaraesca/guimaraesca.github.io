---
layout: page
title: Hachura · PNLD 2027 — TRILHA-IA
description: IA generativa com governança editorial para produção de material didático.
img: assets/img/case_trilhaia.png
importance: 2
category: educação digital
---

> **Nota de governança editorial.** Visão de alto nível do método; artefactos e dados de produção permanecem sob sigilo editorial.

**Contexto.** Produção e avaliação de material didático (coleção "Educação Digital", **PNLD 2027**) com **IA generativa controlada** — não apenas gerar texto, mas governar estrutura, qualidade, alinhamento curricular, revisão, evidências e integração com ambientes digitais de aprendizagem.

**Papel.** **Editor Geral** e concepção do **TRILHA-IA**, motor de produção de material didático com IA generativa.

**Decisões técnicas.**

- Arquitetura dual de LLMs e **pipeline de 7 estágios**.
- **JSON Schema** com 28 campos, ontologia controlada e **rubrica RV-DIA de 10 dimensões**.
- **RAG** com sqlite-vec / BGE-m3, **LoRA/QLoRA** para adaptação.
- Integração com **H5P, SCORM, cmi5, xAPI, BPMN 2.0 e Moodle**.

**Resultado.** Qualidade editorial, alinhamento curricular, aprendizagem ativa e rastreabilidade integrados em um fluxo único de produção.

**Em uma frase.** Desenvolvi uma abordagem de IA educacional voltada à produção didática com critério — controlar estrutura, qualidade, alinhamento, revisão, evidências e integração, não apenas gerar texto.
