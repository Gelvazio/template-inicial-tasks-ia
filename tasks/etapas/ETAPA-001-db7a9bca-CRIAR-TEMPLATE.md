## Etapa 001-db7a9bca — TEMPLATE: Criar o esqueleto de projeto com IA a partir do Dashboard AI

**Tarefa:** TEMPLATE · **Pedido em:** 2026-10-14 08:39 · **Criada por:** Claude Code (Opus 5.5) (local · main)
**Pedido:** "leia a pasta C:\fontes\dashboard-ai-claude-code-senai e entenda como é feito o controle de
tarefas e copie pra esta pasta aqui, como um esqueleto inicial de qualquer projeto com IA"
**Objetivo:** ter um repositório-modelo com as regras e o quadro de tarefas prontos para qualquer
projeto com várias IAs.

### Escopo

- **Entra:** `AGENTS.md`, `CLAUDE.md`, `GEMINI.md`; `.claude/rules/` (índice, início, git, tarefas,
  várias IAs, testes, código, visualizador); `tasks/` vazio pelos modelos; hooks do Claude Code
  (`.claude/hooks/` + `settings.json`) e do Git (`.githooks/`); `.gitattributes`;
  `scripts/sincronizar-agentes.mjs` + `package.json` mínimo; skills `proxima-task`,
  `classificar-tarefa` e `liderar-equipe`; agentes `classificador-tarefas` e `executor-*`.
- **Não entra:** nada específico do Dashboard AI (Supabase, Laya Server, MCP próprio, monitor,
  histórico de tarefas, `reporte-progresso.md`).

### Riscos

- Ficar referência ao projeto de origem → conferido com `grep` por "Dashboard", "Laya", "Supabase"
  e códigos `SUB-`.

### Decisões

- 2026-10-14 08:45 — Gelvazio escolheu incluir a equipe de agentes e o visualizador (marcou também
  "Só o núcleo", lido como engano por contradizer as outras duas opções).
- 2026-10-14 — Classificação de nível só por sinais (sem o Laya Server); matriz de modelos fica
  como ponto de partida ajustável.
- 2026-10-14 — `sincronizar-agentes.mjs` passa a gerar `.codex/agents/*.toml` a partir de
  `.agents/agents/` (no original eram cópias à mão, com caminho `.Codex/rules` errado).

### TEMPLATE.1 — Copiar e generalizar regras, quadro, skills, agentes, hooks e visualizador

**Próximo passo:** nenhum — concluída.

- **Nível:** PESADO — estrutura nova e mais de 3 arquivos ligados
- **Descrição:** copiar os arquivos do escopo e tirar deles tudo o que é do Dashboard AI.
- **Critérios de Aceitação:** nenhuma referência ao projeto de origem; `npm run check:agentes`
  sem cópias desatualizadas; sintaxe dos scripts conferida com `node --check`.
- **Entrega:** commit `feat(TEMPLATE.1)` · **Verificação:** `grep` sem referências ao Dashboard
  AI, `node --check` nos `.mjs`, `bash -n` nos hooks, `npm run sync:agentes` e
  `npm run check:agentes` com código 0.
