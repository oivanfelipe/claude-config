# CLAUDE.md — Projeto

> Este arquivo complementa as orientações gerais (`oivanfelipe/claude-config`). Em sessões na nuvem as orientações gerais não são carregadas, então o essencial está repetido aqui.

## Sobre o projeto

- **Nome:** (preencher)
- **Objetivo:** (uma frase: que problema resolve e para quem)
- **Stack:** (preencher após o TRD)
- **Publicação:** (ex.: GitHub → Vercel; `index.html` é o arquivo oficial de produção, quando aplicável)

## Criação de app, MVP ou produto digital

Antes de escrever qualquer código ou prompt para app builder (Claude Code, Cursor, Vibecode, Lovable, Bolt, v0), use a skill `vibecode-blueprint` (`.claude/skills/vibecode-blueprint/`).

- Gere os 6 documentos em `docs/blueprint/`: `01-prd.md`, `02-trd.md`, `03-appflow.md`, `04-design-brief.md`, `05-backend-schema.md`, `06-implementation-plan.md`.
- Se `docs/blueprint/` já tiver os documentos, leia e valide antes de construir. Não recrie do zero.
- Durante a construção, os 6 documentos são a fonte de verdade: PRD define o escopo, TRD a stack, AppFlow as telas, Design Brief o visual, Backend Schema os dados, Plano de Implementação a ordem.
- Mudou uma decisão? Atualize o documento correspondente no mesmo commit.

## Regras essenciais

- Idioma: português do Brasil.
- Faça a menor alteração necessária. Preserve funcionalidades existentes. Não adicione dependências sem necessidade.
- Não crie arquivos `_v2`, `_final`, `_novo`. O histórico é do Git.
- Nunca faça commit de senhas, tokens, API keys ou `.env` com dados sensíveis.
- Nunca execute sem autorização explícita: `git reset --hard`, `git push --force`, exclusão de branches, remoção em massa.
- Antes de commit: revise `git diff`. Depois de alterar: valide (testes, layout, responsividade) e diga o que não foi possível validar.
- Ao concluir: informe o que mudou, quais arquivos, como foi validado e próximos passos.
