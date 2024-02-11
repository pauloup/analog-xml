+++
weight = 12
+++

## Extras
Recursos que não fazem parte de Analog, mas podem ser ativados manualmente nas configurações.
### Compensação de Exposição
Se as fotos em geral ficam mais escuras, ou mais claras, do que você gostaria, o recurso de Compensação de Exposição pode ajudar.
#### Enable exposure compensation
- Valor: Ligada
- Caminho: Configurações > Configurações Adicionais > Compensação de Exposição

Essa opção ativa um aumento ou redução constante da exposição automática, e pode ser ajustado pra cada lente e modo.
#### Seleção da Compensação de Exposição
- Valor: 
	- Front lens (Frontal): +0,6
	- Main lens (Principal): +0,6
	- Tele lens (Macro): +0,6
	- Wide lens (Ultra Angular): +0,6
	- ID4 lens (Preto e Branco): +0,6
	- ID5 lens (Qualidade Máxima): +0,6
	- Night mode (Visão Noturna): +0,6
	- Portrait mode (Retrato): +0,6
 - Caminho: Configurações > Configurações Adicionais > Compensação de Exposição

O valor sugerido é de +0,6 pra deixar as fotos levemente mais claras.

Valores positivos clareiam a foto, mas tem maior chance de estourar as luzes para o branco. Podem deixar a foto mais lenta e com desfoque de movimento pelo maior tempo de exposição, ou aumentar o ruído pelo ISO maior.

Valores negativos escurecem a foto, mas preservam mais detalhes nas luzes, mas podem introduzir o problema de sombras esverdeadas, ou reduzir a qualidade geral da foto pelo ISO menor ou tempo de exposição mais curto.

Esse ajuste é aplicado a todas as fotos, mas ainda é possível ajustar a compensação de exposição a cada foto com o [Ajuste de exposição na tela](#Ajuste%20de%20exposição%20na%20tela), ou a [Exposição manual](#Exposição%20manual).
### RAW no Retrato

gouda.raw
- Valor: Ligada
- Caminho: Configurações > Developer Settings > camera.gouda.raw

Salva a foto original em RAW no modo Retrato.

A imagem é salva no formato PPM, com nome "rgb_in.ppm", numa nova pasta dentro de SGCAM/XML/portrait. Dados EXIF, como data e exposição, não são salvos na imagem.

primary_raw
- Valor: Ligada
- Caminho: Configurações > Developer Settings > camera.gouda.primary_raw

Salva a foto original em RAW no modo Retrato.

A imagem é salva no formato DNG, com nome "primary.dng", numa nova pasta dentro de SGCAM/XML/portrait. Dados EXIF, como data e exposição, não são salvos na imagem.

Requer [gouda.raw](#gouda.raw) ligada.

allow_raw_blur_rear
- Valor: Ligada
- Caminho: Configurações > Developer Settings > camera.gouda.allow_raw_blur_rear
- Ativa o RAW no Retrato para as lentes Principal, Ultra Angular e Macro.

Requer [gouda.raw](#gouda.raw) ligada.

allow_raw_blur_front
- Valor: Ligada
- Caminho: Configurações > Developer Settings > camera.gouda.allow_raw_blur_front
- Ativa o RAW no Retrato para a lentes Frontal.
- Requer gouda.raw ligada.
- Bug: O fundo desfocado fica superexposto.
### Melhor Foto
O recurso Melhor Foto grava um vídeo junto ao se tirar uma foto no modo HDR+ Ativado, e permite extrair outras fotos dele.

[Imagem da interface com a opção Top Shot Ativada no menu superior aberto.]

A partir desse vídeo, a Google Camera seleciona quadros que dariam boas fotos e processa com o HDR+ Ativado.

O vídeo fica salvo "dentro" da foto e só pode ser assistido ao abrir a foto no Google Fotos, onde é possível extrair os quadros processados.

[Imagem da interface do Google Photos, com o vídeo tocando ao abrir a foto, e a lista de quadros nos detalhes da foto.]

Com a opção Motion Photo ativada no Google Fotos, nos detalhes da foto são mostrados quadros selecionados pela Google Camera como "os melhores".

[Imagem]

É possível exportar esses quadros com maior resolução (4K 4:3 com 2160 x 2880 pixels) e um efeito de HDR.

Ele funciona só no modo HDR+ Ativado. É possível gravar um vídeo de Melhor Foto no HDR+ Melhorado segurando o obturador.
#### enable_micro
- Valor: Ligada
- Caminho: Configurações > Developer Settings > camera.enable_micro

Ativa o Melhor Foto.

Às vezes, o Google Fotos não mostra a seleção de quadros nos detalhes da foto. Nesse caso, toque em Editar e na seção Motion para acessar.
#### mts_fast_hdr
- Valor: Desligada
- Caminho: Configurações > Developer Settings > camera.mts_fast_hdr

Salva quadros mais rápido, mas com menos qualidade, e por isso fica desligada.

Motion photo


### Video 8K
Precisa desativar estabilização e mudar stream 

Se a tela ficar preta, trocar para o modo Camera e voltar ao modo Vídeo.

O vídeo vai aparecer distorcido e com a proporção errada na tela, mas será salvo corretamente.

Somente 30fps.
#### Estabilização
- Valor: Desligada
- Caminho: Configurações > Additional Settings > Stream Config > Main cam > Video mode
#### Stream Video mode
- Valor: 262144 - OpMode (Default)
- Caminho: Configurações > Additional Settings > Stream Config > Main cam > Video mode

Também funciona com Stream 32797 - Video EIS 8K
### Video 4:3 Full Sensor
Para gravar vídeo na proporção 4:3, com a imagem do sensor inteira e sem corte, ligue a opção Resolução Manual nas Configurações.
#### Enable manual resolution 
Valor: Ligada
- Caminho: Configurações > Additional Settings > Video settings > Video resolution > Enable manual resolution
- Ativa a resolução manual de vídeo:
    - Front lens (Frontal): 3264 x 2448
    - Main lens (Principal): 3264 x 2448
    - Tele lens (Macro): 1200 x 1600
    - Wide lens (Ultra Angular): 3264 x 2448
    - ID4 lens (Preto e Branco): 3264 x 2448
    - ID5 lens (Qualidade Máxima): 3264 x 2448

A resolução de 3264 x 2448 é a mais próxima do 4K 4:3 (3840 x 2440) que está disponível e grava sem dificuldades, como perda de frames. Veja todas as resoluções disponíveis para gravação de vídeo em [Especificações](#Especificações).

A lente Macro só faz vídeo com essa opção ligada, já que a resolução máxima do sensor de 1200 x 1600 é menor que a opção Full HD de 1920 x 1080, padrão mínimo da Google Camera.

A lente Frontal parece não ter implementado estabilização de vídeo na proporção 4:3, então é preciso desativar a estabilização:
- Caminho: Configurações > Additional Settings > Stream config > Front cam > Video mode: 0 - default. 
### Balanço de branco manual
Para ativar o balanço de branco manual:
- Ativar a configuração White Balance
- Desligar a opção AWB
- Tocar na imagem na tela para ajustar o balanço de branco

Problema: Há um grande atraso no disparo da foto quando esse recurso está ativo.
#### Configuração White Balance
- Valor: Ligada
- Caminho: Configurações > White Balance

#### Opção AWB
- Valor: Desligada
- Caminho: Botão AWB

### Flash de Preenchimento Sintético
O recurso de Flash de Preenchimento Sintético (Synthetic Fill Flash) projeta uma luz artificial que destaca pessoas em fotos tiradas no modo Retrato. Esse efeito de luz suaviza sombras e clareia o rosto e o corpo das pessoas.

[Imagem comparando uma foto sem e outra com o Flash de Preenchimento Sintético]

Ele não é usado em Analog porque modifica muito a realidade da foto, mas tem qualidade suficiente pra servir como recurso criativo.

O efeito pode ser forte ou sutil, e não há como controlar sua intensidade. A Google Camera decide quando e como aplica-lo.

É possível ver a foto ainda sem o efeito por um breve momento depois do disparo, tocando na miniatura da galeria para ver a foto temporária exibida enquanto a foto é processada.

[Imagem comparando a foto temporária exibida antes da foto ser processada, sem o efeito de Flash de Preenchimento Sintético, e depois de processada, já com o efeito]

Nas configurações de desenvolvedor existem várias opções relacionadas a esse recurso com as palavras "acat", "firefly" e "spotlight". Em Analog, é suficiente ligar a opção a seguir.
#### gouda.firefly_enabled
- Valor: Ligada
- Caminho: Configurações > Developer Settings > camera.gouda.firefly_enabled
