# claude-config

Fonte oficial das orientações gerais do Claude Code para todos os projetos.

O arquivo [`CLAUDE.md`](./CLAUDE.md) deste repositório é a fonte de verdade. Ele fica linkado em `~/.claude/CLAUDE.md` via symlink, então qualquer edição feita aqui (e commitada) já vale para todas as sessões do Claude Code na máquina.

## Como funciona

```
~/.claude/CLAUDE.md  →  symlink  →  ~/claude-config/CLAUDE.md (este repo)
```

## Editando

Edite o `CLAUDE.md` normalmente, revise com `git diff`, e commit:

```bash
cd ~/claude-config
git add CLAUDE.md
git commit -m "docs: atualiza orientações gerais"
git push
```

## Projetos específicos

Este repositório guarda apenas as orientações **gerais**. Projetos individuais devem ter seu próprio repositório no GitHub, cada um com seu próprio `CLAUDE.md` local complementando este (ver seção 12 do documento).

## Projetos relacionados

- [dashboard-verba-clientes](https://github.com/oivanfelipe/dashboard-verba-clientes) —
  acompanhamento de verba e investimento em Meta Ads e Google Ads por cliente.
  Nasceu aqui e foi movido para repositório próprio com o histórico preservado.
