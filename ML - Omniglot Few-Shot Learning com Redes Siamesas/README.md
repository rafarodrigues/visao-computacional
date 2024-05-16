# Omniglot Few-Shot Learning com Redes Siamesas

> Este repositório apresenta a aplicação de Redes Siamesas para resolver o problema de one-shot learning, utilizando o dataset Omniglot.

</br> <div align="center"> <img src="https://github.com/brendenlake/omniglot/raw/master/omniglot_grid.jpg" width="800"> </div>

## Introdução

O one-shot learning é um desafio na área de aprendizado de máquina, onde o objetivo é aprender informações sobre categorias a partir de apenas um ou poucos exemplos. Este repositório documenta a aplicação de Redes Siamesas para classificar imagens do dataset Omniglot, abordando desde o carregamento e pré-processamento dos dados até a construção, treinamento e avaliação dos modelos.

## Sobre o Omniglot

O Omniglot é um conjunto de dados composto por 1.623 caracteres de 50 alfabetos diferentes, com 20 exemplos por caractere. Cada imagem possui 105x105 pixels e é comumente utilizado para problemas de one-shot learning devido à sua diversidade e complexidade.

**Links úteis:**

- [Omniglot Dataset](https://www.cs.cmu.edu/~rsalakhu/papers/oneshot1.pdf)
- [Repositório Original do Código](https://github.com/akshaysharma096/Siamese-Networks/blob/master/Few%20Shot%20Learning%20-%20V1.ipynb)

## Objetivos e Metodologia

### Objetivos

- **Atualizar o código:** Substituir bibliotecas e funções descontinuadas por alternativas modernas.
- **Implementar Redes Siamesas:** Utilizar a arquitetura proposta por Gregory et al. para resolver o problema de one-shot learning.
- **Avaliar o desempenho:** Medir a acurácia e outras métricas relevantes para avaliar a eficácia dos modelos treinados.

### Metodologia

1. **Carregar e pré-processar os dados:** Preparar o dataset Omniglot, dividindo-o em conjuntos de treinamento e validação.
2. **Implementar Redes Siamesas:** Construir o modelo utilizando Keras e TensorFlow, seguindo a arquitetura proposta no paper.
3. **Treinar os modelos:** Utilizar técnicas de regularização e otimização de hiperparâmetros para melhorar o desempenho.
4. **Avaliar o modelo:** Realizar testes de one-shot learning e medir a acurácia nos conjuntos de validação.

## Desenvolvimento dos Modelos

### Arquitetura da Rede Neural Siamesa

A Rede Neural Siamesa é composta por duas sub-redes idênticas que processam duas imagens em paralelo. A diferença entre as saídas das sub-redes é utilizada para determinar se as imagens pertencem à mesma classe.

### Hiperparâmetros

Foram otimizados diversos hiperparâmetros utilizando um framework de otimização bayesiana, incluindo taxas de aprendizado, penalidades de regularização L2, e tamanhos de filtros convolucionais.

## Treinamento e Avaliação

### Treinamento dos Modelos

Os modelos foram treinados utilizando técnicas de data augmentation e esquemas de aprendizado distribuído com TPUs para acelerar o processo.

### Avaliação do Modelo

A avaliação foi realizada com tarefas de one-shot learning, onde o modelo deve identificar a imagem correspondente em um conjunto de suporte. As métricas de avaliação incluíram acurácia e análise de exemplos de classificações corretas e incorretas.

## Resultados e Conclusão

A aplicação de Redes Siamesas no dataset Omniglot demonstrou um desempenho promissor, embora existam oportunidades para melhorias, como a experimentação com outras arquiteturas de redes e técnicas de regularização.

## Referências

- [Siamese Neural Networks for One-shot Image Recognition](https://www.cs.cmu.edu/~rsalakhu/papers/oneshot1.pdf)
- [Repositório Original do Código](https://github.com/akshaysharma096/Siamese-Networks/blob/master/Few%20Shot%20Learning%20-%20V1.ipynb)

## Links para o Projeto

- [Projeto no GitHub](https://github.com/seu_usuario/seu_projeto)

Este README serve como guia completo para o projeto de aprendizado de máquina utilizando Redes Siamesas para one-shot learning, fornecendo uma visão geral, metodologia, e resultados obtidos.