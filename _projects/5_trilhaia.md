---
layout: page
title: Hachura · PNLD 2027 — TRILHA-IA
description: Arquitetura de um motor de IA generativa com RAG híbrido e governança editorial para material didático.
img: assets/img/case_trilhaia.png
logo: assets/img/logos/hachura.png
importance: 2
theme: t2
category: educação digital
---

> **Nota de governança editorial.** Visão de alto nível do método; artefactos e dados de produção permanecem sob sigilo editorial.

**Período.** 2025–2026 · Editor Geral · Hachura Estúdio (coleção "Educação Digital", PNLD 2027).

**Contexto.** Produção e avaliação de material didático com **IA generativa controlada** — governar estrutura, qualidade, alinhamento curricular, revisão e rastreabilidade, não apenas gerar texto.

**Desafio.** Escalar a produção didática sem abrir mão de estrutura, alinhamento à BNCC, revisão e auditabilidade — requisitos inegociáveis em um edital como o PNLD.

**Arquitetura do TRILHA-IA (decisões técnicas).**

- **Pipeline de múltiplos estágios** com **arquitetura dual de LLMs** e **validação determinística** via **Pydantic** e **JSON Schema** (28 campos) — mitigando alucinações.
- **RAG híbrido**: embeddings **BGE-m3**, busca densa + esparsa (**BM25**) e **reranking** com Cross-Encoders, para fundamentação documental e rastreabilidade.
- **Ontologia controlada** e **rubrica RV-DIA de 10 dimensões** para avaliação; adaptação com **LoRA/QLoRA**.
- Integração com **H5P, SCORM, cmi5, xAPI, BPMN 2.0 e Moodle**.

**Entregáveis.** Motor TRILHA-IA; JSON Schema e ontologia; rubrica RV-DIA; pipeline RAG documentado; governança editorial do processo.

**Resultado.** Qualidade editorial, alinhamento curricular, aprendizagem ativa e rastreabilidade integrados em um fluxo único de produção.

**Stack.** LLMs · RAG (BGE-m3 · BM25 · reranking) · sqlite-vec · LoRA/QLoRA · Pydantic · JSON Schema · Python · H5P/SCORM/xAPI.

**Em uma frase.** Projetei um motor de IA educacional que controla estrutura, qualidade, alinhamento, revisão e rastreabilidade — engenharia de IA aplicada à produção didática.
