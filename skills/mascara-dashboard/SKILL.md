---
name: mascara-dashboard
description: "Transforma um site, landing page, dashboard ou tela de app com cara de \"feito por IA\" (vibecoded) numa interface com acabamento de designer profissional e personalidade própria. Faz uma auditoria dos sinais de IA, define uma direção a partir do próprio produto e corrige espaçamento, cor, ícones, textos, tipografia, layout, detalhes, visuais e animação, nessa ordem. Use SEMPRE que o usuário pedir para deixar um site \"mais profissional\", \"com cara de designer\", \"menos genérico\", \"menos cara de IA\", para dar um polimento, repaginar, redesenhar ou limpar uma tela, ou quando a interface mostrar os vícios típicos de IA: gradiente roxo/azul, brilho (glow), texto com gradiente, emoji nos rótulos, selos \"Novo ✨\", bolhas 3D brilhantes, rótulos em CAIXA ALTA espaçada, elementos pulsando, espaçamento irregular ou textos com \"Bem-vindo de volta! 👋\". Funciona com HTML, CSS, Tailwind e React, a partir de código, de um link ou de um print."
license: CC-BY-4.0
metadata:
  baseado-em: "unslop, de Damir Sokolovsky (@heydamir) — https://github.com/heydamir/unslop"
---

# Máscara Dashboard

Adaptação em português do **unslop**, criado por Damir Sokolovsky ([@heydamir](https://x.com/heydamir)), licenciado em CC BY 4.0. Mantenha este crédito em qualquer cópia ou adaptação.

Interface gerada às pressas por IA erra sempre do mesmo jeito: tudo brilha, todo rótulo tem emoji, o espaçamento é aleatório e o texto grita. O objetivo aqui é consertar o acabamento sem mudar o produto. Funcionalidades, conteúdo e ordem das seções ficam. O que muda é que cada tamanho, cor, palavra e imagem passa a ser uma decisão.

Tirar os vícios é só metade do trabalho. Uma tela limpa que poderia ser de qualquer produto é só o próximo template. Toda execução termina com uma tela que só *este* produto poderia ter.

A diferença entre "cara de IA" e trabalho de designer está em **onde fica a riqueza visual**. A versão de IA espalha cor e efeito na moldura — fundos, botões, bordas, rótulos. O designer deixa a moldura quieta e concentra a riqueza em um ou dois momentos de conteúdo que as pessoas lembram: um objeto renderizado, um gráfico bonito, uma imagem do mundo do produto.

Trabalhe como um designer fazendo uma revisão em camadas: uma camada por vez, na tela inteira.

## Como é o resultado bom

- **Um elemento de destaque.** Cada tela tem uma coisa caprichada que carrega cor e acabamento. O resto fica calmo, então ela se lê na hora.
- **Moldura quieta.** Navegação, botões e textos usam neutros levemente tingidos e uma única cor de destaque. Nada brilha, nada compete.
- **Uma ideia clara.** Dá para dizer numa frase o que o visual mostra e por que ele pertence a este produto.
- **Texto sobre espaço calmo.** O título fica numa área deixada vazia para ele, curto e específico, com uma ação principal e no máximo uma secundária.
- **Produto real, material real.** Prévias parecem o app de verdade com dados plausíveis; objetos têm peso, luz e sombra.

## Fluxo

1. **Olhe a tela.** Encontre os arquivos que a renderizam. Se der para abrir no navegador e tirar print, faça isso — julgue o que as pessoas veem, não só o código.
   - **Só um link, sem código?** Busque o HTML da página (WebFetch, navegador ou `curl`), salve como `original.html` e trabalhe numa cópia. Se tiver navegador, tire um print da página ao vivo para comparar. Fundos animados por script não sobrevivem; descreva-os na auditoria.
   - **Só um print?** Recrie a tela como um HTML estático o mais fiel possível e trate isso como o original.
   - Nesses dois casos o resultado é uma página redesenhada em código que o usuário pode entregar a quem cuida do site real. Diga isso no relatório.
2. **Auditoria.** Percorra [references/sinais.md](references/sinais.md) e liste cada sinal encontrado, uma linha cada, dizendo onde ele está.
3. **Decida o tamanho da mudança.** Leia a auditoria com honestidade antes de planejar.
   - **Muita cara de IA** (sinais em cor, tipo, ícones e texto): faça o processo completo.
   - **Pouca** (tela já desenhada, com alguns vícios): modo polimento. Corrija só o que a auditoria achou, tire a direção da marca existente e mantenha paleta, tipografia, layout e visual. Ideias maiores vão como sugestão no relatório.
   - **Nenhuma:** diga isso claramente e sugira no máximo duas ou três melhorias pequenas, com valores exatos. Só aplique se o usuário concordar. Nunca mude uma tela boa só para ser diferente.
4. **Defina a direção e pare.** Escreva as cinco linhas da seção Direção. Mostre auditoria + direção ao usuário e espere resposta antes de editar, porque mudar a direção depois obriga a refazer tudo. Pergunte pela ferramenta de perguntas se houver; senão, em texto, e pare. Só pule a espera se o usuário já disse "pode fazer direto".
5. **Corrija em nove passadas, na ordem.** Termine uma passada na tela toda antes de começar a próxima. Se quase todas as linhas mudam, planeje as passadas em ordem e escreva a tela nova de uma vez, desde que cada passada seja aplicada. Espaçamento vem primeiro porque todo o resto se lê diferente quando o ritmo está certo. Texto vem antes de tipografia e layout porque o tamanho do título decide o tamanho da fonte e a posição. Visuais e animação vêm por último porque devem encaixar numa tela que já funciona sem eles.
6. **Confira.** Rode o checklist do fim deste arquivo, renderize de novo e compare com a auditoria. O que sobrou na lista é corrigido.
7. **Relatório:** a direção, poucas linhas por passada sobre o que mudou, e qualquer prompt de imagem que você escreveu.

Mantenha a execução rápida: renderize para conferir no máximo três vezes. Se for gerar imagem, dispare logo após a direção ser confirmada e siga com as primeiras passadas enquanto ela roda.

Valores exatos de cada passada estão em [references/tokens.md](references/tokens.md). Como escolher e gerar visuais está em [references/visuais.md](references/visuais.md).

## Direção

Antes de mexer em qualquer coisa, escreva cinco linhas curtas. Tire-as do que a página diz que o produto faz e para quem — nunca do que está na moda.

- **Produto.** O que faz e para quem, numa frase simples.
- **Personalidade.** Duas ou três palavras concretas, como `calmo, preciso, um pouco caloroso` ou `rápido, técnico, brincalhão`. Palavras como limpo, moderno, elegante, minimalista e premium são proibidas, porque descrevem qualquer template.
- **Mundo.** O lugar ou material ao qual o produto pertence naturalmente. Um app de notas vive perto de papel e tinta; uma ferramenta de monitoramento, perto de instrumentos e plantão noturno; um app de viagem, perto de mapas e luz de janela. O mundo define o tom dos neutros, a cor de destaque e o visual.
- **Momentos.** Um ou dois lugares onde a tela ganha cor, material e detalhe, escolhidos do que o produto mostra: um cartão renderizado dentro da prévia, um gráfico onde cada cor é uma série, um objeto do mundo ao lado do conteúdo.
- **Assinatura.** Um único detalhe pequeno que só este produto teria, usado de forma consistente: um ponto de status "ao vivo", teclas de atalho para ferramenta de dev, um sublinhado à mão para app educativo, uma linha de rota para app de entrega. Um detalhe, não cinco.

Os exemplos só mostram o formato da resposta. Derive a sua do produto em questão.

Se o produto já tem marca de verdade (logo, cor ou fonte que não seja vício de IA), mantenha e construa a direção em volta. Gradiente violeta→azul, brilhinhos e glow são vício mesmo quando estão no logo, a menos que o usuário diga que fazem parte da marca.

## 1. Espaçamento

- Tudo numa grade de 4px. Margens, paddings, gaps e alturas fixas são múltiplos de 4. Passo de 2px só para ajustes dentro de controles pequenos.
- Mesma coisa, mesmo tamanho. Todas as linhas de uma lista com a mesma altura e o mesmo gap; todos os cards de uma fileira com o mesmo padding.
- O espaço mostra o agrupamento: espaço dentro do grupo menor que espaço entre grupos.
- Tudo alinhado. Ícones numa coluna, rótulos começando na mesma linha, números alinhados à direita numa coluna. Nada empurrado com translate ou margem avulsa.
- Padding segue a densidade: painéis compactos e sidebars ~16, cards 20–24, bordas da página 24–32.
- A navegação é a parte mais densa de um app: linhas de 32–36 de altura com 2–4 entre elas. O rótulo de seção fica mais perto dos seus itens do que da seção acima (ex.: 24 acima, 8 abaixo). Meça a sidebar depois da passada — é onde o espaçamento mais quebra.
- Remova valores avulsos tipo `mt-[13px]` ou `py-[11px]` e troque por passos da escala.

## 2. Cor

- Construa a partir de uma única escala de neutros, levemente tingida para o mundo da direção (grafite, quente ou tinta, em tokens.md). Fundo, superfícies, bordas e texto vêm dessa escala.
- Em apps e dashboards, fundos, superfícies, bordas e texto ficam neutros. As pessoas olham para isso por horas e quem carrega a cor é o conteúdo. Se o fundo parece laranja, marrom, azul ou verde, passou do ponto. Landing pages podem tingir mais.
- Três papéis de texto: primário, secundário e apagado. Não dez lilases quase iguais.
- Na moldura, uma cor de destaque, usada pouco: ação principal, seleção ou o único número que importa.
- Os momentos da direção são a exceção: ali a cor pode ser rica, desde que fique dentro do mundo e cada cor signifique algo.
- Se a marca tem uma cor real, ela vira o destaque e sai das superfícies. Se não tem, tire o destaque do mundo.
- Texto sobre o destaque precisa de contraste 4,5:1. Se não chegar, escureça o destaque ou use texto escuro.
- Em tema escuro, o botão principal pode ser um quase-branco da escala com texto escuro, e o destaque vai para um lugar menor. Costuma parecer mais intencional que um botão colorido.
- Cores semânticas (verde = bom, vermelho = erro) só com significado, e suavizadas para caber na paleta.
- Remova gradientes de matiz em superfícies, texto com gradiente, brilhos e sombras coloridas, manchas radiais de cor e bordas neon.
- Bordas são linhas finas: a cor do texto primário a 6–10% de opacidade.
- Em tema escuro, profundidade vem de degraus de superfície e linhas finas, não de sombra. Em tema claro, sombras neutras, suaves e pequenas.
- Gradiente só como leve mudança de tom dentro de um mesmo neutro (ex.: linha ativa de #2b2b2b a #1f1f1f). Nunca de uma cor para outra.

## 3. Ícones

- Todo emoji usado como ícone ou enfeite vira ícone de linha de um único conjunto. Use o que o projeto já tem; senão, lucide.
- Um tamanho e uma espessura em tudo: 16 ou 18px, traço 1,5.
- Ícones herdam a cor do papel de texto (secundário ou apagado). Nunca cores próprias.
- A caixa do ícone tem a mesma largura em toda linha e o gap até o rótulo é fixo (8 ou 10).
- Corte ícones que não acrescentam nada. Categorias que precisam de cor ganham um pontinho de status.

## 4. Texto

- Títulos dizem o que o produto faz e para quem, em palavras simples, de um jeito que não caberia em outro produto. Use os fatos que já estão na página; não invente.
- Sem ponto de exclamação na interface, e nunca `!!`.
- Sem título de saudação tipo `Bem-vindo de volta, João! 👋`. O título nomeia o contexto: a página ou o período, como `Outubro de 2026`.
- Rótulos curtos: `Buscar`, não `Busque qualquer coisa...`.
- Variação diz com o que compara: `+12% vs. mês passado`, `3 a menos que no mês passado`.
- Títulos, subtítulos, rótulos, botões e legendas sem ponto final. Só parágrafos com várias frases mantêm.
- Sem palavras de hype: revolucione, potencialize, turbine, desbloqueie, mágico, sem esforço, descubra o poder, o futuro de, transforme, "com IA" em tudo. Em inglês também: supercharge, seamless, unlock, game-changing.
- Afirmações que não dá para verificar (`Mais de 10.000 empresas confiam`, `10x mais rápido`) ficam discretas e específicas se o usuário confirmar que são reais, e saem caso contrário. Pergunte e liste no relatório.
- Dados de exemplo parecem reais: números e nomes plausíveis (Mariana Costa, R$ 48.210), nunca `[X]` ou `123.456`.
- Selos como `PRO`, `Novo ✨` ou `Beta 🚀` saem, a menos que o produto realmente precise — e aí viram texto discreto.
- Use os padrões brasileiros quando a página estiver em português: `R$ 1.234,56`, datas `02/11/2026` ou `2 de nov.`, vírgula decimal.

## 5. Tipografia

- Escolha a fonte pela personalidade, entre as famílias de tokens.md. Mantenha a fonte do projeto quando ela for parte de uma marca real. Um padrão tipo Inter que ninguém escolheu pode ser trocado se outra família combinar mais. Uma família para a interface, mais no máximo uma parceira (mono para números/meta ou display para títulos grandes).
- Poucos tamanhos de uma escala e dois pesos, 400 e 500; 600 no máximo para ênfase rara. Nada de títulos 700–900, nada de texto com gradiente.
- Hierarquia vem de tamanho e cor, não de peso.
- Caixa de frase em tudo. `NAVEGAÇÃO` ou `PAGO ESTE MÊS` com tracking largo viram `Navegação` e `Pago este mês`.
- Texto pequeno nunca tem letter-spacing negativo. Tracking apertado só em display grande.
- Números com `tabular-nums` e um formato só na tela. Se um é `R$ 48.210`, o próximo não é `R$ 124.860,40`.
- Sem itálico para ênfase.

## 6. Layout

- Mantenha as seções e a ordem. Dentro de uma seção, alinhamento e proporções podem mudar se ficar mais claro.
- Apps e dashboards mantêm proporções reais: o app ocupa a viewport, sidebar de 240–280 e conteúdo fluido limitado a ~1440–1600. Nunca encolha um app numa coluna estreita centralizada.
- O hero de landing mais forte é uma **cena**: uma imagem ocupando o hero de ponta a ponta, o assunto num lado e o título na parte calma e vazia da mesma imagem, com a prévia do produto subindo da borda inferior.
- Sem cena, use divisão assimétrica (texto num lado, visual com pelo menos metade da largura) ou texto sobre uma prévia grande do produto abaixo. Tudo empilhado e centralizado é o padrão de template; só serve para hero curto sem visual.
- Títulos longos alinhados à esquerda. Centralizado só para uma ou duas linhas curtas.
- Uma ação principal e no máximo uma secundária. O resto sai do hero.
- Navegação quieta: logo, os links existentes, um botão. "Entrar" é link de texto discreto, não segundo botão.
- Componha a primeira tela como um todo, sem faixa morta vazia. Se o conteúdo for curto, deixe a prévia do produto começar baixo e passar da borda, convidando a rolar.
- No celular, tudo empilha em ordem de leitura e prévias densas ficam mais simples (menos linhas e colunas) em vez de encolher. Nenhum texto abaixo de 11px.

## 7. Detalhes

- Raio aninhado: raio interno = raio externo − padding entre eles, nunca abaixo de 4. Controles 8–10, cards 12–16, painéis 14–20. Nem tudo é pílula.
- Contagens e metadados viram texto discreto (muitas vezes mono e apagado) em vez de pílulas brilhantes.
- Atalhos de teclado viram pequenas teclas (keycaps).
- Gráficos sobre grade apagada com rótulos mono apagados. Sem barras arco-íris numa mesma série, sem barras brilhando, sem dias em caixa alta. Se o gráfico é enfeite sem dado, troque por dados que contem algo.
- Hierarquia de gráficos: um gráfico principal claramente maior e caprichado; o resto é menor e de outro tipo (lista ranqueada com barras finas, tabela curta), nunca um segundo gráfico do mesmo tamanho.
- Um destaque por gráfico: o que importa ganha a cor; o resto fica em degraus neutros.
- Cards de estatística são números: rótulo, valor grande e variação com referência. Nada de sparklines, mini-barras ou ícones para preencher.
- Varie os tamanhos. Cards de mesma largura lado a lado com o mesmo conteúdo parecem template. Dê ritmo à grade.
- Tipo de gráfico pelo dado: tendência = linha, comparação = barras, participação = uma barra empilhada ou lista com barras, meta = barra de progresso.
- Estado ativo é um degrau de superfície com linha fina de luz, não gradiente com glow.
- Hover e foco existem e ficam dentro da paleta, com anel de foco visível para teclado.
- O logo é o nome do produto na fonte principal, mais uma marca simples se houver. Sem logotipo em gradiente nem quadradinho com brilhinho.
- A assinatura da direção aparece onde faz sentido e em nenhum outro lugar.

## 8. Visuais

- Enfeite de preenchimento sai: bolhas brilhantes, orbes, nebulosas, cubos flutuando, grades brilhantes, cérebros holográficos e robôs não dizem nada sobre o produto.
- Hero de landing ganha um visual que mostra algo verdadeiro.
- Dashboards e telas de app quase nunca precisam de imagem gerada. Os momentos vêm do próprio produto: gráfico caprichado, números bem compostos, conteúdo real, um status que parece vivo. Um objeto físico do produto (um cartão num app financeiro) normalmente fica melhor feito em código.
- Com ferramenta de geração de imagem, a primeira escolha para hero de landing é uma cena do mundo da direção, larga o suficiente para ficar atrás do hero inteiro, com espaço vazio onde vai o texto.
- Abaixo da cena, ou como visual quando não há ferramenta, mostre o produto: uma prévia em código do que a página já promete, com dados plausíveis. Mostrar o que o texto já afirma não é inventar funcionalidade.
- Sem ferramenta de imagem: construa o que der em código, escreva os prompts do resto e deixe espaços vazios do tamanho certo (superfície lisa, sem texto dentro).
- Leia [references/visuais.md](references/visuais.md) antes desta passada.

## 9. Animação

- Remova animação em loop sem motivo: `animate-pulse` ou `animate-ping` em coisas que não são "ao vivo", shimmer em título, brilho respirando, elementos flutuando, parallax.
- Remova `transition-all`, molas saltitantes, `hover:scale` em cards e qualquer coisa que se mexa mais que alguns pixels no hover.
- Mantenha animação que explica algo: hover é troca rápida de cor ou superfície, clique é leve redução de escala, menu aparece com fade subindo poucos pixels, número que muda faz tween.
- Anime só cor, fundo, borda, opacidade e transform, nomeando (`transition-colors`, `transition-[transform,opacity]`). Nunca width, height, top, left, margens ou blur grande.
- Uma curva de easing e poucas durações (tokens.md).
- No máximo uma entrada ao carregar: fade + subida curta do conteúdo principal, com leve escalonamento.

## Não faça

- Não renomeie o produto, mesmo que tenha "IA" no nome. Mantenha um logo real. Se o próprio logo for vício (emoji, brilhinho em quadrado com gradiente), redesenhe plano: só o nome na fonte nova, ou um símbolo simples numa cor sólida.
- Não mude o que o produto é. Mantenha funcionalidades, conteúdo e ordem das seções. Conteúdo placeholder sem significado pode virar conteúdo com significado.
- Não troque decoração removida por decoração nova, nem uma moda por outra (glassmorphism, granulado, ruído, neon, bento grid).
- Não invente funcionalidades, afirmações ou dados.
- Não caia sempre no mesmo visual para todo produto. A direção decide tom, fonte e visual — não o hábito.

## Checklist

- [ ] Direção escrita e todas as passadas seguem ela
- [ ] Todo espaçamento na escala de 4px; coisas iguais com tamanhos iguais
- [ ] Ícones, rótulos e números alinhados cada um numa coluna
- [ ] Uma escala de neutros tingida, três papéis de texto, um destaque com contraste suficiente
- [ ] Sem gradiente de matiz, texto com gradiente, glow, sombra colorida ou manchas de cor
- [ ] Nenhum emoji na interface
- [ ] Um conjunto de ícones, um tamanho, um traço
- [ ] Fonte escolhida pela personalidade, pesos 400–600, sem caixa alta espaçada, sem itálico, sem tracking negativo em texto pequeno
- [ ] Sem exclamação, sem ponto final em textos curtos, sem título de saudação, sem afirmação não verificada
- [ ] Números num formato só, com algarismos tabulares (e padrão BR se a página é em português)
- [ ] Raios aninhados batem
- [ ] Hero tem visual real ou prévia do produto com pelo menos um momento — nunca enfeite e nunca placeholder com rótulo
- [ ] Primeira tela composta como um todo, sem faixa morta
- [ ] Sem animação em loop ou saltitante, uma curva de easing, sem animar propriedades de layout
- [ ] **Teste do template:** se você trocasse o nome do produto pelo de outro, a tela ainda serviria? Se sim, force mais a direção no texto, no visual e na assinatura

---

Baseado no unslop de Damir Sokolovsky ([@heydamir](https://x.com/heydamir)), CC BY 4.0. Mantenha este crédito em cópias e adaptações.
