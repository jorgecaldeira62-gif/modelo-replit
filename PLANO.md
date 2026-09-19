# PLANO DO PROJETO: modelo Replit

> Gerado automaticamente pelo SK Code Editor em 19/09/2026, 08:54:19
> **208 arquivo(s)** | **~42.587 linhas de codigo**

---

## RESUMO EXECUTIVO

- **Tipo de aplicacao:** Aplicacao Web Frontend (React)
- **Frontend / Stack principal:** React, TypeScript

**Para rodar o projeto:**
```bash
# Abra index.html no Preview (botao Play)
```

---

## ESTRUTURA DE ARQUIVOS

```
modelo Replit/
├── api-server/
│   ├── .replit-artifact/
│   │   └── artifact.toml
│   ├── src/
│   │   ├── lib/
│   │   │   ├── logger.ts
│   │   │   └── terminal.ts
│   │   ├── routes/
│   │   │   ├── aiProcess.ts
│   │   │   ├── ghProxy.ts
│   │   │   ├── health.ts
│   │   │   ├── index.ts
│   │   │   └── siteExtract.ts
│   │   ├── app.ts
│   │   └── index.ts
│   ├── build.mjs
│   ├── package.json
│   └── tsconfig.json
├── code-editor/
│   ├── .replit-artifact/
│   │   └── artifact.toml
│   ├── desktop/
│   │   ├── app/
│   │   │   ├── extrator.html
│   │   │   ├── favicon.svg
│   │   │   ├── index.html
│   │   │   ├── manifest.json
│   │   │   └── sw.js
│   │   ├── package.json
│   │   ├── server_main.js
│   │   └── server.js
│   ├── dist-apk/
│   │   ├── extrator.html
│   │   ├── favicon.svg
│   │   ├── index.html
│   │   ├── manifest.json
│   │   └── sw.js
│   ├── dist-standalone/
│   │   ├── assets/
│   │   │   └── index-CQchCeow.css
│   │   ├── favicon.svg
│   │   ├── index.html
│   │   ├── manifest.json
│   │   └── sw.js
│   ├── public/
│   │   ├── extrator.html
│   │   ├── favicon.svg
│   │   ├── manifest.json
│   │   └── sw.js
│   ├── src/
│   │   ├── components/
│   │   │   ├── ui/
│   │   │   │   ├── accordion.tsx
│   │   │   │   ├── alert-dialog.tsx
│   │   │   │   ├── alert.tsx
│   │   │   │   ├── aspect-ratio.tsx
│   │   │   │   ├── avatar.tsx
│   │   │   │   ├── badge.tsx
│   │   │   │   ├── breadcrumb.tsx
│   │   │   │   ├── button-group.tsx
│   │   │   │   ├── button.tsx
│   │   │   │   ├── calendar.tsx
│   │   │   │   ├── card.tsx
│   │   │   │   ├── carousel.tsx
│   │   │   │   ├── chart.tsx
│   │   │   │   ├── checkbox.tsx
│   │   │   │   ├── collapsible.tsx
│   │   │   │   ├── command.tsx
│   │   │   │   ├── context-menu.tsx
│   │   │   │   ├── dialog.tsx
│   │   │   │   ├── drawer.tsx
│   │   │   │   ├── dropdown-menu.tsx
│   │   │   │   ├── empty.tsx
│   │   │   │   ├── field.tsx
│   │   │   │   ├── form.tsx
│   │   │   │   ├── hover-card.tsx
│   │   │   │   ├── input-group.tsx
│   │   │   │   ├── input-otp.tsx
│   │   │   │   ├── input.tsx
│   │   │   │   ├── item.tsx
│   │   │   │   ├── kbd.tsx
│   │   │   │   ├── label.tsx
│   │   │   │   ├── menubar.tsx
│   │   │   │   ├── navigation-menu.tsx
│   │   │   │   ├── pagination.tsx
│   │   │   │   ├── popover.tsx
│   │   │   │   ├── progress.tsx
│   │   │   │   ├── radio-group.tsx
│   │   │   │   ├── resizable.tsx
│   │   │   │   ├── scroll-area.tsx
│   │   │   │   ├── select.tsx
│   │   │   │   ├── separator.tsx
│   │   │   │   ├── sheet.tsx
│   │   │   │   ├── sidebar.tsx
│   │   │   │   ├── skeleton.tsx
│   │   │   │   ├── slider.tsx
│   │   │   │   ├── sonner.tsx
│   │   │   │   ├── spinner.tsx
│   │   │   │   ├── switch.tsx
│   │   │   │   ├── table.tsx
│   │   │   │   ├── tabs.tsx
│   │   │   │   ├── textarea.tsx
│   │   │   │   ├── toast.tsx
│   │   │   │   ├── toaster.tsx
│   │   │   │   ├── toggle-group.tsx
│   │   │   │   ├── toggle.tsx
│   │   │   │   └── tooltip.tsx
│   │   │   ├── AbrirOnline.tsx
│   │   │   ├── AIChat.tsx
│   │   │   ├── AssistenteJuridico.tsx
│   │   │   ├── BrowserTerminal.tsx
│   │   │   ├── CampoLivre.tsx
│   │   │   ├── CodeEditor.tsx
│   │   │   ├── DriveBackupPanel.tsx
│   │   │   ├── EditorLayout.tsx
│   │   │   ├── Extrator.tsx
│   │   │   ├── FileTree.tsx
│   │   │   ├── GitHubPanel.tsx
│   │   │   ├── InAppBrowser.tsx
│   │   │   ├── manual.tsx
│   │   │   ├── PackageSearch.tsx
│   │   │   ├── Preview.tsx
│   │   │   ├── QuickPrompt.tsx
│   │   │   ├── RealTerminal.tsx
│   │   │   ├── Scanner.tsx
│   │   │   ├── StreamTerminal.tsx
│   │   │   ├── TemplateSelector.tsx
│   │   │   ├── Terminal.tsx
│   │   │   ├── VoiceCard.tsx
│   │   │   └── VoiceMode.tsx
│   │   ├── hooks/
│   │   │   ├── use-mobile.tsx
│   │   │   └── use-toast.ts
│   │   ├── lib/
│   │   │   ├── ai-service.ts
│   │   │   ├── github-service.ts
│   │   │   ├── projects.ts
│   │   │   ├── store.ts
│   │   │   ├── templates.ts
│   │   │   ├── tts-service.ts
│   │   │   ├── utils.ts
│   │   │   ├── virtual-fs.ts
│   │   │   └── zip-service.ts
│   │   ├── pages/
│   │   │   └── not-found.tsx
│   │   ├── App.tsx
│   │   ├── index.css
│   │   └── main.tsx
│   ├── capacitor.config.ts
│   ├── components.json
│   ├── index.html
│   ├── MANUAL-APK.md
│   ├── package.json
│   ├── tsconfig.json
│   ├── vite.config.apk.ts
│   ├── vite.config.standalone.ts
│   └── vite.config.ts
├── mockup-sandbox/
│   ├── .replit-artifact/
│   │   └── artifact.toml
│   ├── src/
│   │   ├── .generated/
│   │   │   └── mockup-components.ts
│   │   ├── components/
│   │   │   └── ui/
│   │   │       ├── accordion.tsx
│   │   │       ├── alert-dialog.tsx
│   │   │       ├── alert.tsx
│   │   │       ├── aspect-ratio.tsx
│   │   │       ├── avatar.tsx
│   │   │       ├── badge.tsx
│   │   │       ├── breadcrumb.tsx
│   │   │       ├── button-group.tsx
│   │   │       ├── button.tsx
│   │   │       ├── calendar.tsx
│   │   │       ├── card.tsx
│   │   │       ├── carousel.tsx
│   │   │       ├── chart.tsx
│   │   │       ├── checkbox.tsx
│   │   │       ├── collapsible.tsx
│   │   │       ├── command.tsx
│   │   │       ├── context-menu.tsx
│   │   │       ├── dialog.tsx
│   │   │       ├── drawer.tsx
│   │   │       ├── dropdown-menu.tsx
│   │   │       ├── empty.tsx
│   │   │       ├── field.tsx
│   │   │       ├── form.tsx
│   │   │       ├── hover-card.tsx
│   │   │       ├── input-group.tsx
│   │   │       ├── input-otp.tsx
│   │   │       ├── input.tsx
│   │   │       ├── item.tsx
│   │   │       ├── kbd.tsx
│   │   │       ├── label.tsx
│   │   │       ├── menubar.tsx
│   │   │       ├── navigation-menu.tsx
│   │   │       ├── pagination.tsx
│   │   │       ├── popover.tsx
│   │   │       ├── progress.tsx
│   │   │       ├── radio-group.tsx
│   │   │       ├── resizable.tsx
│   │   │       ├── scroll-area.tsx
│   │   │       ├── select.tsx
│   │   │       ├── separator.tsx
│   │   │       ├── sheet.tsx
│   │   │       ├── sidebar.tsx
│   │   │       ├── skeleton.tsx
│   │   │       ├── slider.tsx
│   │   │       ├── sonner.tsx
│   │   │       ├── spinner.tsx
│   │   │       ├── switch.tsx
│   │   │       ├── table.tsx
│   │   │       ├── tabs.tsx
│   │   │       ├── textarea.tsx
│   │   │       ├── toast.tsx
│   │   │       ├── toaster.tsx
│   │   │       ├── toggle-group.tsx
│   │   │       ├── toggle.tsx
│   │   │       └── tooltip.tsx
│   │   ├── hooks/
│   │   │   ├── use-mobile.tsx
│   │   │   └── use-toast.ts
│   │   ├── lib/
│   │   │   └── utils.ts
│   │   ├── App.tsx
│   │   ├── index.css
│   │   └── main.tsx
│   ├── components.json
│   ├── index.html
│   ├── mockupPreviewPlugin.ts
│   ├── package.json
│   ├── tsconfig.json
│   └── vite.config.ts
└── PLANO.md
```

---

## STACK TECNOLOGICO DETECTADO

- **Frontend:** React, TypeScript

---

## ROTAS DA API (endpoints detectados automaticamente)

```
USE    /api  (em api-server/src/app.ts)
POST   /ai/process  (em api-server/src/routes/aiProcess.ts)
POST   /code-assistant  (em api-server/src/routes/aiProcess.ts)
GET    /gh-proxy/zipball  (em api-server/src/routes/ghProxy.ts)
GET    /gh-proxy/repo  (em api-server/src/routes/ghProxy.ts)
GET    /healthz  (em api-server/src/routes/health.ts)
GET    /config  (em api-server/src/routes/index.ts)
POST   /site-extract  (em api-server/src/routes/siteExtract.ts)
GET    /site-extract/proxy  (em api-server/src/routes/siteExtract.ts)
GET    /api/items  (em code-editor/src/lib/templates.ts)
GET    /api/items/:id  (em code-editor/src/lib/templates.ts)
POST   /api/items  (em code-editor/src/lib/templates.ts)
GET    /api/health  (em code-editor/src/lib/templates.ts)
USE    /api/auth  (em code-editor/src/lib/templates.ts)
USE    /api/usuarios  (em code-editor/src/lib/templates.ts)
POST   /register  (em code-editor/src/lib/templates.ts)
POST   /login  (em code-editor/src/lib/templates.ts)
GET    /perfil  (em code-editor/src/lib/templates.ts)
```

---

## VARIAVEIS DE AMBIENTE NECESSARIAS

Crie um arquivo `.env` na raiz com estas variaveis:

```env
LOG_LEVEL=seu_valor_aqui
PORT=seu_valor_aqui
ALLOWED_ORIGINS=seu_valor_aqui
JWT_SECRET=seu_valor_aqui
JWT_EXPIRES_IN=seu_valor_aqui
DATABASE_URL=seu_valor_aqui
BASE_PATH=seu_valor_aqui
REPL_ID=seu_valor_aqui
```

---

## ARQUIVOS PRINCIPAIS

- `api-server/src/app.ts` — Ponto de entrada do backend
- `api-server/src/index.ts` — Ponto de entrada do backend
- `api-server/src/routes/index.ts` — Ponto de entrada do backend
- `code-editor/desktop/app/index.html` — Arquivo principal
- `code-editor/desktop/server.js` — Ponto de entrada do backend
- `code-editor/dist-apk/index.html` — Arquivo principal
- `code-editor/dist-standalone/index.html` — Arquivo principal
- `code-editor/index.html` — Arquivo principal
- `code-editor/src/App.tsx` — Componente raiz do frontend
- `code-editor/src/main.tsx` — Arquivo principal

---

## GUIA COMPLETO — O QUE CADA PARTE DO PROJETO FAZ

> Esta secao explica, em linguagem simples, o que e para que serve cada pasta e cada arquivo.

### 📁 Raiz do Projeto (pasta principal)
> Arquivos de configuracao e pontos de entrada ficam aqui.

**`PLANO.md`** _(3568 linhas)_
Este documento! Gerado automaticamente pelo SK Code Editor com toda a estrutura do projeto.

---

### 📁 `api-server/`
> Pasta 'api-server' — agrupamento de arquivos relacionados.

**`build.mjs`** _(127 linhas)_
Arquivo MJS — parte do projeto.

**`package.json`** _(38 linhas)_
Registro de dependencias e scripts do projeto. Aqui ficam os comandos (npm run dev, npm start) e os pacotes instalados.

**`tsconfig.json`** _(18 linhas)_
Configuracao do TypeScript. Diz para o computador como interpretar o codigo .ts e .tsx.

---

### 📁 `code-editor/`
> Pasta 'code-editor' — agrupamento de arquivos relacionados.

**`MANUAL-APK.md`** _(258 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`capacitor.config.ts`** _(24 linhas)_
Arquivo de CONSTANTES/CONFIGURACAO — valores fixos usados em varios lugares do projeto.

**`components.json`** _(20 linhas)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

**`index.html`** _(28 linhas)_
Pagina HTML raiz do projeto. E o ponto de entrada que o browser carrega primeiro.

**`package.json`** _(129 linhas)_
Registro de dependencias e scripts do projeto. Aqui ficam os comandos (npm run dev, npm start) e os pacotes instalados.

**`tsconfig.json`** _(16 linhas)_
Configuracao do TypeScript. Diz para o computador como interpretar o codigo .ts e .tsx.

**`vite.config.apk.ts`** _(29 linhas)_
Arquivo de CONSTANTES/CONFIGURACAO — valores fixos usados em varios lugares do projeto.

**`vite.config.standalone.ts`** _(22 linhas)_
Arquivo de CONSTANTES/CONFIGURACAO — valores fixos usados em varios lugares do projeto.

**`vite.config.ts`** _(74 linhas)_
Configuracao do Vite (servidor de desenvolvimento). Define a porta, alias de caminhos e plugins usados.

---

### 📁 `mockup-sandbox/`
> Pasta 'mockup-sandbox' — agrupamento de arquivos relacionados.

**`components.json`** _(22 linhas)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

**`index.html`** _(32 linhas)_
Pagina HTML raiz do projeto. E o ponto de entrada que o browser carrega primeiro.

**`mockupPreviewPlugin.ts`** _(181 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`package.json`** _(75 linhas)_
Registro de dependencias e scripts do projeto. Aqui ficam os comandos (npm run dev, npm start) e os pacotes instalados.

**`tsconfig.json`** _(17 linhas)_
Configuracao do TypeScript. Diz para o computador como interpretar o codigo .ts e .tsx.

**`vite.config.ts`** _(73 linhas)_
Configuracao do Vite (servidor de desenvolvimento). Define a porta, alias de caminhos e plugins usados.

---

### 📁 `api-server/.replit-artifact/`
> Pasta '.replit-artifact' — agrupamento de arquivos relacionados.

**`artifact.toml`** _(33 linhas)_
Arquivo TOML — parte do projeto.

---

### 📁 `api-server/src/`
> Codigo-fonte principal do projeto. Nao apague esta pasta.

**`app.ts`** _(35 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`index.ts`** _(44 linhas)_
Arquivo INDEX — ponto de entrada da pasta, exporta tudo que esta dentro.

---

### 📁 `code-editor/.replit-artifact/`
> Pasta '.replit-artifact' — agrupamento de arquivos relacionados.

**`artifact.toml`** _(32 linhas)_
Arquivo TOML — parte do projeto.

---

### 📁 `code-editor/desktop/`
> Pasta 'desktop' — agrupamento de arquivos relacionados.

**`package.json`** _(19 linhas)_
Registro de dependencias e scripts do projeto. Aqui ficam os comandos (npm run dev, npm start) e os pacotes instalados.

**`server.js`** _(95 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`server_main.js`** _(73 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `code-editor/dist-apk/`
> Pasta 'dist-apk' — agrupamento de arquivos relacionados.

**`extrator.html`** _(920 linhas)_
Arquivo HTML — parte do projeto.

**`favicon.svg`** _(17 linhas)_
Imagem vetorial (icone ou ilustracao que nao perde qualidade ao ampliar).

**`index.html`** _(28 linhas)_
Pagina HTML raiz do projeto. E o ponto de entrada que o browser carrega primeiro.

**`manifest.json`** _(49 linhas)_
Manifesto do PWA — define nome, icone e configuracoes para instalar o app no celular.

**`sw.js`** _(41 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `code-editor/dist-standalone/`
> Pasta 'dist-standalone' — agrupamento de arquivos relacionados.

**`favicon.svg`** _(17 linhas)_
Imagem vetorial (icone ou ilustracao que nao perde qualidade ao ampliar).

**`index.html`** _(37 linhas)_
Pagina HTML raiz do projeto. E o ponto de entrada que o browser carrega primeiro.

**`manifest.json`** _(49 linhas)_
Manifesto do PWA — define nome, icone e configuracoes para instalar o app no celular.

**`sw.js`** _(41 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `code-editor/public/`
> Arquivos estaticos: imagens, icones, fontes, arquivos publicos.

**`extrator.html`** _(920 linhas)_
Arquivo HTML — parte do projeto.

**`favicon.svg`** _(17 linhas)_
Imagem vetorial (icone ou ilustracao que nao perde qualidade ao ampliar).

**`manifest.json`** _(49 linhas)_
Manifesto do PWA — define nome, icone e configuracoes para instalar o app no celular.

**`sw.js`** _(41 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `code-editor/src/`
> Codigo-fonte principal do projeto. Nao apague esta pasta.

**`App.tsx`** _(254 linhas)_
Componente RAIZ do frontend — e o pai de todos os outros componentes. Aqui ficam as rotas principais.

**`index.css`** _(269 linhas)_
Arquivo de estilos visuais — cores, tamanhos, fontes, espacamentos da interface.

**`main.tsx`** _(6 linhas)_
Ponto de entrada do React — monta o componente App na pagina HTML.

---

### 📁 `mockup-sandbox/.replit-artifact/`
> Pasta '.replit-artifact' — agrupamento de arquivos relacionados.

**`artifact.toml`** _(18 linhas)_
Arquivo TOML — parte do projeto.

---

### 📁 `mockup-sandbox/src/`
> Codigo-fonte principal do projeto. Nao apague esta pasta.

**`App.tsx`** _(147 linhas)_
Componente RAIZ do frontend — e o pai de todos os outros componentes. Aqui ficam as rotas principais.

**`index.css`** _(158 linhas)_
Arquivo de estilos visuais — cores, tamanhos, fontes, espacamentos da interface.

**`main.tsx`** _(6 linhas)_
Ponto de entrada do React — monta o componente App na pagina HTML.

---

### 📁 `api-server/src/lib/`
> Funcoes auxiliares reutilizaveis em varios lugares do projeto.

**`logger.ts`** _(21 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`terminal.ts`** _(113 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `api-server/src/routes/`
> Definicao das URLs e navegacao do app.

**`aiProcess.ts`** _(209 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`ghProxy.ts`** _(90 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`health.ts`** _(12 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`index.ts`** _(27 linhas)_
Arquivo INDEX — ponto de entrada da pasta, exporta tudo que esta dentro.

**`siteExtract.ts`** _(456 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `code-editor/desktop/app/`
> Pasta 'app' — agrupamento de arquivos relacionados.

**`extrator.html`** _(920 linhas)_
Arquivo HTML — parte do projeto.

**`favicon.svg`** _(17 linhas)_
Imagem vetorial (icone ou ilustracao que nao perde qualidade ao ampliar).

**`index.html`** _(36 linhas)_
Pagina HTML raiz do projeto. E o ponto de entrada que o browser carrega primeiro.

**`manifest.json`** _(49 linhas)_
Manifesto do PWA — define nome, icone e configuracoes para instalar o app no celular.

**`sw.js`** _(41 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `code-editor/dist-standalone/assets/`
> Arquivos estaticos: imagens, icones, fontes, arquivos publicos.

**`index-CQchCeow.css`** _(2 linhas)_
Arquivo de estilos visuais — cores, tamanhos, fontes, espacamentos da interface.

---

### 📁 `code-editor/src/components/`
> Pecas visuais reutilizaveis da interface (botoes, cards, formularios...).

**`AIChat.tsx`** _(2370 linhas)_
Componente de CHAT/MENSAGENS — interface de conversa em tempo real.

**`AbrirOnline.tsx`** _(226 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`AssistenteJuridico.tsx`** _(1190 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`BrowserTerminal.tsx`** _(720 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`CampoLivre.tsx`** _(499 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`CodeEditor.tsx`** _(154 linhas)_
Componente EDITOR — area de edicao de texto, codigo ou conteudo rico.

**`DriveBackupPanel.tsx`** _(200 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`EditorLayout.tsx`** _(2568 linhas)_
Componente de LAYOUT — define a estrutura visual da pagina (cabecalho, sidebar, rodape). Envolve outros componentes.

**`Extrator.tsx`** _(824 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`FileTree.tsx`** _(400 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`GitHubPanel.tsx`** _(668 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`InAppBrowser.tsx`** _(148 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`PackageSearch.tsx`** _(415 linhas)_
Componente de BUSCA — campo e logica para filtrar/encontrar conteudo.

**`Preview.tsx`** _(496 linhas)_
Componente de PAGINA/TELA — representa uma tela completa navegavel no app.

**`QuickPrompt.tsx`** _(274 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`RealTerminal.tsx`** _(634 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`Scanner.tsx`** _(357 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`StreamTerminal.tsx`** _(495 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`TemplateSelector.tsx`** _(513 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`Terminal.tsx`** _(1516 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`VoiceCard.tsx`** _(427 linhas)_
Componente CARD (cartao) — exibe uma informacao em um bloco visual com borda e sombra. Muito usado para listas de items.

**`VoiceMode.tsx`** _(277 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`manual.tsx`** _(1726 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

---

### 📁 `code-editor/src/hooks/`
> Hooks React customizados — logica reutilizavel de estado e efeitos.

**`use-mobile.tsx`** _(20 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`use-toast.ts`** _(192 linhas)_
HOOK React personalizado para gerenciar estado/comportamento de '-toast'.

---

### 📁 `code-editor/src/lib/`
> Funcoes auxiliares reutilizaveis em varios lugares do projeto.

**`ai-service.ts`** _(446 linhas)_
Arquivo de SERVICO/API — funcoes para comunicar com o servidor ou API externa.

**`github-service.ts`** _(197 linhas)_
Arquivo de SERVICO/API — funcoes para comunicar com o servidor ou API externa.

**`projects.ts`** _(206 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`store.ts`** _(38 linhas)_
STORE de estado — gerencia o estado global do app (dados compartilhados entre telas).

**`templates.ts`** _(1629 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`tts-service.ts`** _(294 linhas)_
Arquivo de SERVICO/API — funcoes para comunicar com o servidor ou API externa.

**`utils.ts`** _(7 linhas)_
Funcoes UTILITARIAS — ferramentas reutilizaveis de uso geral no projeto.

**`virtual-fs.ts`** _(200 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`zip-service.ts`** _(246 linhas)_
Arquivo de SERVICO/API — funcoes para comunicar com o servidor ou API externa.

---

### 📁 `code-editor/src/pages/`
> Telas completas do app — cada arquivo aqui e uma pagina navegavel.

**`not-found.tsx`** _(22 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

---

### 📁 `mockup-sandbox/src/.generated/`
> Pasta '.generated' — agrupamento de arquivos relacionados.

**`mockup-components.ts`** _(6 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `mockup-sandbox/src/hooks/`
> Hooks React customizados — logica reutilizavel de estado e efeitos.

**`use-mobile.tsx`** _(20 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`use-toast.ts`** _(190 linhas)_
HOOK React personalizado para gerenciar estado/comportamento de '-toast'.

---

### 📁 `mockup-sandbox/src/lib/`
> Funcoes auxiliares reutilizaveis em varios lugares do projeto.

**`utils.ts`** _(7 linhas)_
Funcoes UTILITARIAS — ferramentas reutilizaveis de uso geral no projeto.

---

### 📁 `code-editor/src/components/ui/`
> Componentes de UI (interface) basicos e genericos.

**`accordion.tsx`** _(56 linhas)_
Componente ACCORDION — secoes que abrem/fecham ao clicar, economizando espaco na tela.

**`alert-dialog.tsx`** _(140 linhas)_
Componente de NOTIFICACAO/ALERTA — mensagem temporaria que aparece na tela (ex: 'Salvo com sucesso!').

**`alert.tsx`** _(60 linhas)_
Componente de NOTIFICACAO/ALERTA — mensagem temporaria que aparece na tela (ex: 'Salvo com sucesso!').

**`aspect-ratio.tsx`** _(6 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`avatar.tsx`** _(51 linhas)_
Componente AVATAR — foto ou iniciais do usuario em formato circular.

**`badge.tsx`** _(44 linhas)_
Componente BADGE (etiqueta) — pequeno indicador com numero ou status (ex: '3 novas mensagens').

**`breadcrumb.tsx`** _(116 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`button-group.tsx`** _(84 linhas)_
Componente de BOTAO — elemento clicavel reutilizavel com estilo padrao do projeto.

**`button.tsx`** _(66 linhas)_
Componente de BOTAO — elemento clicavel reutilizavel com estilo padrao do projeto.

**`calendar.tsx`** _(214 linhas)_
Componente CALENDARIO/AGENDA — visualizacao e selecao de datas e eventos.

**`card.tsx`** _(77 linhas)_
Componente CARD (cartao) — exibe uma informacao em um bloco visual com borda e sombra. Muito usado para listas de items.

**`carousel.tsx`** _(261 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`chart.tsx`** _(368 linhas)_
Componente de GRAFICO — visualizacao de dados em forma de grafico (barras, linhas, pizza...).

**`checkbox.tsx`** _(29 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`collapsible.tsx`** _(12 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`command.tsx`** _(154 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`context-menu.tsx`** _(199 linhas)_
CONTEXT do React — mecanismo para compartilhar dados entre componentes sem passar por props.

**`dialog.tsx`** _(121 linhas)_
Componente DIALOG — caixa de dialogo que exige resposta do usuario (confirmar, cancelar...).

**`drawer.tsx`** _(117 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`dropdown-menu.tsx`** _(202 linhas)_
Componente de MENU/DROPDOWN — lista de opcoes que aparece ao clicar em um botao.

**`empty.tsx`** _(105 linhas)_
Componente de ESTADO VAZIO — exibido quando nao ha dados para mostrar (ex: 'Nenhum resultado encontrado').

**`field.tsx`** _(245 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`form.tsx`** _(177 linhas)_
Componente de FORMULARIO — campos de entrada de dados (texto, selecao, etc.) com validacao.

**`hover-card.tsx`** _(28 linhas)_
Componente CARD (cartao) — exibe uma informacao em um bloco visual com borda e sombra. Muito usado para listas de items.

**`input-group.tsx`** _(169 linhas)_
Componente de CAMPO DE ENTRADA — elemento de input com estilo personalizado.

**`input-otp.tsx`** _(70 linhas)_
Componente de CAMPO DE ENTRADA — elemento de input com estilo personalizado.

**`input.tsx`** _(23 linhas)_
Componente de CAMPO DE ENTRADA — elemento de input com estilo personalizado.

**`item.tsx`** _(194 linhas)_
Componente de ITEM — representa um elemento individual dentro de uma lista ou colecao.

**`kbd.tsx`** _(29 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`label.tsx`** _(27 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`menubar.tsx`** _(255 linhas)_
Componente de MENU/DROPDOWN — lista de opcoes que aparece ao clicar em um botao.

**`navigation-menu.tsx`** _(129 linhas)_
Componente de NAVEGACAO/CABECALHO — barra superior com logo, menu e links de navegacao.

**`pagination.tsx`** _(118 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`popover.tsx`** _(32 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`progress.tsx`** _(29 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`radio-group.tsx`** _(43 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`resizable.tsx`** _(46 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`scroll-area.tsx`** _(47 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`select.tsx`** _(160 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`separator.tsx`** _(30 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`sheet.tsx`** _(141 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`sidebar.tsx`** _(728 linhas)_
Componente de BARRA LATERAL — menu ou painel que aparece na lateral da tela.

**`skeleton.tsx`** _(16 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`slider.tsx`** _(27 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`sonner.tsx`** _(32 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`spinner.tsx`** _(17 linhas)_
Componente de CARREGAMENTO — animacao visual que aparece enquanto dados estao sendo buscados.

**`switch.tsx`** _(28 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`table.tsx`** _(121 linhas)_
Componente de TABELA — exibe dados em linhas e colunas.

**`tabs.tsx`** _(54 linhas)_
Componente de ABAS — permite alternar entre diferentes secoes de conteudo com clique.

**`textarea.tsx`** _(23 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`toast.tsx`** _(128 linhas)_
Componente de NOTIFICACAO/ALERTA — mensagem temporaria que aparece na tela (ex: 'Salvo com sucesso!').

**`toaster.tsx`** _(34 linhas)_
Componente de NOTIFICACAO/ALERTA — mensagem temporaria que aparece na tela (ex: 'Salvo com sucesso!').

**`toggle-group.tsx`** _(62 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`toggle.tsx`** _(44 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`tooltip.tsx`** _(33 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

---

### 📁 `mockup-sandbox/src/components/ui/`
> Componentes de UI (interface) basicos e genericos.

**`accordion.tsx`** _(56 linhas)_
Componente ACCORDION — secoes que abrem/fecham ao clicar, economizando espaco na tela.

**`alert-dialog.tsx`** _(140 linhas)_
Componente de NOTIFICACAO/ALERTA — mensagem temporaria que aparece na tela (ex: 'Salvo com sucesso!').

**`alert.tsx`** _(60 linhas)_
Componente de NOTIFICACAO/ALERTA — mensagem temporaria que aparece na tela (ex: 'Salvo com sucesso!').

**`aspect-ratio.tsx`** _(6 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`avatar.tsx`** _(51 linhas)_
Componente AVATAR — foto ou iniciais do usuario em formato circular.

**`badge.tsx`** _(38 linhas)_
Componente BADGE (etiqueta) — pequeno indicador com numero ou status (ex: '3 novas mensagens').

**`breadcrumb.tsx`** _(116 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`button-group.tsx`** _(84 linhas)_
Componente de BOTAO — elemento clicavel reutilizavel com estilo padrao do projeto.

**`button.tsx`** _(59 linhas)_
Componente de BOTAO — elemento clicavel reutilizavel com estilo padrao do projeto.

**`calendar.tsx`** _(214 linhas)_
Componente CALENDARIO/AGENDA — visualizacao e selecao de datas e eventos.

**`card.tsx`** _(77 linhas)_
Componente CARD (cartao) — exibe uma informacao em um bloco visual com borda e sombra. Muito usado para listas de items.

**`carousel.tsx`** _(261 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`chart.tsx`** _(366 linhas)_
Componente de GRAFICO — visualizacao de dados em forma de grafico (barras, linhas, pizza...).

**`checkbox.tsx`** _(29 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`collapsible.tsx`** _(12 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`command.tsx`** _(154 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`context-menu.tsx`** _(199 linhas)_
CONTEXT do React — mecanismo para compartilhar dados entre componentes sem passar por props.

**`dialog.tsx`** _(121 linhas)_
Componente DIALOG — caixa de dialogo que exige resposta do usuario (confirmar, cancelar...).

**`drawer.tsx`** _(117 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`dropdown-menu.tsx`** _(202 linhas)_
Componente de MENU/DROPDOWN — lista de opcoes que aparece ao clicar em um botao.

**`empty.tsx`** _(105 linhas)_
Componente de ESTADO VAZIO — exibido quando nao ha dados para mostrar (ex: 'Nenhum resultado encontrado').

**`field.tsx`** _(245 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`form.tsx`** _(177 linhas)_
Componente de FORMULARIO — campos de entrada de dados (texto, selecao, etc.) com validacao.

**`hover-card.tsx`** _(28 linhas)_
Componente CARD (cartao) — exibe uma informacao em um bloco visual com borda e sombra. Muito usado para listas de items.

**`input-group.tsx`** _(166 linhas)_
Componente de CAMPO DE ENTRADA — elemento de input com estilo personalizado.

**`input-otp.tsx`** _(70 linhas)_
Componente de CAMPO DE ENTRADA — elemento de input com estilo personalizado.

**`input.tsx`** _(23 linhas)_
Componente de CAMPO DE ENTRADA — elemento de input com estilo personalizado.

**`item.tsx`** _(194 linhas)_
Componente de ITEM — representa um elemento individual dentro de uma lista ou colecao.

**`kbd.tsx`** _(29 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`label.tsx`** _(27 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`menubar.tsx`** _(255 linhas)_
Componente de MENU/DROPDOWN — lista de opcoes que aparece ao clicar em um botao.

**`navigation-menu.tsx`** _(129 linhas)_
Componente de NAVEGACAO/CABECALHO — barra superior com logo, menu e links de navegacao.

**`pagination.tsx`** _(118 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`popover.tsx`** _(32 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`progress.tsx`** _(29 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`radio-group.tsx`** _(43 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`resizable.tsx`** _(46 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`scroll-area.tsx`** _(47 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`select.tsx`** _(160 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`separator.tsx`** _(30 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`sheet.tsx`** _(141 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`sidebar.tsx`** _(715 linhas)_
Componente de BARRA LATERAL — menu ou painel que aparece na lateral da tela.

**`skeleton.tsx`** _(16 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`slider.tsx`** _(27 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`sonner.tsx`** _(32 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`spinner.tsx`** _(17 linhas)_
Componente de CARREGAMENTO — animacao visual que aparece enquanto dados estao sendo buscados.

**`switch.tsx`** _(28 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`table.tsx`** _(121 linhas)_
Componente de TABELA — exibe dados em linhas e colunas.

**`tabs.tsx`** _(54 linhas)_
Componente de ABAS — permite alternar entre diferentes secoes de conteudo com clique.

**`textarea.tsx`** _(23 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`toast.tsx`** _(128 linhas)_
Componente de NOTIFICACAO/ALERTA — mensagem temporaria que aparece na tela (ex: 'Salvo com sucesso!').

**`toaster.tsx`** _(34 linhas)_
Componente de NOTIFICACAO/ALERTA — mensagem temporaria que aparece na tela (ex: 'Salvo com sucesso!').

**`toggle-group.tsx`** _(62 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`toggle.tsx`** _(44 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`tooltip.tsx`** _(33 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

---

## CONTEXTO PARA IA (copie e cole para continuar o projeto)

> Use este bloco para explicar o projeto para qualquer IA ou desenvolvedor:

```
Projeto: modelo Replit
Tipo: Aplicacao Web Frontend (React)
Stack: React, TypeScript
Arquivos: 208 | Linhas: ~42.587
Rotas API: 18 endpoint(s) detectado(s)
Variaveis de ambiente necessarias: LOG_LEVEL, PORT, ALLOWED_ORIGINS, JWT_SECRET, JWT_EXPIRES_IN, DATABASE_URL, BASE_PATH, REPL_ID

Estrutura principal:
  PLANO.md
  api-server/.replit-artifact/artifact.toml
  api-server/build.mjs
  api-server/package.json
  api-server/src/app.ts
  api-server/src/index.ts
  api-server/src/lib/logger.ts
  api-server/src/lib/terminal.ts
  api-server/src/routes/aiProcess.ts
  api-server/src/routes/ghProxy.ts
  api-server/src/routes/health.ts
  api-server/src/routes/index.ts
  api-server/src/routes/siteExtract.ts
  api-server/tsconfig.json
  code-editor/.replit-artifact/artifact.toml
  code-editor/MANUAL-APK.md
  code-editor/capacitor.config.ts
  code-editor/components.json
  code-editor/desktop/app/extrator.html
  code-editor/desktop/app/favicon.svg
  code-editor/desktop/app/index.html
  code-editor/desktop/app/manifest.json
  code-editor/desktop/app/sw.js
  code-editor/desktop/package.json
  code-editor/desktop/server.js
  code-editor/desktop/server_main.js
  code-editor/dist-apk/extrator.html
  code-editor/dist-apk/favicon.svg
  code-editor/dist-apk/index.html
  code-editor/dist-apk/manifest.json
  code-editor/dist-apk/sw.js
  code-editor/dist-standalone/assets/index-CQchCeow.css
  code-editor/dist-standalone/favicon.svg
  code-editor/dist-standalone/index.html
  code-editor/dist-standalone/manifest.json
  code-editor/dist-standalone/sw.js
  code-editor/index.html
  code-editor/package.json
  code-editor/public/extrator.html
  code-editor/public/favicon.svg
  code-editor/public/manifest.json
  code-editor/public/sw.js
  code-editor/src/App.tsx
  code-editor/src/components/AIChat.tsx
  code-editor/src/components/AbrirOnline.tsx
  code-editor/src/components/AssistenteJuridico.tsx
  code-editor/src/components/BrowserTerminal.tsx
  code-editor/src/components/CampoLivre.tsx
  code-editor/src/components/CodeEditor.tsx
  code-editor/src/components/DriveBackupPanel.tsx
  code-editor/src/components/EditorLayout.tsx
  code-editor/src/components/Extrator.tsx
  code-editor/src/components/FileTree.tsx
  code-editor/src/components/GitHubPanel.tsx
  code-editor/src/components/InAppBrowser.tsx
  code-editor/src/components/PackageSearch.tsx
  code-editor/src/components/Preview.tsx
  code-editor/src/components/QuickPrompt.tsx
  code-editor/src/components/RealTerminal.tsx
  code-editor/src/components/Scanner.tsx
  code-editor/src/components/StreamTerminal.tsx
  code-editor/src/components/TemplateSelector.tsx
  code-editor/src/components/Terminal.tsx
  code-editor/src/components/VoiceCard.tsx
  code-editor/src/components/VoiceMode.tsx
  code-editor/src/components/manual.tsx
  code-editor/src/components/ui/accordion.tsx
  code-editor/src/components/ui/alert-dialog.tsx
  code-editor/src/components/ui/alert.tsx
  code-editor/src/components/ui/aspect-ratio.tsx
  code-editor/src/components/ui/avatar.tsx
  code-editor/src/components/ui/badge.tsx
  code-editor/src/components/ui/breadcrumb.tsx
  code-editor/src/components/ui/button-group.tsx
  code-editor/src/components/ui/button.tsx
  code-editor/src/components/ui/calendar.tsx
  code-editor/src/components/ui/card.tsx
  code-editor/src/components/ui/carousel.tsx
  code-editor/src/components/ui/chart.tsx
  code-editor/src/components/ui/checkbox.tsx
  code-editor/src/components/ui/collapsible.tsx
  code-editor/src/components/ui/command.tsx
  code-editor/src/components/ui/context-menu.tsx
  code-editor/src/components/ui/dialog.tsx
  code-editor/src/components/ui/drawer.tsx
  code-editor/src/components/ui/dropdown-menu.tsx
  code-editor/src/components/ui/empty.tsx
  code-editor/src/components/ui/field.tsx
  code-editor/src/components/ui/form.tsx
  code-editor/src/components/ui/hover-card.tsx
  code-editor/src/components/ui/input-group.tsx
  code-editor/src/components/ui/input-otp.tsx
  code-editor/src/components/ui/input.tsx
  code-editor/src/components/ui/item.tsx
  code-editor/src/components/ui/kbd.tsx
  code-editor/src/components/ui/label.tsx
  code-editor/src/components/ui/menubar.tsx
  code-editor/src/components/ui/navigation-menu.tsx
  code-editor/src/components/ui/pagination.tsx
  code-editor/src/components/ui/popover.tsx
  code-editor/src/components/ui/progress.tsx
  code-editor/src/components/ui/radio-group.tsx
  code-editor/src/components/ui/resizable.tsx
  code-editor/src/components/ui/scroll-area.tsx
  code-editor/src/components/ui/select.tsx
  code-editor/src/components/ui/separator.tsx
  code-editor/src/components/ui/sheet.tsx
  code-editor/src/components/ui/sidebar.tsx
  code-editor/src/components/ui/skeleton.tsx
  code-editor/src/components/ui/slider.tsx
  code-editor/src/components/ui/sonner.tsx
  code-editor/src/components/ui/spinner.tsx
  code-editor/src/components/ui/switch.tsx
  code-editor/src/components/ui/table.tsx
  code-editor/src/components/ui/tabs.tsx
  code-editor/src/components/ui/textarea.tsx
  code-editor/src/components/ui/toast.tsx
  code-editor/src/components/ui/toaster.tsx
  code-editor/src/components/ui/toggle-group.tsx
  code-editor/src/components/ui/toggle.tsx
  code-editor/src/components/ui/tooltip.tsx
  code-editor/src/hooks/use-mobile.tsx
  code-editor/src/hooks/use-toast.ts
  code-editor/src/index.css
  code-editor/src/lib/ai-service.ts
  code-editor/src/lib/github-service.ts
  code-editor/src/lib/projects.ts
  code-editor/src/lib/store.ts
  code-editor/src/lib/templates.ts
  code-editor/src/lib/tts-service.ts
  code-editor/src/lib/utils.ts
  code-editor/src/lib/virtual-fs.ts
  code-editor/src/lib/zip-service.ts
  code-editor/src/main.tsx
  code-editor/src/pages/not-found.tsx
  code-editor/tsconfig.json
  code-editor/vite.config.apk.ts
  code-editor/vite.config.standalone.ts
  code-editor/vite.config.ts
  mockup-sandbox/.replit-artifact/artifact.toml
  mockup-sandbox/components.json
  mockup-sandbox/index.html
  mockup-sandbox/mockupPreviewPlugin.ts
  mockup-sandbox/package.json
  mockup-sandbox/src/.generated/mockup-components.ts
  mockup-sandbox/src/App.tsx
  mockup-sandbox/src/components/ui/accordion.tsx
  mockup-sandbox/src/components/ui/alert-dialog.tsx
  mockup-sandbox/src/components/ui/alert.tsx
  mockup-sandbox/src/components/ui/aspect-ratio.tsx
  mockup-sandbox/src/components/ui/avatar.tsx
  mockup-sandbox/src/components/ui/badge.tsx
  mockup-sandbox/src/components/ui/breadcrumb.tsx
  mockup-sandbox/src/components/ui/button-group.tsx
  mockup-sandbox/src/components/ui/button.tsx
  mockup-sandbox/src/components/ui/calendar.tsx
  mockup-sandbox/src/components/ui/card.tsx
  mockup-sandbox/src/components/ui/carousel.tsx
  mockup-sandbox/src/components/ui/chart.tsx
  mockup-sandbox/src/components/ui/checkbox.tsx
  mockup-sandbox/src/components/ui/collapsible.tsx
  mockup-sandbox/src/components/ui/command.tsx
  mockup-sandbox/src/components/ui/context-menu.tsx
  mockup-sandbox/src/components/ui/dialog.tsx
  mockup-sandbox/src/components/ui/drawer.tsx
  mockup-sandbox/src/components/ui/dropdown-menu.tsx
  mockup-sandbox/src/components/ui/empty.tsx
  mockup-sandbox/src/components/ui/field.tsx
  mockup-sandbox/src/components/ui/form.tsx
  mockup-sandbox/src/components/ui/hover-card.tsx
  mockup-sandbox/src/components/ui/input-group.tsx
  mockup-sandbox/src/components/ui/input-otp.tsx
  mockup-sandbox/src/components/ui/input.tsx
  mockup-sandbox/src/components/ui/item.tsx
  mockup-sandbox/src/components/ui/kbd.tsx
  mockup-sandbox/src/components/ui/label.tsx
  mockup-sandbox/src/components/ui/menubar.tsx
  mockup-sandbox/src/components/ui/navigation-menu.tsx
  mockup-sandbox/src/components/ui/pagination.tsx
  mockup-sandbox/src/components/ui/popover.tsx
  mockup-sandbox/src/components/ui/progress.tsx
  mockup-sandbox/src/components/ui/radio-group.tsx
  mockup-sandbox/src/components/ui/resizable.tsx
  mockup-sandbox/src/components/ui/scroll-area.tsx
  mockup-sandbox/src/components/ui/select.tsx
  mockup-sandbox/src/components/ui/separator.tsx
  mockup-sandbox/src/components/ui/sheet.tsx
  mockup-sandbox/src/components/ui/sidebar.tsx
  mockup-sandbox/src/components/ui/skeleton.tsx
  mockup-sandbox/src/components/ui/slider.tsx
  mockup-sandbox/src/components/ui/sonner.tsx
  mockup-sandbox/src/components/ui/spinner.tsx
  mockup-sandbox/src/components/ui/switch.tsx
  mockup-sandbox/src/components/ui/table.tsx
  mockup-sandbox/src/components/ui/tabs.tsx
  mockup-sandbox/src/components/ui/textarea.tsx
  mockup-sandbox/src/components/ui/toast.tsx
  mockup-sandbox/src/components/ui/toaster.tsx
  mockup-sandbox/src/components/ui/toggle-group.tsx
  mockup-sandbox/src/components/ui/toggle.tsx
  mockup-sandbox/src/components/ui/tooltip.tsx
  mockup-sandbox/src/hooks/use-mobile.tsx
  mockup-sandbox/src/hooks/use-toast.ts
  mockup-sandbox/src/index.css
  mockup-sandbox/src/lib/utils.ts
  mockup-sandbox/src/main.tsx
  mockup-sandbox/tsconfig.json
  mockup-sandbox/vite.config.ts
```

---

*Plano gerado pelo SK Code Editor — 19/09/2026, 08:54:19*