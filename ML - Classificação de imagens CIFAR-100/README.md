# CIFAR-100: Classificação de Imagens com Transfer Learning

> Este repositório apresenta a aplicação de técnicas de Transfer Learning para a classificação de imagens do dataset CIFAR-100. O trabalho inclui a correção e aprimoramento de um código inicial, com ênfase na criação de modelos eficientes e avaliação de seu desempenho.

<div align="center"> <img src="https://datarepository.wolframcloud.com/resources/images/69f/69f1e629-81e6-4eaa-998f-f6734fcd2cb3-io-4-o.en.gif" width="800"> </div>

## Introdução

A classificação de imagens é um problema central em visão computacional. Este repositório documenta a aplicação de Transfer Learning para classificar imagens do dataset CIFAR-100, abordando desde o carregamento e pré-processamento dos dados até a construção, treinamento e avaliação dos modelos. O trabalho também inclui a correção de um código inicial desenvolvido por um colega, que apresentava problemas na manipulação e estruturação dos dados.

## Sobre o CIFAR-100

O CIFAR-100 é um conjunto de dados composto por 60.000 imagens coloridas, distribuídas em 100 classes com 600 imagens cada. Cada imagem possui 32x32 pixels e as classes são agrupadas em 20 superclasses. Este dataset é mais complexo que o CIFAR-10 e é amplamente utilizado para testar algoritmos de classificação de imagens.

**Link para o dataset:**

- [CIFAR-100 Dataset](https://www.cs.toronto.edu/~kriz/cifar.html)

## Objetivos e Metodologia

### Objetivos

- **Corrigir a estrutura de dados:** Ajustar o código para lidar corretamente com a separação e pré-processamento dos dados.
- **Implementar Transfer Learning:** Utilizar modelos preexistentes, como EfficientNetB0 e MobileNetV2, para melhorar a precisão na classificação.
- **Avaliar o desempenho:** Medir a precisão e outras métricas relevantes para avaliar a eficácia dos modelos treinados.

### Metodologia

1. **Carregar e pré-processar os dados:** Dividir o dataset em conjuntos de treinamento, validação e teste. Redimensionar as imagens e realizar o one-hot encoding nas labels.
2. **Implementar modelos de Transfer Learning:** Utilizar EfficientNetB0 e MobileNetV2 para construir modelos de classificação.
3. **Treinar os modelos:** Treinar cada modelo utilizando os dados de treinamento e validação, com ajustes finos para evitar overfitting.
4. **Avaliar o modelo:** Medir o desempenho dos modelos no conjunto de teste utilizando métricas como acurácia e F1 score.

## Desenvolvimento dos Modelos

### MobileNetV2

MobileNetV2 foi escolhido por sua eficiência em balancear desempenho e custo computacional. O modelo foi ajustado para trabalhar com o dataset CIFAR-100, utilizando técnicas de pré-processamento específicas para a arquitetura MobileNetV2.

### EfficientNetB0

EfficientNetB0 foi utilizado pela sua arquitetura otimizada que oferece alta precisão com menor quantidade de parâmetros. O modelo foi configurado para congelar as camadas iniciais treinadas no ImageNet e treinar as camadas finais no dataset CIFAR-100.

## Treinamento e Avaliação

### Treinamento dos Modelos

Os modelos foram treinados por 30 épocas, utilizando um esquema de aprendizado distribuído com TPUs para acelerar o processo. A técnica de dropout foi aplicada para evitar overfitting.

### Avaliação do Modelo

A avaliação dos modelos foi feita no conjunto de teste, utilizando métricas como acurácia, F1 score, e visualização de exemplos de classificações corretas e incorretas para análise visual.

## Link para o projeto

<a href="https://github.com/rafarodrigues/visao-computacional/blob/main/ML%20-%20Classifica%C3%A7%C3%A3o%20de%20imagens%20CIFAR-100/classificacao-imagens-CIFAR100-v1.ipynb" target="_blank">visao-computacional/ML - Classificação de imagens CIFAR-100
/classificacao-imagens-CIFAR100-v1.ipynb</a>

## Resultados e Conclusão

Através da aplicação de Transfer Learning com MobileNetV2 e EfficientNetB0, foi possível alcançar um desempenho significativo no treinamento, mas abaixo do esperado na validação. Isso abre espaço para melhorias no treinamento e na busca de resultados melhores.

## Referências

- [CIFAR-100 Dataset](https://www.cs.toronto.edu/~kriz/cifar.html)
- [TensorFlow Datasets](https://www.tensorflow.org/datasets/catalog/cifar100?hl=en)