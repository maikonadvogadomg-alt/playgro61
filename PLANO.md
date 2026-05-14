# PLANO DO PROJETO: HTML/CSS/JS

> Gerado automaticamente pelo SK Code Editor em 14/05/2026, 15:28:00
> **79 arquivo(s)** | **~33.723 linhas de codigo**

---

## RESUMO EXECUTIVO

- **Tipo de aplicacao:** Aplicacao Web Frontend (React)
- **Frontend / Stack principal:** React, TypeScript
- **Versao:** 0.0.0

**Para rodar o projeto:**
```bash
npm install && npm run dev
```

---

## ESTRUTURA DE ARQUIVOS

```
HTML/CSS/JS/
├── .github/
│   └── workflows/
│       ├── build-apk-eas.yml
│       └── build-apk-local.yml
├── .replit-artifact/
│   └── artifact.toml
├── app/
│   ├── (tabs)/
│   │   ├── _layout.tsx
│   │   ├── ai.tsx
│   │   ├── browser.tsx
│   │   ├── editor.tsx
│   │   ├── index.tsx
│   │   ├── plugins.tsx
│   │   ├── pwa.tsx
│   │   ├── settings.tsx
│   │   ├── tasks.tsx
│   │   └── terminal.tsx
│   ├── _layout.tsx
│   └── +not-found.tsx
├── components/
│   ├── AIChat.tsx
│   ├── AIMemoryModal.tsx
│   ├── APKBuilderModal.tsx
│   ├── AppStatusChecker.tsx
│   ├── CampoLivreModal.tsx
│   ├── CheckpointsModal.tsx
│   ├── CodeEditor.tsx
│   ├── CombinarAppsModal.tsx
│   ├── DatabasePanel.tsx
│   ├── ErrorBoundary.tsx
│   ├── ErrorFallback.tsx
│   ├── FileSidebar.tsx
│   ├── FloatingAI.tsx
│   ├── GitHubModal.tsx
│   ├── HtmlPlayground.tsx
│   ├── KeyboardAwareScrollViewCompat.tsx
│   ├── LibrarySearch.tsx
│   ├── ManualModal.tsx
│   ├── MessageRenderer.tsx
│   ├── MonacoEditor.tsx
│   ├── PreviewPanel.tsx
│   ├── ProjectOverviewModal.tsx
│   ├── ProjectPlanModal.tsx
│   ├── SystemStatus.tsx
│   ├── Terminal.tsx
│   ├── VoiceAssistant.tsx
│   ├── VSCodeView.tsx
│   ├── VSCodeWebModal.tsx
│   └── XTermWebView.tsx
├── constants/
│   └── colors.ts
├── context/
│   └── AppContext.tsx
├── data/
│   ├── featuredProjects.ts
│   └── legalModes.ts
├── hooks/
│   ├── useApiBase.ts
│   └── useColors.ts
├── plugins/
│   └── withTermuxIntent.js
├── server/
│   ├── templates/
│   │   └── landing-page.html
│   └── serve.js
├── services/
│   ├── apiBase.ts
│   ├── githubService.ts
│   ├── localSQLite.ts
│   ├── previewService.ts
│   ├── runtimeMode.ts
│   ├── storageService.ts
│   └── terminalService.ts
├── utils/
│   ├── projectPlan.ts
│   └── zipUtils.ts
├── .easignore
├── .env
├── .env.example
├── .gitignore
├── .npmrc
├── app.json
├── babel.config.js
├── capacitor.config.ts
├── COMO_BUILDAR.md
├── COMO-BUILDAR-APK.md
├── eas.json
├── expo-env.d.ts
├── GERAR-APK.md
├── metro.config.js
├── package.json
├── PLANO.md
└── tsconfig.json
```

---

## STACK TECNOLOGICO DETECTADO

- **Frontend:** React, TypeScript
- **Todos os pacotes (60):** @babel/core, @babel/runtime, @expo-google-fonts/inter, @expo/cli, @expo/config, @expo/config-plugins, @expo/ngrok, @expo/vector-icons, @react-native-async-storage/async-storage, @stardazed/streams-text-encoding, @tanstack/react-query, @ungap/structured-clone, babel-plugin-react-compiler, babel-preset-expo, eas-cli, expo, expo-blur, expo-clipboard, expo-constants, expo-document-picker, expo-file-system, expo-font, expo-haptics, expo-image, expo-image-picker, expo-intent-launcher, expo-linear-gradient, expo-linking, expo-location, expo-router, expo-sharing, expo-speech, expo-splash-screen, expo-sqlite, expo-status-bar, expo-symbols, expo-system-ui, expo-web-browser, jszip, metro, metro-runtime, pako, react, react-dom, react-native, react-native-gesture-handler, react-native-keyboard-controller, react-native-reanimated, react-native-safe-area-context, react-native-screens, react-native-svg, react-native-web, react-native-webview, react-native-worklets, zod, zod-validation-error, @types/pako, @types/react, @types/react-dom, typescript

---

## ROTAS DA API (endpoints detectados automaticamente)

```
POST   /api/chat  (em data/featuredProjects.ts)
GET    /api/saude  (em data/featuredProjects.ts)
POST   /api/chat  (em data/featuredProjects.ts)
GET    /api/saude  (em data/featuredProjects.ts)
POST   /api/chat  (em data/featuredProjects.ts)
GET    /api/saude  (em data/featuredProjects.ts)
POST   /api/chat  (em data/featuredProjects.ts)
GET    /api/provedores  (em data/featuredProjects.ts)
GET    /api/saude  (em data/featuredProjects.ts)
```

---

## SCRIPTS DISPONIVEIS (package.json)

```bash
npm run dev           # EXPO_TOKEN= pnpm exec expo start --localhost --port $PORT
npm run start         # pnpm exec expo start
npm run android       # pnpm exec expo run:android
npm run ios           # pnpm exec expo run:ios
npm run web           # pnpm exec expo start --web
```

---

## VARIAVEIS DE AMBIENTE NECESSARIAS

Crie um arquivo `.env` na raiz com estas variaveis:

```env
PORT=seu_valor_aqui
GROQ_API_KEY=seu_valor_aqui
GROQ_MODEL=seu_valor_aqui
ANTHROPIC_API_KEY=seu_valor_aqui
CLAUDE_MODEL=seu_valor_aqui
GEMINI_API_KEY=seu_valor_aqui
GEMINI_MODEL=seu_valor_aqui
OPENAI_API_KEY=seu_valor_aqui
EXPO_PUBLIC_DOMAIN=seu_valor_aqui
BASE_PATH=seu_valor_aqui
EXPO_PUBLIC_API_BASE_URL=seu_valor_aqui
EXPO_PUBLIC_REMOTE_API_URL=seu_valor_aqui
EXPO_PUBLIC_APP_MODE=seu_valor_aqui
EXPO_PUBLIC_API_STRATEGY=seu_valor_aqui
EXPO_PUBLIC_LOCAL_API_PORT=seu_valor_aqui
EXPO_PUBLIC_LOCAL_PREVIEW_PORT=seu_valor_aqui
EXPO_PUBLIC_ENABLE_TERMUX=seu_valor_aqui
EXPO_PUBLIC_ENABLE_REMOTE_AI=seu_valor_aqui
EXPO_PUBLIC_ENABLE_GITHUB=seu_valor_aqui
EXPO_PUBLIC_ENABLE_REMOTE_DB=seu_valor_aqui
EXPO_PUBLIC_ENABLE_REMOTE_TERMINAL=seu_valor_aqui
EXPO_PUBLIC_GEMINI_KEY=seu_valor_aqui
EXPO_PUBLIC_GROQ_KEY=seu_valor_aqui
EXPO_PUBLIC_OPENAI_KEY=seu_valor_aqui
EXPO_PUBLIC_ANTHROPIC_KEY=seu_valor_aqui
EXPO_PUBLIC_OPENROUTER_KEY=seu_valor_aqui
EXPO_PUBLIC_XAI_KEY=seu_valor_aqui
EXPO_PUBLIC_PERPLEXITY_KEY=seu_valor_aqui
DATABASE_URL=seu_valor_aqui
NEON_HOST=seu_valor_aqui
NEON_DATABASE=seu_valor_aqui
NEON_USER=seu_valor_aqui
NEON_PASSWORD=seu_valor_aqui
NEON_PORT=seu_valor_aqui
NEON_SSL=seu_valor_aqui
BCRYPT_SALT_ROUNDS=seu_valor_aqui
JWT_SECRET=seu_valor_aqui
SESSION_SECRET=seu_valor_aqui
EXPO_PUBLIC_GITHUB_TOKEN=seu_valor_aqui
EXPO_PUBLIC_GITHUB_USER=seu_valor_aqui
EXPO_TOKEN=seu_valor_aqui
```

---

## ARQUIVOS PRINCIPAIS

- `app/(tabs)/index.tsx` — Arquivo principal

---

## GUIA COMPLETO — O QUE CADA PARTE DO PROJETO FAZ

> Esta secao explica, em linguagem simples, o que e para que serve cada pasta e cada arquivo.

### 📁 Raiz do Projeto (pasta principal)
> Arquivos de configuracao e pontos de entrada ficam aqui.

**`.easignore`** _(25 linhas)_
Arquivo EASIGNORE — parte do projeto.

**`.env`** _(2 linhas)_
Arquivo de variaveis secretas (senhas, chaves de API). NUNCA suba este arquivo para o GitHub.

**`.env.example`** _(91 linhas)_
Arquivo de variaveis secretas (senhas, chaves de API). NUNCA suba este arquivo para o GitHub.

**`.gitignore`** _(42 linhas)_
Lista de arquivos/pastas que o Git deve IGNORAR (nao versionar). Ex: node_modules, .env

**`.npmrc`** _(3 linhas)_
Arquivo NPMRC — parte do projeto.

**`COMO-BUILDAR-APK.md`** _(78 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`COMO_BUILDAR.md`** _(113 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`GERAR-APK.md`** _(62 linhas)_
Arquivo de documentacao em Markdown (texto formatado com #titulos, **negrito**, listas).

**`PLANO.md`** _(187 linhas)_
Este documento! Gerado automaticamente pelo SK Code Editor com toda a estrutura do projeto.

**`app.json`** _(63 linhas)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

**`babel.config.js`** _(7 linhas)_
Arquivo de CONSTANTES/CONFIGURACAO — valores fixos usados em varios lugares do projeto.

**`capacitor.config.ts`** _(43 linhas)_
Arquivo de CONSTANTES/CONFIGURACAO — valores fixos usados em varios lugares do projeto.

**`eas.json`** _(58 linhas)_
Arquivo de dados ou configuracao no formato JSON (chave: valor).

**`expo-env.d.ts`** _(3 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`metro.config.js`** _(28 linhas)_
Arquivo de CONSTANTES/CONFIGURACAO — valores fixos usados em varios lugares do projeto.

**`package.json`** _(78 linhas)_
Registro de dependencias e scripts do projeto. Aqui ficam os comandos (npm run dev, npm start) e os pacotes instalados.

**`tsconfig.json`** _(24 linhas)_
Configuracao do TypeScript. Diz para o computador como interpretar o codigo .ts e .tsx.

---

### 📁 `.replit-artifact/`
> Pasta '.replit-artifact' — agrupamento de arquivos relacionados.

**`artifact.toml`** _(23 linhas)_
Arquivo TOML — parte do projeto.

---

### 📁 `app/`
> Pasta 'app' — agrupamento de arquivos relacionados.

**`+not-found.tsx`** _(46 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`_layout.tsx`** _(69 linhas)_
Componente de LAYOUT — define a estrutura visual da pagina (cabecalho, sidebar, rodape). Envolve outros componentes.

---

### 📁 `components/`
> Pecas visuais reutilizaveis da interface (botoes, cards, formularios...).

**`AIChat.tsx`** _(1577 linhas)_
Componente de CHAT/MENSAGENS — interface de conversa em tempo real.

**`AIMemoryModal.tsx`** _(203 linhas)_
Componente MODAL — janela/popup que aparece sobre a tela pedindo uma acao ou mostrando uma informacao importante.

**`APKBuilderModal.tsx`** _(1058 linhas)_
Componente MODAL — janela/popup que aparece sobre a tela pedindo uma acao ou mostrando uma informacao importante.

**`AppStatusChecker.tsx`** _(368 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`CampoLivreModal.tsx`** _(1071 linhas)_
Componente MODAL — janela/popup que aparece sobre a tela pedindo uma acao ou mostrando uma informacao importante.

**`CheckpointsModal.tsx`** _(173 linhas)_
Componente MODAL — janela/popup que aparece sobre a tela pedindo uma acao ou mostrando uma informacao importante.

**`CodeEditor.tsx`** _(383 linhas)_
Componente EDITOR — area de edicao de texto, codigo ou conteudo rico.

**`CombinarAppsModal.tsx`** _(352 linhas)_
Componente MODAL — janela/popup que aparece sobre a tela pedindo uma acao ou mostrando uma informacao importante.

**`DatabasePanel.tsx`** _(1122 linhas)_
Componente de ABAS — permite alternar entre diferentes secoes de conteudo com clique.

**`ErrorBoundary.tsx`** _(55 linhas)_
Componente de ERRO — exibido quando algo da errado, com mensagem explicativa.

**`ErrorFallback.tsx`** _(279 linhas)_
Componente de ERRO — exibido quando algo da errado, com mensagem explicativa.

**`FileSidebar.tsx`** _(742 linhas)_
Componente de BARRA LATERAL — menu ou painel que aparece na lateral da tela.

**`FloatingAI.tsx`** _(897 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`GitHubModal.tsx`** _(1257 linhas)_
Componente MODAL — janela/popup que aparece sobre a tela pedindo uma acao ou mostrando uma informacao importante.

**`HtmlPlayground.tsx`** _(706 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`KeyboardAwareScrollViewCompat.tsx`** _(30 linhas)_
Componente de PAGINA/TELA — representa uma tela completa navegavel no app.

**`LibrarySearch.tsx`** _(327 linhas)_
Componente de BUSCA — campo e logica para filtrar/encontrar conteudo.

**`ManualModal.tsx`** _(776 linhas)_
Componente MODAL — janela/popup que aparece sobre a tela pedindo uma acao ou mostrando uma informacao importante.

**`MessageRenderer.tsx`** _(504 linhas)_
Componente de CHAT/MENSAGENS — interface de conversa em tempo real.

**`MonacoEditor.tsx`** _(163 linhas)_
Componente EDITOR — area de edicao de texto, codigo ou conteudo rico.

**`PreviewPanel.tsx`** _(500 linhas)_
Componente de PAGINA/TELA — representa uma tela completa navegavel no app.

**`ProjectOverviewModal.tsx`** _(504 linhas)_
Componente MODAL — janela/popup que aparece sobre a tela pedindo uma acao ou mostrando uma informacao importante.

**`ProjectPlanModal.tsx`** _(369 linhas)_
Componente MODAL — janela/popup que aparece sobre a tela pedindo uma acao ou mostrando uma informacao importante.

**`SystemStatus.tsx`** _(480 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`Terminal.tsx`** _(1297 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`VSCodeView.tsx`** _(685 linhas)_
Componente de PAGINA/TELA — representa uma tela completa navegavel no app.

**`VSCodeWebModal.tsx`** _(363 linhas)_
Componente MODAL — janela/popup que aparece sobre a tela pedindo uma acao ou mostrando uma informacao importante.

**`VoiceAssistant.tsx`** _(1020 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`XTermWebView.tsx`** _(311 linhas)_
Componente de PAGINA/TELA — representa uma tela completa navegavel no app.

---

### 📁 `constants/`
> Pasta 'constants' — agrupamento de arquivos relacionados.

**`colors.ts`** _(98 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `context/`
> Gerenciamento de estado global — dados compartilhados entre telas.

**`AppContext.tsx`** _(1385 linhas)_
CONTEXT do React — mecanismo para compartilhar dados entre componentes sem passar por props.

---

### 📁 `data/`
> Pasta 'data' — agrupamento de arquivos relacionados.

**`featuredProjects.ts`** _(802 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`legalModes.ts`** _(106 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `hooks/`
> Hooks React customizados — logica reutilizavel de estado e efeitos.

**`useApiBase.ts`** _(100 linhas)_
HOOK de dados — busca informacoes da API e gerencia estado de carregamento e erro.

**`useColors.ts`** _(25 linhas)_
HOOK React personalizado para gerenciar estado/comportamento de 'colors'.

---

### 📁 `plugins/`
> Pasta 'plugins' — agrupamento de arquivos relacionados.

**`withTermuxIntent.js`** _(26 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `server/`
> Pasta 'server' — agrupamento de arquivos relacionados.

**`serve.js`** _(136 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

---

### 📁 `services/`
> Comunicacao com servidor, banco de dados ou APIs externas.

**`apiBase.ts`** _(28 linhas)_
Arquivo de SERVICO/API — funcoes para comunicar com o servidor ou API externa.

**`githubService.ts`** _(530 linhas)_
Arquivo de SERVICO/API — funcoes para comunicar com o servidor ou API externa.

**`localSQLite.ts`** _(81 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`previewService.ts`** _(17 linhas)_
Arquivo de SERVICO/API — funcoes para comunicar com o servidor ou API externa.

**`runtimeMode.ts`** _(56 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`storageService.ts`** _(16 linhas)_
Arquivo de SERVICO/API — funcoes para comunicar com o servidor ou API externa.

**`terminalService.ts`** _(29 linhas)_
Arquivo de SERVICO/API — funcoes para comunicar com o servidor ou API externa.

---

### 📁 `utils/`
> Funcoes auxiliares reutilizaveis em varios lugares do projeto.

**`projectPlan.ts`** _(208 linhas)_
Arquivo TypeScript/JavaScript — logica, funcoes ou modulo do projeto.

**`zipUtils.ts`** _(473 linhas)_
Funcoes UTILITARIAS — ferramentas reutilizaveis de uso geral no projeto.

---

### 📁 `.github/workflows/`
> Pasta 'workflows' — agrupamento de arquivos relacionados.

**`build-apk-eas.yml`** _(72 linhas)_
Arquivo YML — parte do projeto.

**`build-apk-local.yml`** _(126 linhas)_
Arquivo YML — parte do projeto.

---

### 📁 `app/(tabs)/`
> Pasta '(tabs)' — agrupamento de arquivos relacionados.

**`_layout.tsx`** _(170 linhas)_
Componente de LAYOUT — define a estrutura visual da pagina (cabecalho, sidebar, rodape). Envolve outros componentes.

**`ai.tsx`** _(48 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`browser.tsx`** _(203 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`editor.tsx`** _(1403 linhas)_
Componente EDITOR — area de edicao de texto, codigo ou conteudo rico.

**`index.tsx`** _(3958 linhas)_
Ponto de entrada do React — monta o componente App na pagina HTML.

**`plugins.tsx`** _(1234 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`pwa.tsx`** _(625 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`settings.tsx`** _(1955 linhas)_
Componente de CONFIGURACOES — tela onde o usuario ajusta preferencias do app.

**`tasks.tsx`** _(522 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

**`terminal.tsx`** _(213 linhas)_
Componente React — parte visual reutilizavel da interface do usuario.

---

### 📁 `server/templates/`
> Pasta 'templates' — agrupamento de arquivos relacionados.

**`landing-page.html`** _(461 linhas)_
Arquivo HTML — parte do projeto.

---

## CONTEXTO PARA IA (copie e cole para continuar o projeto)

> Use este bloco para explicar o projeto para qualquer IA ou desenvolvedor:

```
Projeto: HTML/CSS/JS
Tipo: Aplicacao Web Frontend (React)
Stack: React, TypeScript
Arquivos: 79 | Linhas: ~33.723
Rotas API: 9 endpoint(s) detectado(s)
Variaveis de ambiente necessarias: PORT, GROQ_API_KEY, GROQ_MODEL, ANTHROPIC_API_KEY, CLAUDE_MODEL, GEMINI_API_KEY, GEMINI_MODEL, OPENAI_API_KEY, EXPO_PUBLIC_DOMAIN, BASE_PATH, EXPO_PUBLIC_API_BASE_URL, EXPO_PUBLIC_REMOTE_API_URL, EXPO_PUBLIC_APP_MODE, EXPO_PUBLIC_API_STRATEGY, EXPO_PUBLIC_LOCAL_API_PORT, EXPO_PUBLIC_LOCAL_PREVIEW_PORT, EXPO_PUBLIC_ENABLE_TERMUX, EXPO_PUBLIC_ENABLE_REMOTE_AI, EXPO_PUBLIC_ENABLE_GITHUB, EXPO_PUBLIC_ENABLE_REMOTE_DB, EXPO_PUBLIC_ENABLE_REMOTE_TERMINAL, EXPO_PUBLIC_GEMINI_KEY, EXPO_PUBLIC_GROQ_KEY, EXPO_PUBLIC_OPENAI_KEY, EXPO_PUBLIC_ANTHROPIC_KEY, EXPO_PUBLIC_OPENROUTER_KEY, EXPO_PUBLIC_XAI_KEY, EXPO_PUBLIC_PERPLEXITY_KEY, DATABASE_URL, NEON_HOST, NEON_DATABASE, NEON_USER, NEON_PASSWORD, NEON_PORT, NEON_SSL, BCRYPT_SALT_ROUNDS, JWT_SECRET, SESSION_SECRET, EXPO_PUBLIC_GITHUB_TOKEN, EXPO_PUBLIC_GITHUB_USER, EXPO_TOKEN

Estrutura principal:
  .easignore
  .env
  .env.example
  .github/workflows/build-apk-eas.yml
  .github/workflows/build-apk-local.yml
  .gitignore
  .npmrc
  .replit-artifact/artifact.toml
  COMO-BUILDAR-APK.md
  COMO_BUILDAR.md
  GERAR-APK.md
  PLANO.md
  app.json
  app/(tabs)/_layout.tsx
  app/(tabs)/ai.tsx
  app/(tabs)/browser.tsx
  app/(tabs)/editor.tsx
  app/(tabs)/index.tsx
  app/(tabs)/plugins.tsx
  app/(tabs)/pwa.tsx
  app/(tabs)/settings.tsx
  app/(tabs)/tasks.tsx
  app/(tabs)/terminal.tsx
  app/+not-found.tsx
  app/_layout.tsx
  babel.config.js
  capacitor.config.ts
  components/AIChat.tsx
  components/AIMemoryModal.tsx
  components/APKBuilderModal.tsx
  components/AppStatusChecker.tsx
  components/CampoLivreModal.tsx
  components/CheckpointsModal.tsx
  components/CodeEditor.tsx
  components/CombinarAppsModal.tsx
  components/DatabasePanel.tsx
  components/ErrorBoundary.tsx
  components/ErrorFallback.tsx
  components/FileSidebar.tsx
  components/FloatingAI.tsx
  components/GitHubModal.tsx
  components/HtmlPlayground.tsx
  components/KeyboardAwareScrollViewCompat.tsx
  components/LibrarySearch.tsx
  components/ManualModal.tsx
  components/MessageRenderer.tsx
  components/MonacoEditor.tsx
  components/PreviewPanel.tsx
  components/ProjectOverviewModal.tsx
  components/ProjectPlanModal.tsx
  components/SystemStatus.tsx
  components/Terminal.tsx
  components/VSCodeView.tsx
  components/VSCodeWebModal.tsx
  components/VoiceAssistant.tsx
  components/XTermWebView.tsx
  constants/colors.ts
  context/AppContext.tsx
  data/featuredProjects.ts
  data/legalModes.ts
  eas.json
  expo-env.d.ts
  hooks/useApiBase.ts
  hooks/useColors.ts
  metro.config.js
  package.json
  plugins/withTermuxIntent.js
  server/serve.js
  server/templates/landing-page.html
  services/apiBase.ts
  services/githubService.ts
  services/localSQLite.ts
  services/previewService.ts
  services/runtimeMode.ts
  services/storageService.ts
  services/terminalService.ts
  tsconfig.json
  utils/projectPlan.ts
  utils/zipUtils.ts
```

---

*Plano gerado pelo SK Code Editor — 14/05/2026, 15:28:00*