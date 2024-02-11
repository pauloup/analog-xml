+++
weight = 10
+++

## Tecnologias
### AWB
O recurso AWB significa Balanço de Branco Automático (Automatic White Balance), e equilibra as cores na foto.

[Imagem comparando 3 versões da mesma foto de uma paisagem de montanhas verdes com céu nublado: A 1ª foto com balanço de branco frio, onde o céu fica azulado, a 2ª com balanço de branco neutro e céu cinza, e a 3ª com balanço de branco quente e céu amarelado. Um pequeno gráfico indica a níveis dos canais de cor vermelho, verde e azul em cada foto, a 1ª com mais azul, a 2ª com todos iguais, e a 3ª com mais vermelho.]

Ele ajusta a intensidade dos canais de cor vermelho, verde e azul que formam a imagem, de acordo com a luz ambiente na cena.

Esse ajuste tenta deixar a cor branca o mais neutra o possível, o que ajuda na percepção e representação correta das outras cores.
#### Nossa visão
Na realidade, toda luz visível tem cor. Até a luz branca do sol é formada pela combinação de várias cores de luz diferentes.

[Foto de um raio de luz branca do sol passando por um prisma, que decompõe a luz branca, que passa por ele, em uma faixa de arco-íris com várias cores, do vermelho ao azul.]

Nossa visão percebe a luz do sol como branca, mas a atmosfera filtra e modifica a luz do sol ao longo do dia, o que altera sua cor.

De manhã e no poente, o sol próximo ao horizonte fica mais vermelho e cria cores quentes no céu, que vão do rosa ao laranja.

Ao longo do dia, o sol se eleva e o céu filtra menos sua luz. A luz branca do sol e o azul do céu lançam uma cor mais fria no ambiente.

[Imagem comparando uma foto de uma paisagem ao meio dia]

Nosso cérebro precisa reajustar a referência do que é o branco, para compensar essa variação na cor da luz ambiente ao longo do dia.

Por isso, vemos uma blusa branca na luz azulada do meio dia, ou na luz avermelhada do pôr do sol, e ainda sabemos que ela é branca.

Isso é o nosso Balanço de Branco. Nossa mente equilibra a intensidade das cores vermelha, verde e azul, percebidas pelos cones nos olhos.

Nem sempre o nosso balanço de branco concorda com o de outras pessoas, como mostrou o famoso [vestido branco e dourado](https://g1.globo.com/tecnologia/noticia/2015/02/azul-e-preto-ou-branco-e-dourado-vestido-polemico-quebra-internet.html).

[Imagem de um meme do vestido branco e dourado ou preto e azul, que dividiu opiniões em 2015]
#### AWB nas câmeras
Toda câmera digital possui o recurso de Balanço de Branco Automático (AWB), que faz a mesma coisa que a nossa visão.

Esse recurso observa a imagem captada pelo sensor, identifica possíveis áreas brancas e ajusta os canais de cor pra deixa-las neutras.

[Imagem comparando uma foto antes do Balanço de Branco, com uma luz verde intensa cobrindo toda a imagem, e a mesma foto depois do Balanço de Branco, com cores mais corretas e o branco neutro]

O Balanço de Branco Automático depende das cores captadas pelo sensor, e é muito sensível ao modelo do sensor e ao conteúdo da cena.

Cada modelo de sensor precisa de ajustes específicos de Balanço de Branco Automático para representar as cores com precisão.

O POCO F4 GT possui 4 lentes, com sensores da Sony, Omnivision e GalaxyCore. Por isso, as [lentes podem apresentar cores diferentes](#Lentes%20inconsistentes).
#### Dificuldade no AWB 
Cenas com objetos de cores fortes ocupando uma grande área da foto podem confundir o 
Balanço de Branco Automático.

O Balanço de Branco Automático usa áreas brancas como referência, então adicionar objetos brancos na cena pode ajudar.

[Imagem comparando uma foto de uma blusa vermelha bem próxima, que ocupa quase toda a foto e confunde o AWB, deixando o vermelho apagado e esverdeado, e outra foto da mesma blusa, mas com uma parede branca aparecendo ao fundo, o que ajuda o AWB e deixa a blusa no tom de vermelho correto.]
#### AWB do Sistema
O Balanço de Branco Automático do sistema, o mesmo usado na câmera nativa, é usado quando a [opção AWB](#Opção%20AWB) está desativada.

Ele costuma equilibrar bem as cores, especialmente em cenas na sombra, mas pode deixar cores muito saturadas em cenas ao sol.

![](images/source/balanco-de-branco-automatico-do-sistema-na-sombra-no-sol.svg)
[Imagem comparando fotos da câmera nativa usando o Balanço de Branco do sistema, uma com uma pessoa na sombra, dentro de casa, e cores corretas, e outra com a mesma pessoa no sol, com a pele amarelada e saturada.]

#### AWB da Google Camera
A Google Camera permite escolher um Balanço de Branco Automático diferente, que é usado quando a [opção AWB](#Opção%20AWB) está ativada.



Outro recurso aplicado antes do Balanço de Branco é o [CCT](#CCT), que ajusta a influência de um canal no outro para melhorar as cores.


### CCT
A Temperatura de Cor Correlacionada, ou Correlated Color Temperature (CCT) é o recurso converte o sinal do sensor em cores RGB.

O sensor captura 3 canais de cor, vermelho, verde e azul, mas geralmente existe uma sobreposição de sensibilidade entre eles.

[Gráfico da sensibilidade dos canais, verde e azul se sobrepondo]

Assim, o canal verde acaba capturando um pouco de luz vermelha e de luz verde. Essa sobreposição
A sensibilidade de cada canal de cor às frequências de luz, ou cores

https://stella.com.br/blog/temperaturas-de-cor-e-as-percepcoes-humanas
### Pixel Binning
[Pixel Binning](https://techlongreads.com/photography/pixel-binning-for-dummies/)
### Sabre
[Super Res Zoom](https://blog.research.google/2018/10/see-better-and-further-with-super-res.html?m=1) (Sabre)
### Raisr
Upscaling ([Rairs2020](https://blog.research.google/2016/11/enhance-raisr-sharp-images-with-machine.html)) 

The Challenges of Digital Zoom
Digital zoom is tough because a good algorithm is expected to start with a lower resolution image and "reconstruct" missing details reliably — with typical digital zoom a small crop of a single image is scaled up to produce a much larger image. Traditionally, this is done by linear interpolation methods, which attempt to recreate information that is not available in the original image, but introduce a blurry- or “plasticy” look that lacks texture and details. In contrast, most modern single-image upscalers use machine learning (including our own earlier work, RAISR). These magnify some specific image features such as straight edges and can even synthesize certain textures, but they cannot recover natural high-resolution details. While we still use RAISR to enhance the visual quality of images, most of the improved resolution provided by Super Res Zoom (at least for modest zoom factors like 2-3x) comes from our multi-frame approach.

https://blog.research.google/2018/10/see-better-and-further-with-super-res.html?m=1
