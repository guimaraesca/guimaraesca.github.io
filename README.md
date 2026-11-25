# guimaraesca.github.io

Site pessoal de **Carlos Artur Guimarães** — governança de dados para a educação pública.
Construído com **[al-folio](https://github.com/alshedivat/al-folio)** (Jekyll), publicado em
**https://guimaraesca.github.io/**.

## Como funciona
- Conteúdo em `_pages/` (sobre, cases, publicações, cv), cases em `_projects/`,
  publicações em `_bibliography/papers.bib`, CV em `_data/cv.yml`.
- O tema (layouts/estilos) vem dos gems `al_folio_*` (al-folio v1 é um *starter* fino).
- **Build e deploy automáticos** via GitHub Actions (`.github/workflows/deploy.yml`):
  a cada push na `main`, o site é compilado e publicado na branch `gh-pages`,
  que o GitHub Pages serve.

## Editar
- Texto da home: `_pages/about.md`
- Cases (um arquivo por case, com nota de governança onde há sigilo): `_projects/*.md`
- Publicações: `_bibliography/papers.bib`
- Currículo: `_data/cv.yml`
- Identidade/configuração: `_config.yml`

Integridade: sem valores em R$, sem CPF/dados pessoais; logos de terceiros como texto;
a menção honrosa do Google Play (projeto "Lucy") consta como orientação da estudante.
