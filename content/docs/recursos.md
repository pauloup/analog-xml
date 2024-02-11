+++
weight = 3
+++

## Recursos
- [4 Lentes](#4%20Lentes)
- [64MP](#64MP)
- [Granulado natural](#Granulado%20natural)
- [Cor natural](#Cor%20natural)
- [Luz natural](#Luz%20natural)
- [Vídeo](#Vídeo)
- [Visão Noturna](#Visão%20Noturna)
- [Retrato](#Retrato)
- [Preto e Branco](#Preto%20e%20Branco)
- [Qualidade Máxima](#Qualidade%20Máxima)
- [HDR+](#HDR+)
- [RAW](#RAW)
- [Melhor Foto](#Melhor%20Foto)
- [Luz real](#Luz%20real)
- [Vinheta real](#Vinheta%20real)
- [Panorama](#Panorama)
- [Photo Sphere](#Photo%20Sphere)
- [Google Lens](#Google%20Lens)
### 4 Lentes
Todas as lentes configuradas: Lente Principal, Ultra Angular, Macro e Frontal.
[Imagem comparando fotos das 4 lentes]
JPG: Principal, Ultra Angular, Macro, Frontal.

As 4 lentes foram otimizadas para entregar um resultado similar e o mais consistente possível.

Algumas situações podem apresentar diferenças nas lentes. Veja [Limitações: Lentes inconsistentes](#Lentes%20inconsistentes).
### 64MP
Fotos com resolução em dobro, com 64MP na lente Principal, 32MP na Ultra Angular, 32MP na Macro e 20MP na Frontal.
Detalhes finos com nitidez e definição, aproveitando o máximo do sensor.
 
Salvar fotos com o dobro da resolução permite recuperar um nível alto de detalhes, com os algoritmos avançados de processamento da Google Camera, e ter o máximo da qualidade.

O algoritmo de Super Res Zoom (Sabre) combina várias fotos para gerar uma só, com o dobro do tamanho e mais nitidez do que só aumentar a imagem na edição.

#### 64MP reais ou interpolados
O sensor da lente Principal tem 64MP reais (9248 x 6944 pixels), mas a POCO só permite essa resolução no app da câmera nativa, e limita as fotos em 16MP (4624 x 3472 pixels) para apps de terceiros, como a Google Camera.

A tecnologia que reduz a foto de 64MP para 16MP é chamada de [Pixel Binning](#Pixel%20Binning), e combina cada grupo de 4 pixels para formar 1 pixel.

Isso reduz o ruído digital e melhora a capitação de luz em cenas escuras, mas a resolução da foto cai pela metade*, e há menos detalhes.

*\*Nota: Por convenção, se diz que a resolução da foto cai pela metade quando largura e altura são ambas reduzidas pela metade. Assim, o total de pixels da foto, que é o número de MegaPixels, cai para 1/4. Por isso, 16MP é "metade da resolução" de 64MP, mesmo sendo 1/4 do valor numérico.*

Para superar essa limitação, Analog usa os recursos de Upscaling ([Raisr](#Raisr)) e Super Res Zoom ([Sabre](#Sabre)) da Google Camera.

Isso aumenta as fotos de 16MP com binning disponíveis para fotos de 64MP interpolados, com qualidade comparável ou ainda superior aos 64MP reais da câmera nativa.

[Comparação de uma foto com 64MP reais da câmera nativa, e uma com 64MP interpolados da Google Camera.]

*JPG: Nativa 64MP reais vs Google Camera 64MP interpolados*.

Aliás, os 64MP da câmera nativa nem sempre são reais. Em situações mais escuras, a câmera nativa também usa os 16MP com pixel binning, e aumenta a imagem pra 64MP, com bem menos qualidade que a Google Camera.

[Comparação de uma foto com 64MP interpolados da câmera nativa, e uma com 64MP interpolados da Google Camera]

*JPG: Nativa 64MP interpolados vs Google Camera 64MP interpolados*.

O mesmo processo é usado nas outras lentes para dobrar a resolução e produzir fotos com mais qualidade que na câmera nativa.

[Imagem das outras 3 lentes com o dobro de resolução em comparação com a câmera nativa.]

Opcional: Esse recurso é ligado por padrão. Desative a opção Alta Resolução (HIRES) para desligar esse recurso e tirar fotos na resolução padrão de 16MP na lente Principal, 8MP na Ultra Angular, 2MP na Macro e 5MP na Frontal.

[Imagem da opção HIRES desativada]
### Granulado natural
Granulado de filme, como numa câmera analógica, preservando o ruído natural da foto.

O uso exagerado de Remoção de Ruído destrói os detalhes finos da imagem, deixando o visual artificial e digital, comum das fotos de celular.

A Google Camera nasceu da ideia de combinar várias fotos para reduzir ruído de forma natural, a mesma tecnologia usada pela NASA pra fotografar o espaço profundo. Assim, não é preciso usar algoritmos de remoção de ruído.

Graças à combinação de quadros do HDR+ Melhorado, o ruído que fica na imagem é orgânico e não apresenta a característica artificial do sensor digital. E em situações com pouca luz, o ruído faz parte da realidade.

Analog foi criado com a intenção de preservar detalhes e granulado. O granulado real é uma das características fundamentais que permite capturar o máximo de nitidez na fotografia. 

Assim como uma fotografia analógica tirada em câmera de filme, a foto do Analog é orgânica e com textura, ruído, marcas da tecnologia utilizada e, principalmente, sentimento.

Porém, pode ser útil ter um mínimo de remoção de ruído, e por isso há um XML variação chamado Analog-Smooth que abre mão do granulado e usa remoção de ruído, mas tentando preservar todas as outras características do Analog.

Opcional: Esse recurso é ligado por padrão. Desative a opção Library Patch (LIBP) para desligar esse recurso e usar a remoção de ruído padrão da Google Camera. Outras características do Analog também serão desativadas, como as cores fortes.

[Imagem da opção HIRES desativada]
### Cor natural
Comparar balanço de branco frio (celular, digital) e quente (camera, analógico)

#### Redução do ruído verde
O AWB do Pixel 4 tem menos intensidade no canal verde, o que ajuda a reduzir o ruído verde, um problema comum em Astrofotografia.

[Comparação de uma foto com AWB 19.Sony IMX686, com tom médio mais verde, e outra com AWB 4.Google Pixel 4, mais neutra. ]

Como o HDR+ Melhorado combina várias quadros subexpostos, as fotos acabam o com o mesmo problema da Astrofotografia.

Exposições escuras, com pouca luz, ficam com mais ruído nos canais vermelho e azul, e o canal verde se destaca, deixando o ruído verde.

[Comparação de um detalhe com zoom nos pixels das sombras de uma foto, com os canais RGB separados e sua combinação. Os canais vermelho e verde tem mais ruído, enquanto o verde é mais uniforme. O resultado é uma combinação com um tom verde sutil.]

Esse problema não é solucionado com a redução de ruído de cor, porque ela não corrige a diferença de luminosidade média nos canais.

O balanço de branco automático pode ajudar a reduzir o canal verde, equilibrar o tom e deixar a imagem com mais qualidade aparente.
#### Saturação subtrativa
Menos saturação RGB e mais saturação HSV
### Luz natural
Visual flat vs alto contraste 
#### Sombras preservadas

### Vídeo
Estabilização, câmera lenta e 4K 60fps

Estabilização corta as bordas e dá um zoom na imagem.

Pra desligar a estabilização, precisa mudar a  [Stream Video mode](#Stream%20Video%20mode).

Ultra Angular grava em 4K
Macro não grava vídeo

Frontal: 24fps, 30fps e 60fps com estabilização

Não funciona no vídeo, pq a imagem não é processada pela Google Camera:
- Exposição manual
- AWB
- HIRES
- LIBP
- LDR

Funciona no vídeo:
- Ajuste de exposição com toque na tela
- SHAD
- Foco manual
- Melhoria de fala na Frontal, no espectrograma dá pra ver um ganho de 1000 a 2000kHz
### Visão Noturna
Recupera luzes e sombras
Modo Astro demora muito mesmo, parece q travou 
### Retrato
Detecção de rosto ativa, com sugestão de modo retrato
### Preto e Branco
Filtro [ortocromático](https://thedarkroom.com/orthochromatic-vs-panchromatic-film-a-photo-comparison/) que escurece tons vermelhos e dá intensidade à foto, como o [usado no filme O Farol (2019)](https://analogcameraclub.com.br/analog-recomenda-o-farol-the-lightouse-2019).

Dica: ativar a opção [RAW](#RAW) pra salvar a foto original em cores.

Para usar esse recurso em outras lentes, veja [Alternativas: Analog-BW](#Analog-BW).

Não funciona no Vídeo, Panorama e Photo Sphere
### Qualidade Máxima
Por padrão, as fotos tem um número de quadros automático... Mas
### HDR+ Melhorado
Em cenas com luz extremamente baixa, o HDR+ Melhorado pode criar fotos mais escuras que o HDR+ Ativado. Veja [HDR+ melhor que o HDR+ Melhorado](#HDR+%20melhor%20que%20o%20HDR+%20Melhorado)

Faz parte do HDR+ Melhorado tirar várias fotos mais escuras e combinar elas em uma única foto, com menos ruído, que é clareada para a exposição correta no final.

Mas quando a luz da cena é tão baixa, essas fotos mais escuras não conseguem capturar luz suficiente, e mesmo depois de clareada, a foto ainda fica mais escura do que deveria.



### RAW
...

Diferentes tipos de RAW:
- Puro no HDR+
- Processado no HDR+ Melhorado.

: A opção RAW não está disponível no modo Retrato, mas há uma forma de salvar a foto original em DNG. Veja Dicas: Retrato com RAW
### Luz real
Desligar o HDR...
### Vinheta real
Modo Leica...

### Panorama
### Photo Sphere
Não tem processamento HDR
### Google Lens
Usar apk GoogleEn
