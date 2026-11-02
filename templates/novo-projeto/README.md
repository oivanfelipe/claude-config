# novo-projeto (template)

Template de repositório com o setup mínimo do Claude Code para projetos novos.

## O que vem pronto

| Caminho | Função |
|---|---|
| `CLAUDE.md` | Contexto do projeto + regra de usar o blueprint antes de construir app |
| `.claude/skills/vibecode-blueprint/` | Skill que gera os 6 documentos de planejamento |
| `docs/blueprint/` | Destino dos 6 documentos (PRD, TRD, AppFlow, Design Brief, Backend Schema, Plano) |

## Usar

```bash
gh repo create <nome> --template oivanfelipe/novo-projeto --private --clone
cd <nome>
```

Depois preencha a seção "Sobre o projeto" do `CLAUDE.md` e peça ao Claude: "quero criar um app ...".

## Atualizar a skill

A fonte da skill é `oivanfelipe/claude-skills`. Para trazer a versão mais recente:

```bash
tmp=$(mktemp -d) && git clone --depth 1 https://github.com/oivanfelipe/claude-skills "$tmp" \
  && rm -rf .claude/skills/vibecode-blueprint && cp -r "$tmp/vibecode-blueprint" .claude/skills/ && rm -rf "$tmp"
```
