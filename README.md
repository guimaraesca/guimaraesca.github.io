# carlosarturguimaraes.com

Site pessoal de **Carlos Artur Guimarães** — cartão de visita profissional.
Página única estática, sem dependências de build, publicada via **GitHub Pages**.

- **Repositório-alvo:** `guimaraesca/guimaraesca.github.io`
- **Domínio:** `carlosarturguimaraes.com`
- **Idioma:** PT-BR

## Estrutura

```
.
├── index.html          # página única (nav, hero, sobre, experiência, formação, publicações, contato)
├── assets/
│   ├── styles.css       # design system "Sapien" (claro + dark mode)
│   ├── favicon.svg      # favicon (monograma CG)
│   └── og-image.png     # imagem de compartilhamento (1200×630)
├── CNAME                # domínio personalizado (GitHub Pages)
├── CONTEUDO.md          # fonte de conteúdo editável (edite aqui e replique no HTML)
└── README.md
```

Os ícones são SVG de linha embutidos no próprio `index.html` (herdam a cor do
tema). As fontes (Poppins + Inter) vêm do Google Fonts.

## Pré-visualizar localmente

Qualquer servidor estático serve. Exemplos:

```bash
python3 -m http.server 8000
```

Depois abra `http://localhost:8000`. (Abrir o `index.html` direto com
`file://` também funciona, mas um servidor local reproduz melhor o comportamento
real.)

## Publicar no GitHub Pages

> ⚠️ Nada aqui foi commitado/empurrado automaticamente. Os passos abaixo são
> manuais, para você executar quando aprovar o conteúdo.

1. **Criar o repositório** (se ainda não existir) chamado exatamente
   `guimaraesca.github.io` na conta `guimaraesca`.

2. **Enviar os arquivos** a partir desta pasta:

   ```bash
   git add .
   git commit -m "site: cartão de visita profissional"
   git branch -M main
   git remote add origin https://github.com/guimaraesca/guimaraesca.github.io.git
   git push -u origin main
   ```

3. **Ativar o Pages:** em *Settings → Pages*, defina a *Source* como
   `Deploy from a branch`, branch `main`, pasta `/ (root)`. Para repositórios
   `usuario.github.io` o Pages geralmente já publica a partir de `main`.

4. **Domínio personalizado:** o arquivo `CNAME` já contém
   `carlosarturguimaraes.com`. Em *Settings → Pages → Custom domain*, confirme
   o domínio e marque **Enforce HTTPS** após a validação.

5. **DNS** (no provedor do domínio `carlosarturguimaraes.com`):
   - Registros **A** do apex para os IPs do GitHub Pages:
     `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - (Opcional) **AAAA** para IPv6:
     `2606:50c0:8000::153`, `2606:50c0:8001::153`, `2606:50c0:8002::153`, `2606:50c0:8003::153`
   - **CNAME** do subdomínio `www` apontando para `guimaraesca.github.io`.

   > Confira os IPs atuais na documentação oficial do GitHub Pages antes de
   > configurar o DNS, pois podem mudar.

A propagação de DNS e a emissão do certificado HTTPS podem levar de alguns
minutos a algumas horas.

## Acessibilidade e desempenho

- Semântica HTML real (`<header>`, `<main>`, `<section>`, `<nav>`, listas, `<a>`/`<button>`).
- Contraste WCAG AA, foco visível, `aria-label`/`aria-hidden`, skip-link.
- `prefers-color-scheme` (dark mode) e `prefers-reduced-motion`.
- Mobile-first; sem frameworks; apenas HTML + CSS + um pequeno script para o menu.

## Manutenção de conteúdo

Edite `CONTEUDO.md` (fonte legível) e replique as mudanças em `index.html`.
Regras de integridade seguidas: apenas itens verificados; sem valores em R$;
sem CPF/dados pessoais; sem métricas fabricadas; logos de terceiros apenas com
arquivo oficial (por ora, wordmark em texto).
