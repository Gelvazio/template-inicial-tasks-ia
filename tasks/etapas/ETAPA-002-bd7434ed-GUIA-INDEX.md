## Etapa 002-bd7434ed — GUIA: Página `index.html` explicando a estrutura inicial de projetos de IA

**Tarefa:** GUIA · **Pedido em:** 2026-10-14 09:01 · **Criada por:** Claude Code (Opus 5.5) (local · main)
**Pedido:** "CRIE UN INDEX.HTML, EXPLICANDO COMO FUNCIONA A ESTRUTURA INICIAL DE PROJETOS DE IA"
**Objetivo:** uma página na raiz que explica, para quem não é técnico, como o template funciona.

### GUIA.1 — Criar o `index.html` e o estilo da página-guia

**Próximo passo:** nenhum — concluída.

- **Nível:** MEDIO — página nova em 2 arquivos, sem banco nem segredo
- **Descrição:** página estática com: o que é o template, mapa das pastas, ciclo da tarefa, reserva
  entre várias IAs, níveis e equipe de agentes, hooks, skills por IA e como começar um projeto.
- **Critérios de Aceitação:** HTML semântico, CSS separado com tokens em `:root`, tema claro e
  escuro, legível no celular, links para as regras; sem abrir navegador para validar.
- **Entrega:** commit `feat(GUIA.1)` (`index.html` + `guia/estilo.css`) · **Verificação:**
  tags do HTML conferidas por parser (nenhuma aberta ou trocada), nenhuma linha acima de 100
  caracteres, sem `style=`/`onclick`/`<script>`; visual não conferido no navegador (regra do
  projeto) — abrir o `index.html` para ver.
