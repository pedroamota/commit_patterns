# 📋 Guia de Labels para Commits

Padronização de labels para commits em projetos **Backend**, **Frontend** e **Mobile**.  
*Inspirado no Conventional Commits, com emojis para melhor visualização.*

---

## 🎯 Labels Universais

| Emoji + Nome       | Aplicação               | Exemplo de Uso                          |
|--------------------|-------------------------|------------------------------------------|
| `✨ feat`          | Nova funcionalidade     | `✨ feat: Login com Biometria`           |
| `🐛 fix`           | Correção de bugs        | `🐛 fix: Validação de data inválida`     |
| `📚 docs`          | Documentação            | `📚 docs: Atualiza diagrama de arquitetura` |
| `♻️ refactor`      | Refatoração             | `♻️ refactor: Remove código duplicado`   |
| `🚧 wip`           | Trabalho em progresso   | `🚧 wip: Tela de pagamento (50%)`        |
| `🔧 config`        | Configurações           | `🔧 config: Atualiza webpack para v5`    |
| `⚡ perf`          | Performance             | `⚡ perf: Reduz tempo de carga em 40%`    |
| `🧪 test`          | Testes                  | `🧪 test: Cobertura de testes para API`  |

---

## 🔧 Backend

| Emoji + Nome         | Aplicação               | Exemplo de Uso                          |
|----------------------|-------------------------|------------------------------------------|
| `🔒 security`        | Segurança               | `🔒 security: Adiciona sanitização de SQL` |
| `📡 endpoint`        | Endpoints API           | `📡 endpoint: DELETE /api/users/{id}`    |
| `💾 db`              | Banco de Dados          | `💾 db: Migração para UUID`              |
| `📦 package`         | Pacotes/Integrações     | `📦 package: Atualiza SDK do Twilio`     |
| `📈 metrics`         | Monitoramento           | `📈 metrics: Configura New Relic`        |
| `🧩 middleware`      | Middlewares             | `🧩 middleware: Rate limiter global`     |

---

## 🎨 Frontend

| Emoji + Nome         | Aplicação               | Exemplo de Uso                          |
|----------------------|-------------------------|------------------------------------------|
| `🎨 ui`              | Interface               | `🎨 ui: Novo design da homepage`         |
| `📱 responsive`      | Responsividade          | `📱 responsive: Grid ajustável para mobile` |
| `🖼️ assets`         | Imagens/Ícones          | `🖼️ assets: Otimiza imagens em WebP`     |
| `🌐 i18n`            | Internacionalização     | `🌐 i18n: Traduções para japonês`         |
| `📡 api-call`        | Chamadas API            | `📡 api-call: Paginação na busca`        |
| `📊 analytics`       | Rastreamento            | `📊 analytics: Evento de scroll depth`   |

---

## 📱 Mobile

| Emoji + Nome         | Aplicação               | Exemplo de Uso                          |
|----------------------|-------------------------|------------------------------------------|
| `📱 android`         | Android-specific        | `📱 android: Suporte a foldables`        |
| `🍎 ios`             | iOS-specific            | `🍎 ios: Dark mode dinâmico`             |
| `📲 gesture`         | Gestos                  | `📲 gesture: Double tap para like`       |
| `📡 native-module`   | Módulos Nativos         | `📡 native-module: Integração com ARKit` |
| `🔔 push`            | Notificações            | `🔔 push: Notificação local agendada`    |
| `📱 offline`         | Funcionalidade Offline  | `📱 offline: Sync automático`            |

---

## 🛠️ Exemplo de Commit

```bash
git commit -m "✨ feat(search): Adiciona filtro por geolocalização
- Implementa busca por raio de 10km
- Integra com Google Maps API
- Adiciona testes E2E

Refs: #45, #78"
```

---

## 💡 Dicas de Uso

1. **Combine Labels com Escopo**:  
   `🐛 fix(auth): Corrige timeout no login social`

2. **Use Emojis Direto do Guia**:  
   Copie os emojis desta tabela para manter a padronização.

3. **Automatize com Hooks**:  
   Adicione um `commit-msg` hook para validar o formato:
   ```sh
   # .git/hooks/commit-msg
   if ! grep -qE "(✨|🐛|📚|♻️)" "$1"; then
     echo "⚠️ Use labels do padrão especificado no README!"
     exit 1
   fi
   ```

4. **Gere Changelogs Automaticamente**:  
   Use [standard-version](https://github.com/conventional-changelog/standard-version) para gerar logs baseados nos commits.

---

*📄 Licença: [MIT](https://choosealicense.com/licenses/mit/)*  
*🔗 Adapte conforme as necessidades do seu projeto!*
