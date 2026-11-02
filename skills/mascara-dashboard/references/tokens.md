# Tokens

Valores de partida para cada passada. Se o projeto já tem um bom sistema, mantenha os valores dele e só corrija o uso. São pontos de partida, não um estilo da casa — deixe a direção ajustá-los.

## Escala de espaçamento

4, 8, 12, 16, 20, 24, 32, 40, 48, 64, 80, 96, 128

- Dentro de um controle: 4–12
- Entre itens relacionados (linhas de lista): 2–8
- Entre grupos (rótulo e sua lista, dois cards): 12–24
- Entre seções: 32–64; seções de landing 80–128
- Alturas de linha: 32 compacta, 36 padrão, 40–44 toque
- Hero: 96–128 da navegação até o título no desktop, 48–64 no celular

## Layout de app

- Sidebar 240–280 de largura; conteúdo fluido com padding 24–32, limitado a ~1440–1600.
- Barra superior ou cabeçalho da página: 56–64 de altura.
- Linhas de navegação 32–36, gap 2–4; rótulos de seção 24 acima, 8 abaixo.
- Cards de estatística numa fileira com a mesma altura; geralmente 3 ou 4 compactos por fileira.
- O gráfico principal ocupa pelo menos dois terços da largura e tem 280–360 de altura. Um segundo bloco ao lado é lista ou tabela, mais estreito.

## Escalas de neutros

Para apps e dashboards use grafite (ou algo igualmente cinza) em todas as superfícies. Para landing pages, escolha a escala cujo tom combina com o mundo. Quente combina com papel, madeira, comida, artesanato e tudo que é humano. Tinta combina com noite, céu, água e tudo que é técnico. Você pode tingir a sua própria com saturação bem baixa, para que nenhuma superfície pareça uma cor sozinha.

### Escuro

| Papel | Grafite | Quente | Tinta |
| --- | --- | --- | --- |
| Superfície mais funda (sidebar) | #0f0f10 | #12110f | #07080d |
| Fundo da página | #141415 | #161513 | #0b0d14 |
| Card | #19191b | #1c1a18 | #11141c |
| Elevado (linha ativa, input) | #232325 | #262421 | #1a1e28 |
| Linha fina | texto primário a 8% | texto primário a 8% | texto primário a 8% |
| Texto primário | #ededed | #efe9de | #eef0f5 |
| Texto secundário | #a1a1a6 | #aaa398 | #a3a9b8 |
| Texto apagado e ícones | #85858b | #8a847a | #7a8296 |

### Claro

| Papel | Grafite | Quente | Tinta |
| --- | --- | --- | --- |
| Fundo da página | #fafafa | #f7f4ee | #f5f7fa |
| Card | #ffffff | #fdfbf7 | #ffffff |
| Elevado (linha ativa, input) | #f4f4f5 | #efe9df | #eceff4 |
| Linha fina | texto primário a 8% | texto primário a 8% | texto primário a 8% |
| Texto primário | #171717 | #1f1b16 | #111827 |
| Texto secundário | #525252 | #5e554a | #4b5565 |
| Texto apagado e ícones | #737373 | #7b7266 | #6b7487 |

Texto apagado é só para metadados e legendas, mantendo ~4,5:1 sobre a superfície. Corpo de texto usa primário ou secundário.

Cores semânticas, suavizadas para caber em qualquer escala: positivo #4cc38a no escuro e #16a34a no claro; negativo #e5484d no escuro e #dc2626 no claro.

## Destaque

- Mantenha uma cor de marca real. Gradiente violeta→azul ou qualquer brilho de uma cor para outra é vício, não cor de marca, a menos que o usuário diga o contrário.
- Sem cor de marca, tire do mundo. Mundos quentes: âmbar, coral, laranja-brasa. Mundos frios: cobalto, petróleo, azul-céu limpo. Mundos naturais: musgo, sálvia. Evite a família roxo→azul a menos que a marca seja de fato roxa.
- Texto sobre o destaque com contraste 4,5:1.
- O destaque cobre poucos por cento da tela: ação principal, seleção, um número-chave.

## Botões

- Botões do hero 44–48 de altura; da navegação 32–36; padding lateral 16–20.
- Principal no escuro: quase-branco da escala com texto escuro, ou o destaque. Principal no claro: cor do texto primário como preenchimento com texto branco, ou o destaque.
- Secundário: superfície elevada com linha fina, texto primário.
- Um leve reflexo no topo como `inset 0 1px 0 rgba(255,255,255,0.12)` em botões escuros dá profundidade sem glow.

## Famílias tipográficas

Escolha pela personalidade. Todas são gratuitas (Google Fonts ou similares); a parceira pode vir de qualquer linha.

| Personalidade | Família da interface | Parceira opcional |
| --- | --- | --- |
| Preciso, técnico, calmo | Geist, Inter, IBM Plex Sans | Geist Mono, IBM Plex Mono, JetBrains Mono para números e meta |
| Caloroso, amigável, humano | Instrument Sans, DM Sans, Figtree | Instrument Serif ou Newsreader só no título do hero |
| Editorial, literário, artesanal | Inter ou Instrument Sans na interface | Newsreader, Instrument Serif ou Fraunces nos títulos |
| Brincalhão, ousado | Space Grotesk, Bricolage Grotesque | uma mono para rótulos pequenos |

Serifa de display é só para títulos grandes, nunca rótulos ou botões. Confira se a fonte cobre acentos do português (ã, ç, õ) — todas acima cobrem.

## Escala de tipo

| Uso | Tamanho | Altura de linha | Peso |
| --- | --- | --- | --- |
| Rótulos pequenos, meta, contagens | 12 | 16 | 400, mono bem-vinda |
| Texto secundário, legendas | 13–14 | 20 | 400 |
| Corpo, itens de menu | 14–15 | 20–22 | 400–500 |
| Nome do logo | 16–18 | 1 | 500–600 |
| Subtítulo do hero | 18–20 | 28–30 | 400, cor secundária, máx. 36rem |
| Números de card | 28–32 | 1 | 500, tabular |
| Título da página | 28–36 | 1,15 | 400–500 |
| Título do hero | 56–72 desktop, 36–44 celular | 1,02–1,08 | 400–500 |

Letter-spacing 0 para tudo abaixo de 16px; levemente positivo (0,01em) serve para texto pequeno apagado. Display a partir de 40px pode ir a −0,02em; a partir de 56px, −0,03em. Títulos em português costumam ser mais longos que em inglês — reduza um passo de tamanho se quebrar em mais de 3 linhas.

## Raio

| Elemento | Raio |
| --- | --- |
| Keycap, tag, botão pequeno | 4–6 |
| Linha, input, botão | 8–10 |
| Card | 12–16 |
| Painel ou janela | 14–20 |

Raio aninhado: interno = externo − padding, nunca abaixo de 4. Um card de 16px com padding 8 contém itens de raio 8.

## Ícones

lucide, 16 ou 18px, traço 1,5, cor do texto apagado ou secundário, gap de 8–10px até o rótulo.

## Profundidade

- Escuro: degraus de superfície mais linha fina. Linha ativa pode ter `inset 0 1px 0 rgba(255,255,255,0.12)`.
- Claro: `0 1px 2px rgba(0,0,0,0.05)` para coisas pequenas, `0 8px 24px rgba(0,0,0,0.06)` para flutuantes.

## Animação

Uma curva para tudo: `cubic-bezier(0.22, 1, 0.36, 1)`.

| Uso | Duração |
| --- | --- |
| Hover, clique, toggles | 120–180ms |
| Menus, popovers, tooltips | 160–220ms |
| Entradas, painéis, mudanças de layout | 300–500ms |
| Escalonamento entre itens | 40–60ms, no máximo seis itens |

- Subida na entrada: 6–12px. Escala no clique: 0,97–0,98.
- Anime só cor, fundo, borda, opacidade e transform.

---

Baseado no unslop de Damir Sokolovsky ([@heydamir](https://x.com/heydamir)), CC BY 4.0.
