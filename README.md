<h1 align="center">
  REDE NEURAL PARA DETERMINAR A TEMPERATURA DO AR
</h1>

<hr>

![Badge em Desenvolvimento](http://img.shields.io/static/v1?label=STATUS&message=Completo&color=GREEN&style=for-the-badge)

# Sobre

 Projeto desenvolvido na disciplina Tópicos Especiais D - Inteligencia Artificial do curso de graduação em Física. O objetivo é aplicar os conhecimentos teóricos adquiridos em sala de aula.

 O objetivo principal foi desenvolver uma Rede Neural Convolucional capaz determinar a temperatura do ar.

# Funcionalidades e Entidades

## Funcionalidades
- ### Carregar os dados para o treinamento
  A função load_data carrega os dados da pasta data e organiza todos em um novo arquivo csv (all_data.csv)

- ### Previsão de saída
  A rede neural pode realizar previsões com base nos dados de entrada fornecidos após ter sido treinada.

## Entidades
- ### Rede Neural
  A arquitetura da rede neural utilizada consiste em um sequência de camadas que incluem um camada de Input, umada de Conv1D, uma camada de MaxPooling1D, uma camada Flatten e 2 camadas Dense, sendo a ultima a saida.

  - **Camada InputLayer**: Camada de entrada que recebe
  - **Camada Conv1D**:
  - **Camada MaPooling1D**:
  - **Camada Flatten**:
  - **Camadas Dense**:

- ### Compilação do Modelo
  O modelo foi compilado usando o otmizador Adam e a função de perda de erro médio absoluto (mae). A métrica de avaliação utilizada foi a raiz quadrada do erro-médio (RootMeanSquaredError)

- ### Treinamento do Modelo
  O modelo foi treinado por aproximadamente x épocas com um lote (batch) igual a 128. Os dados de treinamento e validação foram fornecidos durante o treinamento para monitorar o desempenho do modelo ao longo do tempo. Além disso, foi utilizado um callback de Early Stopping para interromper o treinamento se a perda não melhorasse após 10 épocas.

# Resultados

A rede neural foi treinada com dados meteorológicos do inmet de 2007 a 2024 da cidade de Pampulha/MG

# Tecnologias utilizadas

- [Python](https://www.python.org)
- [Jupyter Notebook](https://jupyter.org)
- [Pandas](https://pandas.pydata.org)
- [NumPy](https://numpy.org)
- [Tensorflow](https://www.tensorflow.org)
- [Keras](https://keras.io)
- [Scikit-learn](https://scikit-learn.org/stable/)
