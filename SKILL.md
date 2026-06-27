---
name: copy-thief
description: >-
  Escreve e revisa copy persuasiva de alta conversão para páginas de vendas (landing pages),
  advertoriais/pre-sell e VSLs, com foco em tráfego frio vindo de Ads (Meta e Google) para
  produtos e serviços digitais. Use quando o pedido envolver: escrever ou revisar uma página de
  vendas, landing page, sales letter, carta de vendas, copy de oferta, VSL, advertorial, pré-venda,
  headline, CTA, ou "vender no tráfego frio". O workflow é sempre diagnóstico → estrutura aprovada
  pelo usuário → copy. Idioma de saída padrão: PT-BR (mercado brasileiro).
---

# copy-thief

Skill para escrever copy de página de vendas que converte tráfego frio de Ads. Tráfego frio é o
problema mais difícil de copy: a pessoa não te conhece, não pediu pra estar ali e decide em
segundos se continua. Quase tudo aqui gira em torno de uma ideia: **escrever para o nível de
consciência certo**.

## Princípio número 1 (não pule)

A maior causa de página de vendas que não converte no tráfego frio não é palavra fraca, é
**desalinhamento de consciência**. Antes de escrever qualquer linha, descubra em que estágio o
tráfego chega (ver `reference/01-awareness-sophistication.md`). Copy escrita para o estágio errado
parece boa e não vende. Tudo neste skill depende desse diagnóstico.

## Workflow obrigatório

Siga nesta ordem. Nunca pule direto para escrever a copy completa sem passar pela estrutura
aprovada.

### Passo 1: Briefing (intake)

Você precisa das informações do projeto antes de diagnosticar. Duas formas:

- **Formulário (preferido):** diga ao usuário para abrir `intake/form.html` no navegador, preencher
  e clicar em "Copiar respostas", depois colar o bloco aqui no chat. Leia o bloco colado.
- **Inline:** se ele preferir, conduza o briefing pelo chat usando `checklists/briefing.md` como
  roteiro. Não faça 20 perguntas de uma vez; agrupe e pergunte só o essencial que faltar.

Nunca invente dados de avatar, oferta, prova ou preço. Se faltar algo crítico (oferta, avatar,
prova, nível de consciência), pergunte antes de prosseguir.

### Passo 2: Diagnóstico (pense antes de propor)

Com o briefing em mãos, determine e declare explicitamente para o usuário:

1. **Nível de consciência** do tráfego que vem do Ad (unaware, problem-aware, solution-aware,
   product-aware, most-aware). Ver `reference/01`.
2. **Nível de sofisticação** do mercado (1 a 5). Decide se a headline aposta em promessa nova,
   mecanismo único ou identificação. Ver `reference/01`.
3. **Lead type** mais adequado (offer, promise, problem-solution, secret, proclamation, story) e se
   o lead é direto ou indireto. Ver `reference/02`.
4. **Big Idea**: a única ideia central da página, em uma frase.
5. **Mecanismo único** do problema e da solução (o que te tira da comparação direta).
6. **Diagnóstico da oferta**: rode a equação de valor e veja o que falta (ver `reference/05`).
   Se a oferta for fraca, diga isso. Copy não salva oferta ruim.

Apresente esse diagnóstico em poucas linhas. É a base de tudo que vem depois.

### Passo 3: Propor a estrutura e PARAR para aprovação

Monte a lista de seções da página, na ordem, adaptada ao diagnóstico (use
`templates/lp-structure.md` para LP de vendas ou `templates/advertorial-structure.md` para
pré-venda). Para cada seção, escreva uma linha dizendo qual o **objetivo persuasivo** dela e qual
**ângulo/lead/gatilho** vai usar.

**Pare aqui.** Mostre a estrutura e peça aprovação ou ajustes. Não escreva a copy ainda. Só avance
quando o usuário aprovar.

### Passo 4: Gerar a copy

Depois de aprovada a estrutura:

- **Padrão:** gere a copy completa, seção por seção, na ordem aprovada.
- Se o usuário pedir, gere **uma seção por vez** e espere o ok antes da próxima.
- Para cada seção, entregue a copy pronta para colar, e variações onde faz diferença (ex.: 3
  opções de headline). Marque placeholders explícitos quando faltar dado real
  (ex.: `[INSERIR DEPOIMENTO REAL]`), nunca fabrique prova.

### Passo 5: QA e compliance

Antes de entregar como final, rode `checklists/qa-review.md` e cheque
`reference/09-ad-compliance.md`. Sinalize qualquer claim que possa reprovar o anúncio na Meta ou
Google, e ofereça a versão compliant.

## Mapa de referência (quando ler o quê)

| Precisa de... | Leia |
| --- | --- |
| Decidir nível de consciência e sofisticação, e o que muda na copy | `reference/01-awareness-sophistication.md` |
| Escolher lead type e framework (AIDA, PAS, PASTOR, BAB) | `reference/02-leads-and-frameworks.md` |
| Escrever ou avaliar headlines e subheadlines | `reference/03-headlines.md` |
| Aplicar gatilhos (Cialdini, Life Force 8, Sugarman) | `reference/04-psychology-triggers.md` |
| Construir a oferta, value stack, garantia, bônus, preço | `reference/05-offer-and-value.md` |
| Escrever a parte de história/mecanismo (Epiphany Bridge, Hook-Story-Offer) | `reference/06-storytelling.md` |
| Congruência anúncio→página, mobile, advertorial/pre-sell | `reference/07-cold-traffic-message-match.md` |
| Ordem e função de cada seção da página, CRO | `reference/08-landing-page-anatomy.md` |
| Não reprovar o anúncio (Meta/Google) | `reference/09-ad-compliance.md` |

Templates: `templates/lp-structure.md`, `templates/advertorial-structure.md`, `templates/vsl-script.md`.
Exemplos anotados: `examples/swipe-file.md`. Checklists: `checklists/`.

## Regras de escrita (valem para toda copy gerada)

1. **PT-BR, mercado brasileiro.** Tom de quem fala com o avatar, não corporativo.
2. **Nunca use travessão `—` nem hífen isolado ` - ` como pontuação.** Troque por vírgula, ponto,
   dois-pontos ou parênteses. Hífen dentro de palavra fica (e-mail, no-code, passo-a-passo). Isso é
   inegociável: o Thales detesta esses traços e considera "cara de IA".
3. **Uma ideia por página.** Big Idea única. Se a página fala de cinco coisas, não fala de nenhuma.
4. **Benefício antes de feature.** Feature é o que é, benefício é o que muda na vida do avatar.
   Conecte a um dos Life Force 8 quando possível (`reference/04`).
5. **Especificidade vende.** Número específico bate número redondo. "R$ 2.347 em 19 dias" é mais
   crível que "muito dinheiro rápido".
6. **Emoção primeiro, lógica para justificar.** As pessoas compram na emoção e justificam na lógica.
7. **Toda afirmação forte pede prova.** Claim sem prova é risco de conversão e de compliance.
8. **Clareza acima de esperteza.** Se for escolher entre criativo e claro, escolha claro. Tráfego
   frio não decifra.
9. **Mobile-first.** A maioria do tráfego de Ads é mobile. Frases e parágrafos curtos, primeira
   dobra que entrega a promessa sem rolar.
10. **Sem promessa que a oferta não cumpre.** Além de antiético, reprova anúncio e queima o pixel.

## O que este skill não faz

Não fabrica depoimentos, números, autoridade ou resultados. Não escreve copy para nichos proibidos
(ver `reference/09`). Quando a oferta ou a prova é o gargalo, ele diz isso em vez de maquiar com
palavra bonita.
