# Visuais

Como trocar enfeite genérico por um visual que pertence a este produto, e como gerar um quando houver ferramenta de imagem.

## Decida o que é o visual

1. **A tela precisa de um?** Dashboards, configurações e a maioria das telas de app, não. Heros de landing e estados vazios, geralmente sim.
2. **Existe ferramenta de imagem?** Para hero de landing, gere uma cena do mundo como fundo do hero inteiro, assunto num lado e espaço calmo para o título no outro. Depois mostre o produto subindo da borda inferior.
3. **Mostre o produto.** Abaixo da cena, ou como visual quando não há ferramenta, construa em código uma prévia do que a página já promete. Escolha o único momento que prova o título, não o app inteiro: uma agenda mostra uma semana com um horário marcado; um app de hábitos mostra a sequência num card; um delivery mostra um pedido a caminho com a rota. Use os componentes do projeto se existirem, senão HTML cuidadoso na paleta nova, com dados plausíveis e nomes reais.
4. **Escreva a cena numa frase.** Use o mundo e a personalidade da direção. Se não cabe numa frase, ainda não está claro.

Exemplos só do formato (não reutilize, derive do produto):

- Ferramenta de backup → um pequeno farol num litoral rochoso escuro, o facho atravessando a neblina
- App de meditação → uma xícara de chá soltando vapor no parapeito, com a primeira luz da manhã
- API de logística → um navio de contêineres visto de cima, num mar cinza e calmo
- App de idiomas → uma pilha de fichas escritas à mão numa mesa de café, com sol da tarde

Evite os padrões de IA, a menos que o produto seja literalmente sobre eles: bolhas brilhantes, orbes, nebulosas, cromado líquido, cubos flutuando, circuitos neon, hologramas, cérebros brilhando, robôs, foguetes, cristais.

## Estilos que funcionam

Escolha um que combine com a personalidade e mantenha na página toda.

- **Pintura de cenário.** Céu ou paisagem calma com um assunto, como os fundos de animações japonesas modernas: nuvens nítidas, luz suave, céu aberto para o texto. Bom para produtos calorosos e humanos.
- **Foto cinematográfica de um objeto.** Uma coisa real em luz dramática simples sobre fundo liso. Bom para produtos sérios e confiáveis.
- **3D estilizado suave.** Uma cena pequena com materiais foscos e luz gentil. Bom para produtos brincalhões.
- **Render de objeto do produto.** Cartão, celular, embalagem, iluminados em estúdio com materiais reais, usados como momento dentro da interface.
- **Luz e óptica.** Um fenômeno físico em fundo escuro, como luz se dividindo num prisma. Bom para produtos técnicos ou de dados.
- **Gravura ou xilogravura.** Monocromática numa tinta só sobre papel levemente tingido — funciona quando a marca inteira vive nesse estilo (combina muito com produtos de herança, artesanato ou com pegada de cordel/nordeste, se for o caso).

O que costuma falhar:

- Pedir granulado, textura de papel ou ruído no prompt — os modelos assam um padrão xadrez na imagem. Adicione textura em código.
- Um estilo de gravura numa imagem só enquanto o resto é interface moderna lisa — parece filtro.
- Vários assuntos ou colagem cheia.
- Qualquer abstração roxa e azul brilhante.

## Objetos para momentos

- Peça um objeto, iluminado em estúdio, sobre fundo liso na cor exata da página, com sombra de contato suave.
- Peça o ângulo que o layout precisa ("inclinado 20 graus, visto levemente de cima").
- Recorte o fundo se a ferramenta permitir; senão, funda com máscara na cor da página.
- Posicione sobrepondo a borda de um card, levemente rotacionado, com sombra suave na cor mais escura da escala.
- Tudo dentro de um visual conta a mesma história: se a lista mostra o pedido #0142 da cliente Mariana, o celular mostra a mesma cliente, número e valor.

## Gerar a imagem

Procure uma ferramenta de geração entre as disponíveis (MCP de fal, Replicate, OpenAI images, Higgsfield, ferramenta de design etc.). Se houver:

- Mostre ao usuário o prompt, o modelo e o tamanho, e pergunte antes de rodar, porque pode custar dinheiro.
- Rode uma vez. Julgue contra a frase e a paleta antes de tentar de novo; mude o prompt em vez de repetir o mesmo.
- Salve o resultado nos assets do projeto, não numa URL temporária.

Se não houver ferramenta e a tela precisar de cena ou objeto, diga isso antes da passada de Visuais e ofereça conectar uma. Se o usuário pular, deixe o espaço vazio (superfície lisa do tamanho exato, com o raio do layout e sem texto dentro) e coloque o prompt no relatório, não na página.

## Receita de prompt

Monte nesta ordem (prompts em inglês costumam render melhor nos geradores):

- **Assunto.** A frase, concreta e física.
- **Cenário.** Onde está, simples.
- **Luz e paleta.** Casadas com a página. Diga a cor de fundo da página para as bordas fundirem, e a direção da luz.
- **Estilo.** Uma direção clara que combine com a personalidade.
- **Composição.** Onde fica o assunto para o texto ter espaço ("subject on the right half, calm empty space on the left"). Para cena atrás do hero inteiro, peça 16:9 ou mais largo e mantenha o quinto inferior calmo.
- **Exclusões.** No text, no letters, no logos, no UI, no watermark.
- **Formato.** Proporção do espaço, no dobro do tamanho de exibição.

## Colocar na página

- Exporte em WebP ou AVIF no dobro do tamanho de exibição, com `alt` real dizendo o que aparece.
- Case as bordas da imagem com o fundo da página. Se não casarem, use máscara (`mask-image: radial-gradient(closest-side, #000 70%, transparent)`) ou um degradê na cor da página. Retângulo duro sobre página de outra cor é vício.
- Estática, ou com um movimento lento e sutil que combine com o assunto. Sem parallax.
- Carregue a imagem do hero com prioridade alta e dimensões fixas para o layout não pular.

---

Baseado no unslop de Damir Sokolovsky ([@heydamir](https://x.com/heydamir)), CC BY 4.0.
