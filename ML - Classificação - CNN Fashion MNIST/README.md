# Fashion MNIST - Explorando a Classificação de Imagens com CNNs

> Este artigo explora a aplicação de redes neurais convolucionais (CNNs) para a classificação do conjunto de dados Fashion MNIST, demonstrando o processo desde o pré-processamento até a avaliação do modelo.

</br> <div align="center"> <img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fgoodboychan.github.io%2Fimages%2FFashionMNIST.png&f=1&nofb=1&ipt=3e86c27d4e5aa73680c7e935ccb11f4474d954e3300be817d6cf1434ec9c5428&ipo=images" width="300"> </div>

## Introdução

Este artigo apresenta uma abordagem prática para a classificação de imagens de roupas utilizando o dataset Fashion MNIST. O objetivo é demonstrar como redes neurais convolucionais (CNNs) podem ser aplicadas para resolver problemas de visão computacional, destacando os passos necessários desde o carregamento dos dados até a avaliação do modelo.

## Sobre o Fashion MNIST

O Fashion MNIST é um conjunto de dados composto por 70.000 imagens de roupas em escala de cinza, divididas em 10 categorias. Cada imagem possui 28x28 pixels. Este dataset é uma alternativa mais desafiadora ao clássico MNIST, que contém dígitos manuscritos.

**Link para o dataset:**

- [TensorFlow Datasets](https://www.tensorflow.org/datasets/catalog/fashion_mnist?hl=pt-br)
- [GitHub - Zalando Research](https://github.com/zalandoresearch/fashion-mnist)

## Objetivos e Metodologia

### Objetivos

- **Desenvolver um modelo CNN:** Construir uma rede neural convolucional capaz de classificar as imagens do Fashion MNIST com alta precisão.
- **Avaliar o desempenho do modelo:** Utilizar métricas de avaliação como acurácia, F1 score e relatório de classificação para medir o desempenho do modelo.

### Metodologia

- **Carregar e explorar os dados:** Analisar a distribuição das classes e as características dos dados.
- **Pré-processar os dados:** Normalizar os valores dos pixels e preparar os dados para o treinamento.
- **Construir e compilar o modelo:** Definir a arquitetura da CNN e compilar o modelo.
- **Treinar o modelo:** Ajustar os pesos do modelo utilizando o conjunto de treinamento.
- **Avaliar o modelo:** Medir o desempenho do modelo nos conjuntos de teste e validação.

## Pré-processamento dos Dados

O primeiro passo é carregar os dados e realizar uma análise exploratória para entender a distribuição das classes e as características dos dados. Em seguida, normalizamos os valores dos pixels para o intervalo [0, 1] e adicionamos uma dimensão para os canais de cor (escala de cinza).

## Construção e Treinamento do Modelo

Construímos uma CNN com camadas de convolução, pooling e densas, e compilamos o modelo usando o otimizador Adam e a função de perda sparse_categorical_crossentropy. O modelo é então treinado por 5 épocas.

## Avaliação do Modelo

Avaliar o modelo nos conjuntos de teste e validação é crucial para medir seu desempenho. Utilizamos métricas como acurácia e F1 score para uma avaliação detalhada.

## Link para o projeto

<a href="https://github.com/rafarodrigues/visao-computacional/blob/main/ML%20-%20Classifica%C3%A7%C3%A3o%20-%20CNN%20Fashion%20MNIST/Fashion_MNIST.ipynb" target="_blank">visao-computacional/ML - Classificação - CNN Fashion MNIST
/Fashion_MNIST.ipynb</a>

## Conclusão

Através deste estudo, demonstramos a aplicação prática de uma CNN para a classificação de imagens do Fashion MNIST, abordando todas as etapas necessárias desde o pré-processamento até a avaliação do modelo. Os resultados obtidos destacam a eficácia das redes neurais convolucionais em tarefas de visão computacional.

## Referências

- [TensorFlow Datasets](https://www.tensorflow.org/datasets/catalog/fashion_mnist?hl=pt-br)
- [GitHub - Zalando Research](https://github.com/zalandoresearch/fashion-mnist)