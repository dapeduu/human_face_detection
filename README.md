# Algoritmo de reconhecimento de faces

O projeto é uma implementação do algoritmo do artigo: [The Human Face Recognition Algorithm Based on the Improved Binary Morphology](https://ieeexplore.ieee.org/document/8469732) por [Juan Wan](https://ieeexplore.ieee.org/author/37086461467) e [Ya Wang](https://ieeexplore.ieee.org/author/37086461687).

A ideia é realizar um processamento nas imagens de forma a extrair somente os rostos e facilitar o trabalho dos sistemas de detecção.

# Passo a passo

1. Equalização de Histograma
  - https://docs.opencv.org/4.x/d5/daf/tutorial_py_histogram_equalization.html
2. Normalização
  - Filtro passa-baixas no domínio da frequência com auxilio da transformada de fourier
  - https://www.youtube.com/watch?v=YVBxM64kpkU
3. Detecção de cor da pele, modelo YCrCb
4. Detecção de cor da pele, modelo HSV
5. Binarizar a imagem resultante
6. Reduzir ruído
