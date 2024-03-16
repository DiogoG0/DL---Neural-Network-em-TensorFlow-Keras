# Classificação de Imagens com Caltech101

Este projeto visa desenvolver um modelo de classificação de imagens usando o conjunto de dados Caltech101. 
O objetivo é criar um modelo capaz de classificar imagens em uma das 101 classes diferentes de objetos presentes no conjunto de dados.

## Conteúdo

1. [Visão Geral]
2. [Requisitos]
3. [Como Usar]
4. [Arquitetura do Modelo]
5. [Treinar o modelo]
6. [Avaliação do Modelo]
7. [Referências]

## Visão Geral

O conjunto de dados Caltech101 é composto por imagens coloridas de objetos pertencentes a 101 categorias diferentes, incluindo animais, veículos, alimentos, entre outros. O objetivo deste projeto é treinar um modelo de aprendizagem  para reconhecer automaticamente os objetos nessas imagens e classificá-los corretamente em uma das categorias.

## Requisitos

- Google Colab
- TensorFlow
- TensorFlow Datasets
- Outras bibliotecas conforme necessário 


## Como Usar

1. Fazer download do conjunto de dados Caltech101 e preparar os dados para o treino do modelo.
2. Escolher e definir a arquitetura do modelo a ser utilizada.
3. Compilar o modelo com o otimizador, função de perda e métricas apropriadas (precisão).
4. Treine o modelo usando o conjunto de dados de treinamento.
5. Avaliar o modelo usando o conjunto de dados de teste.
6. Fazer previsões usando o modelo que treinámos.

## Arquitetura do Modelo

Neste projeto, são explorados dois tipos de modelos de arquitetura: o baseline, que é um modelo simples utilizado para comparar com o modelo de regularização L2 (l2_model), que incorpora regularização L2 nas camadas densas. 


## Treinar o modelo

Durante o treino do modelo, é importante estar atento regularmente à perda e à precisão do modelo no conjunto de dados de validação de modo a evitar o overfitting. 
Caso acontença, podemos ajustar os hiperparametros do modelo, como o número de epochs, aumentar o número de dados de treino, diminuir a regularzação de l2, para evitar problemas de overfitting e obter o melhor desempenho do modelo.

## Avaliação do Modelo

Após treinar o modelo, avaliámos o modelo usando o conjunto de dados de teste para verificar o desempenho do modelo em dados não vistos. Analisámos métricas como precisão.
Podemos verificar que a precisão do modelo parece estabilizar após um certo número de epochs, indicando-nos que o modelo atingiu um ponto onde não melhora significativamente com mais treino, o que significa que treinar outra vez pode não ser benéfico e pode até levar ao overfitting.

## Referências

- Documentação do TensorFlow: [TensorFlow Documentation](https://www.tensorflow.org/api_docs)
- TensorFlow Datasets: [TensorFlow Datasets](https://www.tensorflow.org/datasets)
- Exemplos do TensorFlow: [TensorFlow Examples](https://www.tensorflow.org/tutorials)


