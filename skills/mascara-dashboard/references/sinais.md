# Sinais de "cara de IA"

Percorra todos os grupos e anote cada sinal encontrado, com o lugar onde ele aparece. Cada linha traz o sinal → a correção.

## Superfícies e cor

- Gradientes roxo→azul ou violeta→rosa em fundos, cards, botões ou item ativo do menu → uma superfície neutra, destaque só onde significa algo
- Texto com gradiente em títulos, números ou logo → cor sólida de texto primário
- Brilhos coloridos, tipo `shadow-[0_0_20px_rgba(139,92,246,0.5)]`, `drop-shadow` em emoji ou pílulas brilhando → remover; profundidade por degraus de superfície e linhas finas
- Manchas radiais de cor ou blobs desfocados atrás do conteúdo → remover
- Bordas neon ou coloridas de alto contraste → linha fina a 6–10% de opacidade
- Vários tons quase iguais da mesma cor no texto (cinco lilases) → três papéis de texto de uma escala neutra
- Tudo destacado, então nada se destaca → um destaque usado uma ou duas vezes por tela
- Cards de vidro (glassmorphism) com reflexo branco e sombra colorida → superfície elevada simples com linha fina

## Tipografia

- Títulos com peso 800 ou 900 → 400–500, hierarquia pelo tamanho
- Rótulos em CAIXA ALTA com tracking largo (`NAVEGAÇÃO`, `PAGO ESTE MÊS`) → caixa de frase, tracking normal
- Tamanhos e pesos demais numa tela → poucos tamanhos da escala, pesos 400 e 500
- Números em formatos misturados (`R$ 48.210` ao lado de `R$ 124.860,40`, ou `07`) → um formato, algarismos tabulares
- Formato americano numa página em português (`$1,234.56`, `11/02/2026` para 2 de novembro) → `R$ 1.234,56`, `02/11/2026`
- Letter-spacing negativo em texto pequeno → zero ou levemente positivo
- Itálico para ênfase → cor ou peso

## Ícones

- Emoji como ícone de menu, enfeite de rótulo ou status (🏠 📥 🚀 💰 ⚠️ 📈 🔥) → um conjunto de ícones de linha, ou nada
- Emoji dentro de pílulas e contagens (`18 👤`) → número simples
- Ícones de vários tamanhos e cores → um tamanho, um traço, cor do papel de texto
- Ícones fora da coluna → mesma largura de caixa em toda linha
- Brilhinho ✨ para qualquer coisa com IA → remover, ou ícone simples só onde explica algo

## Espaçamento

- Valores arbitrários (`mt-[13px]`, `ml-[7px]`, `h-[31px]`) → passos da escala de 4px
- Linhas da mesma lista com alturas ou gaps diferentes → uma altura, um gap
- Grupos mais perto do vizinho do que dos próprios itens → gap menor dentro, maior entre grupos
- Padding desigual em cards irmãos → um padding
- Vão enorme acima de uma seção e aperto abaixo → ritmo equilibrado

## Texto

- Título de saudação (`Bem-vindo de volta, João! 👋`, `Olá, Ana! Pronta para arrasar hoje?`) → nome da página ou do período
- Exclamações e `!!` → afirmação simples
- Variação sem referência (`+12%!!`, `3 a menos!!`) → `+12% vs. mês passado`
- Placeholder prolixo (`Pesquise qualquer coisa...`) → `Buscar`
- Hype: revolucione, potencialize, turbine, eleve, desbloqueie, mágico, sem esforço, o futuro de, descubra o poder, "com IA" em tudo → o que a coisa realmente faz
- Ponto final em rótulos e botões → sem ponto
- Dados com cara de falso (`R$ 123.456`, `[X]`, `Usuário 1`) → números e nomes plausíveis
- Texto traduzido ao pé da letra do inglês ("Comece agora gratuitamente hoje", "Leve seu negócio para o próximo nível") → português natural e direto

## Componentes

- Pílulas brilhantes para contagens, planos, atalhos ou status → texto mono discreto ou keycap
- Selos `PRO`, `Novo ✨`, `Beta 🚀` por todo lado → remover, ou um selo de texto discreto
- Tudo em formato pílula, da busca aos botões e cards → raio por tamanho, raio aninhado
- Gráficos com barras arco-íris, brilhando, arredondadas como pílula ou dias em caixa alta → uma ou duas séries, grade apagada, rótulos mono, uma cor de destaque
- Todo gráfico em vários tons do destaque, nada lidera → degraus neutros e destaque só no que importa
- Sparklines e mini-barras em todo card de estatística → o número, o rótulo e a variação
- Cards iguais lado a lado, cada um com o mesmo gráfico → um gráfico principal, estatísticas compactas, larguras variadas
- Logo como quadrado com gradiente e brilhinho, com nome em gradiente → nome do produto em texto mais uma marca plana
- Logo como orbe brilhante ou bolinha com glow → símbolo plano numa cor sólida, ou só o nome

## Landing pages e heros

- Pílula acima do título (`✨ Apresentando X 2.0`) → remover, ou link de texto discreto se for novidade real
- Título que serve para qualquer produto (`Potencialize seu negócio com IA`) → dizer o que o produto faz e para quem
- Gradiente ou shimmer no título → texto sólido
- Blobs, orbes, grades e linhas brilhando atrás do hero → fundo simples ou um visual real do produto
- Tudo empilhado e centralizado (título, texto, botões, imagem embaixo) → divisão assimétrica ou texto sobre prévia grande
- Três ou mais botões, ou chips e avatares empilhados sob os botões → uma ação principal e no máximo uma secundária
- `Mais de 10.000 empresas confiam`, fileira de avatares, cinco estrelas sem fonte → perguntar se é real; depois deixar discreto e específico, ou remover
- Parallax e elementos flutuando na rolagem → layout estático
- Cards de funcionalidade com emoji, título em negrito e frase vaga → menos itens, texto concreto, ícones de linha ou nenhum
- Botão flutuante de WhatsApp pulsando ou com glow → botão estático, discreto, na paleta

## Visuais

- Bolhas 3D brilhantes, orbes, cromado líquido ou nebulosa roxa como visual principal → o próprio produto ou uma metáfora concreta do que ele faz
- Robôs, cérebros brilhando, circuitos ou hologramas para qualquer coisa de IA → remover, ou mostrar o que a IA realmente entrega
- Texto, botões falsos ou logo embutidos na imagem → texto real na página, imagem limpa
- Imagem que não se funde à página (borda dura, preto diferente) → fundo casado com a página e máscara suave nas bordas
- Um visual em cada seção → um visual onde ajuda, geralmente só no hero

## Animação

- `animate-pulse`, `animate-ping` ou brilho respirando em coisas que não são "ao vivo" → estático
- `transition-all` e `hover:scale` em cards e botões → troca de cor/superfície no hover, leve redução no clique
- Molas saltitantes e overshoot em UI simples → uma curva ease-out
- Tudo voando na tela ao carregar, de direções diferentes → um fade + subida curta com leve escalonamento
- Animar width, height, top ou left → transform e opacity

## Cara de template

Não é vício de IA, mas é onde uma tela limpa cai quando ninguém decidiu nada. Fique atento depois das passadas.

- Página cinza puro #161616, Inter, texto branco e a cor antiga da marca num botão, num produto cujo mundo é quente ou luminoso → escala tingida para o mundo e destaque tirado dele
- Título que serviria para outro produto se trocasse o nome → dizer o que este produto faz, com os substantivos dele
- Visual do hero que é uma caixa vazia ou imagem genérica → prévia em código ou imagem do mundo
- Todo produto ganhando o mesmo layout, fonte e paleta → deixar a direção escolher

---

Baseado no unslop de Damir Sokolovsky ([@heydamir](https://x.com/heydamir)), CC BY 4.0.
