---
name: kiso-workflow
description: >-
  Metodologia Cadeia Kiso — usa briefings, notas, transcrições ou entrevista
  para construir um plano de ação de estratégia de marca e conteúdo, do
  diagnóstico estratégico ao calendário editorial executável. São 13 etapas
  encadeadas em que cada etapa consome as "Variáveis-chave" das anteriores.
  Use SEMPRE que o usuário quiser montar, estruturar ou revisar posicionamento
  de marca, autoridade, plano de conteúdo ou plano de ação estratégico para um
  profissional, negócio ou marca (inclusive posicionamento médico/profissional),
  ou quando mencionar: kiso-workflow, Cadeia Kiso, etapa Kiso, diagnóstico estratégico,
  objetivo estratégico, ICP, persona estratégica, posicionamento estratégico,
  brand persona, manifesto de marca, territórios de marca, radar de canais,
  guia editorial, temas centrais, banco de ideias ou calendário de posts.
  Use também quando pedirem para "continuar a cadeia", "avançar uma etapa",
  ou gerar/revisar qualquer um desses artefatos.
---

# Cadeia Kiso

A Cadeia Kiso é uma **metodologia encadeada** que transforma um profissional, negócio ou marca — de um diagnóstico estratégico inicial até um calendário editorial pronto para executar. São **13 etapas em sequência**. O que torna isto uma *cadeia*, e não uma lista solta de exercícios, é o **contrato de dados**: cada etapa termina com um bloco `Variáveis-chave` (YAML), e a etapa seguinte **consome** essas variáveis como entrada. Nada é decidido do zero duas vezes; cada decisão flui para frente.

Esta skill é **genérica**: funciona para qualquer marca ou profissional. Onde um exemplo ajuda, use um marcador neutro entre colchetes (ex.: `[segmento]`, `[categoria de mercado]`), nunca um caso real embutido.

## Como conduzir a cadeia

Identifique a marca e a etapa a partir do pedido e dos arquivos disponíveis. Para um projeto novo, comece pela Etapa 01, salvo se o usuário indicar outra. Pergunte pela marca ou etapa somente se não for possível identificá-las.

### Começar com material existente

1. Leia primeiro o briefing, as notas, a transcrição ou os artefatos disponíveis. Extraia o que já responde ao roteiro e preserve a origem das informações quando for relevante. Guarde para as etapas seguintes os dados que pertencem a elas.
2. Carregue a referência da etapa e as `Variáveis-chave` de que ela precisa. Use o roteiro como checklist de cobertura. Preencha o rascunho com as informações disponíveis, distinguindo fatos fornecidos, hipóteses e `[LACUNA: ...]`.
3. Pergunte apenas quando uma resposta mudar uma decisão em aberto, desbloquear uma entrega ou resolver uma contradição relevante. Registre lacunas que podem esperar e entregue o rascunho. Se não houver material suficiente, entreviste em blocos de até quatro perguntas.

### Rascunho e aprovação

Para cada etapa, siga o modelo de artefato, inclua o YAML obrigatório e confira a coerência com as entradas. Salve o artefato e atualize o `MAPA.md`.

Quando o usuário pedir rascunhos de várias etapas, encadeie-os em ordem usando os YAMLs provisórios e indique quais dependências ainda precisam de validação. Entregue o lote para uma revisão conjunta, sem pedir aprovação intermediária. Se uma lacuna bloquear parte do lote, entregue o que for viável e agrupe as perguntas que destravam o restante.

Peça validação explícita para aprovar decisões materiais novas ou alteradas, como ICP, promessa ou compromisso de cadência. Agrupe essas decisões na mesma revisão. Só marque como aprovado o que o usuário validou e preserve a versão aprovada quando preparar um rascunho de alteração.

### Retomar um projeto

Leia o `MAPA.md` e os artefatos que ele aponta. Identifique o último ponto aprovado e confira as dependências da etapa solicitada. Se não houver mapa, localize os artefatos na pasta do projeto e use o status registrado neles. Preserve as decisões já aprovadas.

Quando faltar uma chave em um artefato antigo, recupere-a no YAML a partir do texto aprovado se ele for explícito e coerente com as outras fontes. Se a informação estiver ausente, ambígua ou em conflito, pergunte apenas se ela for necessária para a entrega ou a decisão solicitada.

## As 13 etapas

| # | Etapa | Consome (entradas) | Produz (essência) | Referência |
|---|-------|--------------------|-------------------|------------|
| 01 | Diagnóstico Estratégico | — (entrevista inicial) | retrato do negócio, diferencial, ambição, exclusões | `references/etapa-01-diagnostico.md` |
| 02 | Objetivo Estratégico | 01 | momento, objetivo de 3–6 meses, KPI, viabilidade | `references/etapa-02-objetivo.md` |
| 03 | ICP | 01, 02 | perfil de cliente ideal e anti-ICP | `references/etapa-03-icp.md` |
| 04 | Persona Estratégica | 03 | decisor simbólico: dores, desejos, decisão, linguagem | `references/etapa-04-persona.md` |
| 05 | Posicionamento Estratégico | 01, 03, 04 | categoria, inimigo, promessa, diferencial, bandeira | `references/etapa-05-posicionamento.md` |
| 06 | Brand Persona | 05, 03, 04 | território motivacional, arquétipo, tom de voz | `references/etapa-06-brand-persona.md` |
| 07 | Manifesto de Marca | 01, 03, 04, 05, 06 | núcleo ideológico + manifesto público | `references/etapa-07-manifesto.md` |
| 08 | Territórios de Marca | 01, 03, 04, 05, 06, 07 | 3–6 lentes temáticas duradouras (dentro/fora) | `references/etapa-08-territorios.md` |
| 09 | Radar de Canais | 02, 04, 05, 08 (todas) | etapa-gargalo + canais priorizados e cadências | `references/etapa-09-radar-canais.md` |
| 10 | Guia Editorial | 05, 06, 07, 08, 09 (todas) | regras de conteúdo por etapa da jornada e por canal | `references/etapa-10-guia-editorial.md` |
| 11 | Temas Centrais | 08, 09, 10 (todas) | temas recorrentes por território, priorizados | `references/etapa-11-temas-centrais.md` |
| 12 | Banco de Ideias | 08, 09, 10, 11 | repositório de ideias executáveis por tema/canal | `references/etapa-12-banco-de-ideias.md` |
| 13 | Calendário de Posts | 09, 10, 11, 12 | cronograma editorial sustentável (30/60/90 dias) | `references/etapa-13-calendario.md` |

Conceitos próprios do método (jornada de 5 etapas, Needscope, arquétipos, 5S, Score A(c), Matriz Canal × Etapa, teste do "sem logo", etapa-gargalo) estão definidos em `references/glossario.md`. Leia-o na primeira vez que um conceito aparecer.

## Princípios inegociáveis da cadeia

- **O contrato manda.** Toda etapa consome `Variáveis-chave` anteriores e entrega as suas. Se uma entrada estiver faltando, resolva a etapa que falta antes (ou registre `[LACUNA: ...]` e siga com cautela).
- **Não invente dados.** Preço, faturamento, concorrentes, números — só entram se vierem do usuário. Onde faltar, use `[LACUNA: ...]`. É melhor uma lacuna explícita do que um número inventado que contamina todas as etapas seguintes.
- **Coerência antes de avançar.** Cada etapa tem checagens próprias (ex.: promessa sustentável? território sem sobreposição? cadência é viável?). Rode-as e mostre as tensões ao usuário.
- **Nunca prometa resultado garantido.** A metodologia constrói autoridade de substância, não hype. Evite linguagem de garantia ("resultado certo", "sucesso garantido").
- **Respeite o setor.** Em domínios regulados (saúde, jurídico, financeiro), aplique as regras de compliance que aparecem no Guia Editorial e não produza conteúdo que viole normas do conselho/categoria.
- **Teste do "sem logo".** Territórios, temas e conteúdo devem ser reconhecíveis como *desta* marca mesmo sem assinatura. Se qualquer concorrente genérico pudesse ter dito o mesmo, refine.

## Modelo de artefato

Todo artefato de etapa segue o mesmo formato — cabeçalho, corpo em seções, bloco `Variáveis-chave`, alertas de coerência e próxima etapa. O molde completo está em `references/modelo-artefato.md`. Use-o sempre para que os documentos fiquem consistentes e legíveis pela própria cadeia.

## Onde salvar e como nomear

Salve os artefatos como Markdown, para que virem a memória viva do projeto:

- **Etapas 01–11:** em uma pasta do projeto (ex.: `cadeia-kiso/`), no formato `AAAA-MM-DD-<etapa-slug>-<projeto-slug>.md` (ex.: `2026-06-01-diagnostico-estrategico-<projeto>.md`).
- **Etapa 12 (Banco de Ideias):** em `bancos-de-ideias/` (é massa editorial executável, separada do núcleo estratégico).
- **Etapa 13 (Calendário):** em `calendarios-editoriais/`.
- Mantenha um **`MAPA.md`** na pasta do projeto: índice com caminho e status de cada etapa: pendente, rascunho ou aprovado.

Se o usuário tiver uma pasta conectada, salve lá. Caso contrário, salve na pasta de trabalho e ofereça o arquivo. Ao final da cadeia, o calendário pode ser exportado para planilha se o usuário quiser (então use a skill de xlsx).
