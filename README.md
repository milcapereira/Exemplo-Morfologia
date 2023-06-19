# Exemplo-Morfologia
O código utilizado para exemplo é escrito em Python utilizando a biblioteca OpenCV, que serve para realizar processamento de imagens, também é utilizado a biblioteca NumPy, para o uso de matrizes e a função “cv2_imshow” para exibição das imagens no google colab. O código consiste em uma série de operações morfológicas realizadas em uma imagem escolhida pelo programador. As bibliotecas são importadas na primeira parte do código.
Na segunda parte da estrutura do código, é carregada uma imagem de livre escolha usando a função "cv2.imread()" e armazenada na variável “img”. As variáveis “img_opening” e “img_closing” armazenam imagens com ruídos na parte externa e interna, respectivamente. As dimensões das imagens são armazenadas em variáveis através da função “.shape”.  Utilizando a função "np.ones()", é gerado uma matriz 5X5 preenchida com valores 1, onde será utilizado nas operações morfológicas como kernel. Com isso, o kernel é impresso usando a função "print()".
Na terceira parte da estrutura do código, as operações morfológicas são aplicadas à imagem "img" utilizando o kernel definido. É realizado a  erosão com a função "cv2.erode()" e a dilatação é realizada com a função "cv2.dilate()", os resultados são armazenados nas variáveis “erosion” e "dilation", respectivamente. Ambas as operações são realizadas duas vezes a partir da propriedade “iterations = 2”.
Na quarta parte da estrutura do código, são realizadas as operações mais complexas utilizando a função morphologyEx(), o gradiente detecta as bordas da imagem, a abertura remove os ruídos da parte externa da imagem e o fechamento  remove ruídos internos.
Na quinta parte da estrutura do código, as imagens resultantes das operações morfológicas são exibidas utilizando a função "cv2_imshow()", exclusiva do Colab. O trecho do código que roda em Python nativo está comentado.
