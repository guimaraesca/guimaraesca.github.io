---
layout: page
title: Hachura · PNLD 2027 — TRILHA-IA
description: Motor de IA generativa com RAG híbrido, validação determinística e governança editorial para livro didático.
img: assets/img/case_trilhaia.png
logo: assets/img/logos/hachura.png
importance: 1
theme: t3
audience: Setor privado
---

<p class="case-meta" style="--c:#0E7C86"><b>Inovação</b> · Setor privado (editorial) · 2025–2026 · Editor Geral — Hachura Estúdio, coleção Educação Digital (PNLD 2027)</p>

> Artefatos e dados de produção estão sob confidencialidade editorial; o case mostra o método.

**Contexto.** Uso controlado de IA generativa na produção e avaliação de livro didático. O objetivo não era só gerar texto, mas **governar estrutura, qualidade, alinhamento curricular, revisão e rastreabilidade**.

**Problema.** Escalar a produção de uma coleção mantendo estrutura, aderência à BNCC, revisão e auditabilidade — exigências centrais do edital do PNLD.

**O que fiz.**

- **Pipeline multietapa** com dois LLMs e **validação determinística** por **Pydantic e JSON Schema de 28 campos**: saída fora do esquema não avança.
- **RAG híbrido** com embeddings **BGE-m3**, recuperação densa e esparsa (**BM25**) e **reranking por Cross-Encoder**, para ancorar cada conteúdo em documento-fonte rastreável.
- **Ontologia controlada** e **rubrica RV-DIA de 10 dimensões** para avaliar a saída, com adaptação de modelo via **LoRA/QLoRA**.
- **Interoperabilidade editorial e pedagógica:** H5P, SCORM, cmi5, xAPI, BPMN 2.0 e Moodle.

**Entregas.** Motor TRILHA-IA, JSON Schema e ontologia, rubrica RV-DIA, pipeline RAG documentado e processo de governança editorial.

**Stack.** LLMs · RAG (BGE-m3, BM25, Cross-Encoder) · sqlite-vec · LoRA/QLoRA · Pydantic · JSON Schema · Python · H5P · SCORM · cmi5 · xAPI

**Síntese.** IA generativa em produto educacional precisa de **governança embutida no pipeline** — esquema, fonte, rubrica e revisão — para que velocidade não custe qualidade nem rastreabilidade.
