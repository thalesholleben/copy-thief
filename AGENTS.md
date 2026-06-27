# AGENTS.md

Este repositório é uma **skill do Claude Code** (e compatível com qualquer agente que leia
arquivos de instrução). Ele não tem build nem testes: é uma base de conhecimento + workflow para
escrever copy de alta conversão para tráfego frio de Ads (Meta e Google), em PT-BR.

## Ponto de entrada

`SKILL.md` é a fonte da verdade operacional. Contém o frontmatter (`name`, `description`) que
aciona a skill e o **workflow obrigatório**: diagnóstico → estrutura aprovada pelo usuário → copy.
Leia `SKILL.md` antes de qualquer coisa.

## Mapa do repositório

- `SKILL.md` — roteador + workflow obrigatório.
- `reference/` — base de conhecimento (ler sob demanda; ver tabela em `SKILL.md`).
- `templates/` — esqueletos de página: `lp-structure.md`, `advertorial-structure.md`, `vsl-script.md`.
- `intake/form.html` — formulário de briefing client-side (o usuário preenche e cola o resultado).
- `examples/swipe-file.md` — exemplos anotados.
- `checklists/` — `briefing.md` e `qa-review.md`.

## Regras que não podem ser quebradas

1. **Nunca pule o workflow.** Não gere copy completa sem antes diagnosticar e ter a estrutura
   aprovada pelo usuário.
2. **Nunca fabrique prova** (depoimentos, números, autoridade, resultados). Use placeholders
   explícitos como `[INSERIR DEPOIMENTO REAL]`.
3. **Pontuação:** nunca use travessão `—` nem hífen isolado ` - ` como pontuação. Hífen dentro de
   palavra é permitido. Detalhes em `SKILL.md`.
4. **Idioma de saída:** PT-BR, mercado brasileiro.

## Como rodar / instalar

Copie ou aponte esta pasta para `~/.claude/skills/copy-thief`. Não há dependências, install ou
build. O `intake/form.html` abre direto no navegador.

## O que ignorar

`.firecrawl/` (material bruto raspado das fontes) não é versionado e não é necessário: a síntese
própria está em `reference/`.
