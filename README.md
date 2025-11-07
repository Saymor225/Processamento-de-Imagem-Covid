# Processamento de Imagem Covid

Este projeto utiliza a biblioteca OpenCV para aplicar diversas técnicas de processamento de imagens em do virús da covid, visando aprimorar a visualização e preparar as imagens para análises posteriores, como detecção ou segmentação de padrões relacionados a condições pulmonares (como as associadas ao COVID-19).

O código está implementado em um Google Collab (Covid.ipynb).

🛠️ Tecnologias Utilizadas
Python

- OpenCV (cv2): Para manipulação e processamento de imagens.

- NumPy (numpy): Para operações com arrays (estruturas de imagem).

- Matplotlib (matplotlib): Para visualização e plotagem (embora o notebook use principalmente cv2_imshow).

⚙️ Funcionalidades Implementadas
O notebook realiza uma série de transformações na imagem de entrada (COVID.png):

- Leitura e Visualização da Imagem Original:

- Conversão para Escala de Cinza:

Prepara a imagem para técnicas que operam em um único canal de cor.

- Equalização de Histograma:

Aplica a equalização de histograma para aumentar o contraste da imagem, melhorando a visibilidade de detalhes nas áreas escuras e claras.

- Binarização de Otsu (Limiarização):

Calcula automaticamente um limiar para converter a imagem em escala de cinza em uma imagem binária (preto e branco), isolando regiões de interesse (por exemplo, as áreas pulmonares ou lesões).

- Operações Morfológicas:

Utiliza um kernel 3x3 para aplicar transformações morfológicas, provavelmente focando em Dilatação, Erosão, Abertura ou Fechamento para remover ruído, preencher lacunas ou suavizar contornos.
