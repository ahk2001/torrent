# 🚗 Autoescuela Torrent — Website Oficial & Landing Page de Alta Conversão

[![Deploy to GitHub Pages](https://github.com/ahk2001/torrent/actions/workflows/deploy.yml/badge.svg)](https://github.com/ahk2001/torrent/actions/workflows/deploy.yml)
[![Status: Production Ready](https://img.shields.io/badge/Status-Production%20Ready-success.svg)](https://github.com/ahk2001/torrent)
[![License: Proprietary](https://img.shields.io/badge/License-Proprietary-blue.svg)](LICENSE)

> Plataforma web de alta performance e design institucional desenvolvida para a **Autoescuela Torrent** (Academia de Conductores Torrent S.L.), referência há mais de 40 anos na formação de condutores em Torrent e Valência, Espanha.

---

## 📌 Visão Geral do Projeto

O projeto foi construído focado em:
- **Experiência do Usuário (UX/UI)**: Design limpo, paleta de cores corporativa, tipografia premium (`Inter Tight`, `Plus Jakarta Sans`, `JetBrains Mono`) e componentes responsivos.
- **Alta Conversão**: Fluxos diretos para atendimento via WhatsApp com mensagens pré-formatadas, botões de ação e números de contato direto.
- **Performance & SEO**: Estrutura semântica HTML5, imagens em formato WebP otimizado, meta tags Open Graph completas, tags canônicas, `robots.txt` e `sitemap.xml`.
- **Segurança**: Políticas restritas de permissão no CI/CD, prevenção de exposição de dados com `.gitignore` robusto e links externos com proteção `rel="noopener"`.

---

## 📁 Estrutura de Diretórios

```text
torrent/
├── .github/
│   └── workflows/
│       └── deploy.yml          # Pipeline CI/CD automatizado para GitHub Pages
├── assets/                     # Recursos visuais (imagens, logotipos, ícones WebP/PNG)
├── docs/                       # Documentação interna, briefing e dossiê
│   ├── dados.txt               # Dados e links oficiais de referência
│   └── dossie_autoescola.md    # Dossiê de pesquisa de mercado e conteúdo
├── .gitignore                  # Regras de exclusão de arquivos temporários e sensíveis
├── favicon.ico                 # Favicon raiz do site
├── index.html                  # Landing page principal em HTML5/CSS3/JS puro
├── README.md                   # Documentação oficial do projeto
├── robots.txt                  # Diretrizes para indexadores e motores de busca
└── sitemap.xml                 # Mapa do site para indexação de motores de busca
```

---

## 🚀 Como Executar Localmente

Como o projeto é estático e não requer dependências de compilação ou bundlers pesados, basta servi-lo com qualquer servidor web HTTP estático:

### Opção 1: VS Code Live Server
Basta clicar com o botão direito em `index.html` e selecionar **Open with Live Server**.

### Opção 2: Python HTTP Server
```bash
python -m http.server 8000
```
Acesse no navegador: `http://localhost:8000`

### Opção 3: Node.js (npx serve)
```bash
npx serve .
```

---

## 🌐 Deploy e Hospedagem

### GitHub Pages (Configuração Automática)
1. O repositório já conta com workflow em `.github/workflows/deploy.yml`.
2. No GitHub, vá em **Settings** > **Pages**.
3. Em **Build and deployment** > **Source**, selecione **GitHub Actions**.
4. Qualquer push na branch `main` dispara o deploy seguro automaticamente.

### Outras Plataformas Suportadas
- **Vercel**: Importe o repositório diretamente; a detecção de site estático é imediata.
- **Netlify**: Basta arrastar a pasta ou conectar o repositório (diretório base: `/`, comando de build vazio).
- **Cloudflare Pages**: Conexão Git nativa com distribuição global por CDN.

---

## 🔒 Segurança e Boas Práticas

- Nenhum dado confidencial ou chave de API está exposto no código fonte.
- Links externos utilizam o atributo `rel="noopener"` para mitigar riscos de segurança.
- O pipeline de deploy possui permissões mínimas (`contents: read`, `pages: write`, `id-token: write`).
- `.gitignore` configurado para impedir inclusão inadvertida de arquivos locais do sistema e senhas.

---

## 🏢 Contato da Empresa

- **Autoescuela Torrent** — Sede Principal: Avinguda al Vedat 103, Torrent, Valência
- **Pista Própria de Manobras**: Carrer dels Traginers 3, Polígon Industrial Mas del Jutge, Torrent
- **WhatsApp**: [+34 607 401 892](https://wa.me/34607401892)
- **Website Oficial**: [autoescuelatorrent.com](https://www.autoescuelatorrent.com/)
