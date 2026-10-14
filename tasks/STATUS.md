# STATUS — Template inicial de tarefas com IA

**Objetivo:** esqueleto para começar qualquer projeto com IA: regras únicas para todas as IAs e
quadro de tarefas que sobrevive à queda da sessão.
**Partes interessadas:** Gelvazio (decide, aprova e usa) · agentes de IA executam pelo quadro.
**Links:** [Regras](../AGENTS.md) · [Etapas](etapas/) · [Concluídas](task_complete.md) · [Recados](RECADOS.md)

Legenda: ⬜ Pendente · 🔄 Em progresso · ✅ Concluído · ⛔ Bloqueado · 👀 Aguardando o usuário ·
Prioridade: 🔴 Máxima · 🟠 Alta · 🟡 Média · 🟢 Baixa

## 📌 Tarefas

Cada **subtarefa** é uma linha própria e pode ser reservada por **qualquer IA** (coluna "Em uso por"). A linha em
**negrito** é a tarefa-mãe: não se reserva; ela fecha quando todas as subtarefas estiverem ✅. Aqui só ficam
tarefas **abertas ou em andamento**: linha que vira ✅ é movida para o [`task_complete.md`](task_complete.md).

| Tarefa | Título | Prioridade | Depende de | Status | Em uso por | Etapa |
|---|---|---|---|---|---|---|

## Escopo do projeto

- **Entra:** regras em `.claude/rules/`, quadro em `tasks/`, skills e agentes em `.agents/` (com as
  cópias por IA), hooks do Claude Code e do Git, visualizador de regras e tarefas.
- **Não entra:** código de aplicação. Ao criar um projeto a partir deste template, troque este
  objetivo e este escopo pelos do projeto.

## 🗂️ Etapas

| Etapa | Assunto | Arquivo |
|---|---|---|
| 001-db7a9bca | TEMPLATE: criar o esqueleto a partir do Dashboard AI | [ETAPA-001-db7a9bca-CRIAR-TEMPLATE.md](etapas/ETAPA-001-db7a9bca-CRIAR-TEMPLATE.md) |
| 002-bd7434ed | GUIA: página `index.html` explicando a estrutura inicial | [ETAPA-002-bd7434ed-GUIA-INDEX.md](etapas/ETAPA-002-bd7434ed-GUIA-INDEX.md) |

## Riscos

| Risco | Chance | Impacto | Plano B | Situação |
|---|---|---|---|---|
| Duas frentes editarem o `STATUS.md` ao mesmo tempo | Média | Conflito no push | Cada frente mexe só nas próprias linhas; sincronizar e reler antes do push | Acompanhando |

## Bloqueios gerais (sem tarefa)

| Data | Motivo | O que destrava | Resolvido em |
|---|---|---|---|

## Registro de decisões

| Data | Decisão | Quem | Por quê |
|---|---|---|---|
| 2026-10-14 08:47 | Template criado copiando o controle de tarefas do Dashboard AI, sem nada específico dele (Supabase, Laya, histórico); entram a equipe de agentes e o visualizador; o `sincronizar-agentes.mjs` passa a gerar também os agentes do Codex | Gelvazio | Pedido no chat: "copie pra esta pasta aqui, como um esqueleto inicial de qualquer projeto com IA"; escopo escolhido na pergunta |

## Pendências (ficou para depois)

| Data | Pendência | Motivo |
|---|---|---|

## Lições aprendidas

| Data | Lição | Regra criada |
|---|---|---|
