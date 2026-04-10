# EstoqueCP — Gestão de Materiais 📦

> PWA premium para gestão inteligente de materiais e estoque em condomínios.

![Version](https://img.shields.io/badge/versão-2.0-00e5b8?style=flat-square&labelColor=060a0e)
![PWA](https://img.shields.io/badge/PWA-instalável-00e5b8?style=flat-square&labelColor=060a0e)
![Offline](https://img.shields.io/badge/offline-suportado-3b9eff?style=flat-square&labelColor=060a0e)
![License](https://img.shields.io/badge/licença-MIT-a855f7?style=flat-square&labelColor=060a0e)

---

## ✨ Funcionalidades

- **Dashboard** com KPIs em tempo real
- **Cadastro de itens** com categorias, unidades e localização
- **Controle de estoque** com alertas automáticos de nível mínimo
- **Movimentos** de entrada e saída com histórico completo
- **Conferência** de inventário com checklist interativo
- **Relatórios** por categoria e período
- **Instalável** no PC (Windows/macOS/Linux) e mobile (iOS/Android)
- **100% offline** — dados salvos localmente via localStorage

---

## 🚀 Deploy no GitHub Pages

### 1. Crie o repositório

```bash
git init
git add .
git commit -m "feat: EstoqueCP v2.0 — PWA premium"
git branch -M main
git remote add origin https://github.com/SEU_USUARIO/estoquecp.git
git push -u origin main
```

### 2. Ative o GitHub Pages

1. Vá em **Settings → Pages**
2. Em *Source*, selecione **GitHub Actions**
3. O workflow `.github/workflows/deploy.yml` já está configurado
4. Aguarde o deploy (≈ 30 segundos)
5. Acesse: `https://SEU_USUARIO.github.io/estoquecp`

> **Alternativa rápida:** Em *Source* escolha `Deploy from a branch → main / root`

---

## 📱 Instalação no Mobile

### Android (Chrome / Edge)
1. Acesse a URL do GitHub Pages no Chrome
2. Toque no menu **⋮ → Adicionar à tela inicial**
3. Ou aguarde o banner de instalação aparecer automaticamente
4. O app é instalado como aplicativo nativo

### iOS (Safari)
1. Acesse a URL no **Safari** (obrigatório)
2. Toque no ícone **Compartilhar** ↑
3. Role até **Adicionar à Tela de Início**
4. Confirme o nome e toque em **Adicionar**

---

## 💻 Instalação no PC

### Chrome / Edge (Windows, macOS, Linux)
1. Acesse a URL do GitHub Pages
2. Clique no ícone **⊕** na barra de endereço (lado direito)
3. Clique em **Instalar**
4. O app abre em janela própria, sem barra do navegador

### Windows — Atalho na Área de Trabalho
- Após instalar pelo Chrome/Edge, o atalho é criado automaticamente no Menu Iniciar
- Crie um atalho na Área de Trabalho clicando com o botão direito → Enviar para → Área de trabalho

### macOS — Dock
- Após instalar, clique com o botão direito no ícone no Dock → **Manter no Dock**

---

## 🗂 Estrutura de Arquivos

```
estoquecp/
├── index.html              # App principal (SPA completo)
├── manifest.json           # PWA Manifest
├── sw.js                   # Service Worker (cache + offline)
├── favicon.ico             # Favicon
├── icons/
│   ├── icon-72.png
│   ├── icon-96.png
│   ├── icon-128.png
│   ├── icon-144.png
│   ├── icon-152.png
│   ├── icon-192.png
│   ├── icon-256.png
│   ├── icon-384.png
│   ├── icon-512.png
│   └── icon-maskable-512.png
├── splash/
│   ├── splash-iphone-x.png     (1125×2436)
│   ├── splash-iphone-8.png     (750×1334)
│   ├── splash-iphone-se.png    (640×1136)
│   ├── splash-ipad-pro.png     (2048×2732)
│   └── splash-ipad-air.png     (1668×2388)
├── screenshots/
│   ├── screenshot-desktop.png
│   └── screenshot-mobile.png
├── .github/
│   └── workflows/
│       └── deploy.yml          # Auto-deploy para GitHub Pages
├── .gitignore
└── README.md
```

---

## 🛠 Desenvolvimento Local

```bash
# Clone o repositório
git clone https://github.com/SEU_USUARIO/estoquecp.git
cd estoquecp

# Inicie um servidor local (qualquer um serve)
npx serve .
# ou
python3 -m http.server 8080
# ou
php -S localhost:8080

# Acesse: http://localhost:8080
```

> ⚠️ O Service Worker **requer HTTPS** em produção (GitHub Pages já oferece). Para desenvolvimento local, use `localhost` que é tratado como origem segura.

---

## 🎨 Design System

| Token | Valor | Uso |
|-------|-------|-----|
| `--accent` | `#00e5b8` | Cor principal, CTAs |
| `--bg` | `#060a0e` | Fundo do app |
| `--surface` | `#0c1118` | Cards e sidebar |
| `--text` | `#eef3f8` | Texto principal |
| `--sans` | Space Grotesk | UI principal |
| `--mono` | JetBrains Mono | Dados e labels |

---

## 📄 Licença

MIT © 2025 — EstoqueCP

---

<div align="center">
  Feito com ♥ para facilitar a gestão de condomínios brasileiros
</div>
