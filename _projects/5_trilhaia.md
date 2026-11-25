---
layout: page
title: Hachura · PNLD 2027 — TRILHA-IA
description: IA generativa com governança editorial para produção de material didático.
img: assets/img/case_trilhaia.png
importance: 2
category: educação digital
---

> **Nota de governança editorial.** Visão de alto nível do método; artefactos e dados de produção permanecem sob sigilo editorial.

**Desafio.** Produzir e avaliar material didático (coleção "Educação Digital", PNLD 2027) com IA generativa **controlada** — não apenas gerar texto, mas governar estrutura, qualidade, alinhamento curricular, revisão e rastreabilidade.

**Papel e decisões.** Editor Geral e concepção do **TRILHA-IA**, motor de produção com IA generativa:

- Arquitetura dual de LLMs e **pipeline de 7 estágios**.
- **JSON Schema** com 28 campos, ontologia controlada e **rubrica RV-DIA de 10 dimensões**.
- **RAG** (sqlite-vec / BGE-m3), LoRA/QLoRA.
- Integração com H5P, SCORM, cmi5, xAPI, BPMN 2.0 e Moodle.

**Resultado.** Qualidade editorial, alinhamento curricular, aprendizagem ativa e rastreabilidade integrados em um fluxo único de produção.
