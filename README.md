# 📋 Guia de Labels para Commits

Padronização de labels para commits em projetos **Backend**, **Frontend**, **Mobile** e **CI/CD**.

Inspirado no **Conventional Commits**, usando emojis para melhorar a leitura do histórico do Git.

---

## ✅ Padrão do Commit

```bash
<emoji> <tipo>(escopo): mensagem curta
```

Exemplo:

```bash
✨ feat(auth): Adiciona login com biometria
```

---

## 🎯 Labels Universais

| Emoji + Tipo | Código do Emoji | Aplicação | Exemplo de Uso |
|---|---|---|---|
| `✨ feat` | `:sparkles:` | Nova funcionalidade | `✨ feat: Login com biometria` |
| `🐛 fix` | `:bug:` | Correção de bugs | `🐛 fix: Corrige validação de data inválida` |
| `📚 docs` | `:books:` | Documentação | `📚 docs: Atualiza diagrama de arquitetura` |
| `♻️ refactor` | `:recycle:` | Refatoração sem alterar comportamento | `♻️ refactor: Remove código duplicado` |
| `🚧 wip` | `:construction:` | Trabalho em progresso | `🚧 wip: Tela de pagamento parcialmente implementada` |
| `🔧 config` | `:wrench:` | Configurações gerais | `🔧 config: Atualiza webpack para v5` |
| `⚡ perf` | `:zap:` | Performance | `⚡ perf: Reduz tempo de carga da tela inicial` |
| `🧪 test` | `:test_tube:` | Testes | `🧪 test: Adiciona cobertura para API de pedidos` |
| `🔥 remove` | `:fire:` | Remove código, arquivos ou dependências | `🔥 remove: Remove componente legado de login` |
| `🚑 hotfix` | `:ambulance:` | Correção urgente em produção | `🚑 hotfix: Corrige erro crítico no checkout` |
| `📝 chore` | `:memo:` | Tarefa simples de manutenção | `📝 chore: Ajusta scripts do package.json` |

---

## 🔧 Backend

| Emoji + Tipo | Código do Emoji | Aplicação | Exemplo de Uso |
|---|---|---|---|
| `🔒 security` | `:lock:` | Segurança | `🔒 security: Adiciona sanitização contra SQL Injection` |
| `📡 endpoint` | `:satellite:` | Endpoints de API | `📡 endpoint: Cria DELETE /api/users/{id}` |
| `💾 db` | `:floppy_disk:` | Banco de dados, migrations e schemas | `💾 db: Cria migration para UUID` |
| `📦 package` | `:package:` | Pacotes, libs e integrações | `📦 package: Atualiza SDK do Twilio` |
| `📈 metrics` | `:chart_with_upwards_trend:` | Métricas e monitoramento | `📈 metrics: Configura métricas no Prometheus` |
| `🧩 middleware` | `:jigsaw:` | Middlewares | `🧩 middleware: Adiciona rate limiter global` |
| `🧱 model` | `:bricks:` | Models, entidades e schemas | `🧱 model: Adiciona entidade Pedido` |
| `🗃️ repository` | `:card_file_box:` | Repositórios, queries e camada de dados | `🗃️ repository: Otimiza consulta de estoque` |

---

## 🎨 Frontend

| Emoji + Tipo | Código do Emoji | Aplicação | Exemplo de Uso |
|---|---|---|---|
| `🎨 ui` | `:art:` | Interface visual | `🎨 ui: Novo design da homepage` |
| `📱 responsive` | `:iphone:` | Responsividade | `📱 responsive: Ajusta grid para mobile` |
| `🖼️ assets` | `:framed_picture:` | Imagens, ícones e arquivos visuais | `🖼️ assets: Otimiza imagens para WebP` |
| `🌐 i18n` | `:globe_with_meridians:` | Internacionalização | `🌐 i18n: Adiciona traduções para japonês` |
| `📡 api-call` | `:satellite:` | Chamadas para API | `📡 api-call: Adiciona paginação na busca` |
| `📊 analytics` | `:bar_chart:` | Eventos e rastreamento | `📊 analytics: Adiciona evento de scroll depth` |
| `🧭 route` | `:compass:` | Rotas e navegação | `🧭 route: Cria rota de detalhes do pedido` |
| `🧠 state` | `:brain:` | Estado global/local | `🧠 state: Centraliza estado do carrinho` |

---

## 📱 Mobile

| Emoji + Tipo | Código do Emoji | Aplicação | Exemplo de Uso |
|---|---|---|---|
| `🤖 android` | `:robot:` | Android-specific | `🤖 android: Suporte a foldables` |
| `🍎 ios` | `:apple:` | iOS-specific | `🍎 ios: Ajusta dark mode dinâmico` |
| `📲 gesture` | `:calling:` | Gestos | `📲 gesture: Double tap para like` |
| `📡 native-module` | `:satellite:` | Módulos nativos | `📡 native-module: Integração com ARKit` |
| `🔔 push` | `:bell:` | Notificações | `🔔 push: Notificação local agendada` |
| `📴 offline` | `:mobile_phone_off:` | Funcionalidade offline | `📴 offline: Sync automático em segundo plano` |
| `📍 location` | `:round_pushpin:` | GPS e localização | `📍 location: Adiciona tracking em tempo real` |

---

## 🚀 CI/CD, DevOps e Infraestrutura

| Emoji + Tipo | Código do Emoji | Aplicação | Exemplo de Uso |
|---|---|---|---|
| `🚀 ci` | `:rocket:` | Pipeline de CI/CD | `🚀 ci: Adiciona workflow de deploy automático` |
| `🐳 docker` | `:whale:` | Docker, Dockerfile e containers | `🐳 docker: Cria Dockerfile para API FastAPI` |
| `⚙️ pipeline` | `:gear:` | Configuração de pipeline | `⚙️ pipeline: Ajusta stages de build e deploy` |
| `🏗️ build` | `:building_construction:` | Build da aplicação | `🏗️ build: Corrige geração de bundle em produção` |
| `☁️ deploy` | `:cloud:` | Deploy e ambiente remoto | `☁️ deploy: Publica backend no servidor de produção` |
| `🧬 env` | `:dna:` | Variáveis de ambiente | `🧬 env: Adiciona variável DATABASE_URL` |
| `📜 script` | `:scroll:` | Scripts de automação | `📜 script: Cria script de backup do banco` |
| `🛠️ infra` | `:hammer_and_wrench:` | Infraestrutura geral | `🛠️ infra: Configura Nginx como reverse proxy` |
| `🔐 secrets` | `:closed_lock_with_key:` | Secrets, tokens e credenciais | `🔐 secrets: Configura secrets no GitHub Actions` |
| `📦 release` | `:package:` | Releases e versionamento | `📦 release: Gera versão 1.4.0` |

---

## 🧪 Hook simples para validar commits

Crie o arquivo:

```bash
.git/hooks/commit-msg
```

Conteúdo:

```sh
#!/bin/sh

commit_msg_file="$1"

pattern="^(✨|🐛|📚|♻️|🚧|🔧|⚡|🧪|🔥|🚑|📝|🔒|📡|💾|📦|📈|🧩|🧱|🗃️|🎨|📱|🖼️|🌐|📊|🧭|🧠|🤖|🍎|📲|🔔|📴|📍|🚀|🐳|⚙️|🏗️|☁️|🧬|📜|🛠️|🔐) [a-z0-9-]+(\([a-z0-9-]+\))?: .+"

if ! grep -qE "$pattern" "$commit_msg_file"; then
  echo "⚠️ Commit fora do padrão."
  echo ""
  echo "Formato esperado:"
  echo "  <emoji> <tipo>(escopo): mensagem"
  echo ""
  echo "Exemplo:"
  echo "  ✨ feat(auth): Adiciona login com biometria"
  echo ""
  exit 1
fi
```

Dê permissão de execução:

```bash
chmod +x .git/hooks/commit-msg
```
