# copy-thief

Skill do Claude para escrever copy de **alta conversão** para páginas de vendas (landing pages),
advertoriais e VSLs, com foco em **tráfego frio vindo de Ads** (Meta e Google), para produtos e
serviços digitais.

A ideia central: tráfego frio é o problema mais difícil de copy. A skill não sai escrevendo. Ela
**diagnostica** o nível de consciência e sofisticação do tráfego, **propõe a estrutura** da página
e só escreve a copy **depois que você aprova**.

## Como usar
1. Peça ao Claude para escrever/revisar uma página de vendas. A skill é acionada por temas como
   "página de vendas", "landing page", "VSL", "advertorial", "copy de oferta", "tráfego frio".
2. **Briefing:** abra `intake/form.html` no navegador, preencha, clique em **Copiar respostas** e
   cole o bloco no chat. (Ou faça o briefing pelo chat.)
3. **Diagnóstico:** o Claude declara consciência, sofisticação, lead, Big Idea, mecanismo e um
   diagnóstico da oferta.
4. **Estrutura:** ele propõe as seções na ordem e **para para você aprovar**.
5. **Copy:** aprovada a estrutura, ele gera a copy completa (ou seção por seção, se você pedir).
6. **QA + compliance:** revisa contra checklist e políticas de Meta/Google antes de entregar.

## Instalação
Para o Claude Code reconhecer como skill ativa, copie ou aponte esta pasta para
`~/.claude/skills/copy-thief` (no Windows, `C:\Users\Thales\.claude\skills\copy-thief`).

## Estrutura
```
copy-thief/
├── SKILL.md                  # roteador + workflow obrigatório (diagnóstico → estrutura → copy)
├── reference/                # base de conhecimento (ler sob demanda)
│   ├── 01-awareness-sophistication.md   # Schwartz (o coração)
│   ├── 02-leads-and-frameworks.md       # Great Leads + AIDA/PAS/PASTOR/BAB
│   ├── 03-headlines.md
│   ├── 04-psychology-triggers.md        # Cialdini + Life Force 8 + Sugarman
│   ├── 05-offer-and-value.md            # Hormozi: $100M Offers + Money Models
│   ├── 06-storytelling.md               # Epiphany Bridge + Hook-Story-Offer
│   ├── 07-cold-traffic-message-match.md
│   ├── 08-landing-page-anatomy.md       # CRO
│   └── 09-ad-compliance.md              # Meta + Google
├── templates/                # esqueletos: lp-structure, advertorial-structure, vsl-script
├── intake/form.html          # formulário de briefing (copiar e colar)
├── examples/swipe-file.md    # exemplos anotados (o porquê de cada escolha)
└── checklists/               # briefing.md e qa-review.md
```

## Fontes da pesquisa
Eugene Schwartz (*Breakthrough Advertising*), Alex Hormozi (*$100M Offers*, *$100M Money Models*,
2025), Masterson & Forde (*Great Leads*), Robert Cialdini (*Influence*), Drew Whitman
(*Cashvertising*), Joseph Sugarman (*Triggers*), Russell Brunson (Epiphany Bridge / Hook-Story-Offer),
David Ogilvy e John Caples (headlines), CXL (CRO), e as políticas oficiais de anúncios de Meta e
Google. A síntese própria desse material vive em `reference/`.

## Regra de estilo (importante)
Toda copy gerada é PT-BR e **nunca** usa travessão `—` nem hífen isolado ` - ` como pontuação
(preferência do Thales). Hífen dentro de palavra é permitido.
