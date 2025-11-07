<img width="450" height="330" alt="image" src="https://github.com/user-attachments/assets/b0fa84d2-2728-45e0-a16a-1a52eba7d167" /># Processamento de Imagem Covid

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
  <p allign = center>
    <img width="500" height="372" alt="COVID" src="https://github.com/user-attachments/assets/13adebba-2087-4621-b7c5-7da7309db2da" />
  </p>

- Conversão para Escala de Cinza e Equalização de Histograma::

   <p allign = center>
    <img width="504" height="377" alt="image" src="https://github.com/user-attachments/assets/a5969e0f-eb37-45ef-b07f-9e8f15060297" />
  </p>

  


Prepara a imagem para técnicas que operam em um único canal de cor e aplica a equalização de histograma para aumentar o contraste da imagem, melhorando a visibilidade de detalhes nas áreas escuras e claras.

- Binarização de Otsu (Limiarização):
  <p allign = center>
    <img width="501" height="367" alt="image" src="https://github.com/user-attachments/assets/63c10361-e8c2-471c-ba29-67cbac2bda12" />>
  </p>
Calcula automaticamente um limiar para converter a imagem em escala de cinza em uma imagem binária (preto e branco), isolando regiões de interesse (por exemplo, as áreas pulmonares ou lesões).

-Gauss e Laplaciano
<p allign = center>
<img width="448" height="327" alt="image" src="https://github.com/user-attachments/assets/192f1788-984a-410c-9d57-e9c04e6896c5" />

<img width="446" height="334" alt="image" src="https://github.com/user-attachments/assets/c40c3232-e758-4d4b-a1fa-8275158f8365" />

</p>

- Erosão:

  <p allign = center>
    <img width="450" height="332" alt="image" src="https://github.com/user-attachments/assets/1eeb613e-0d2a-46cb-ad75-0e9fb700463c" />
    <img width="454" height="336" alt="image" src="https://github.com/user-attachments/assets/7afc1af0-8c08-49b4-ab22-58e93300d4e7" />
    <img width="450" height="330" alt="image" src="https://github.com/user-attachments/assets/8daedff3-bd7a-4706-afc8-fb6107a3017c" />

  </p>
  
- Operações Morfológicas:
 <p allign = center>
  <img width="374" height="559" alt="image" src="https://github.com/user-attachments/assets/4f7cb650-831c-401f-be65-73f97d0fd13d" />
  <img width="445" height="329" alt="image" src="https://github.com/user-attachments/assets/80cbdda7-7089-4a35-8016-4c8727211ee2" />
  <img width="447" height="331" alt="image" src="https://github.com/user-attachments/assets/13c169a0-199b-4050-8ba7-010e1e7d2ef1" />
  </p>


Utiliza um kernel 3x3 para aplicar transformações morfológicas focando em Dilatação, Erosão, Abertura ou Fechamento para remover ruído, preencher lacunas ou suavizar contornos.
