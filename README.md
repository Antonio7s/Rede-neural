# Rede-neural
Rede neural para classificação de intenções de frases utilizando TensorFlow. Um exemplo simples de assistente virtual baseado em NLP para identificar intenções em frases do usuário.
# Assistente Virtual - Classificação de Intenções

Este projeto contém um modelo de **rede neural** para classificar intenções de frases de usuários, usando técnicas de **Processamento de Linguagem Natural (NLP)**. O objetivo deste modelo é identificar o que o usuário deseja, como, por exemplo, consultar o tempo, fazer uma compra ou solicitar ajuda, com base em suas frases.

## Visão Geral

O modelo foi construído utilizando a biblioteca **TensorFlow** e segue os seguintes passos principais:

1. **Pré-processamento de dados**: 
   - As frases dos usuários são tokenizadas (divididas em palavras).
   - As palavras são lematizadas (reduzidas às suas formas básicas).
   - A entrada é convertida para um formato numérico que pode ser entendido pela rede neural.

2. **Modelo de Rede Neural**:
   - O modelo é uma rede neural simples com camadas densas.
   - Ele é treinado para identificar intenções associadas às frases de entrada.
   - A saída do modelo é a **intenção** da frase, como "previsao_tempo", "fazer_compra", etc.

3. **Treinamento e Previsão**:
   - O modelo é treinado usando um conjunto de frases e suas intenções associadas.
   - Após o treinamento, o modelo pode classificar novas frases e determinar qual a intenção do usuário.

## Como Funciona

1. **Entrada**: Uma frase do usuário, como por exemplo:
   - "Qual o tempo hoje?"
   - "Me ajude a fazer uma compra"

2. **Processamento**:
   - O modelo converte a frase em um vetor de números.
   - Esse vetor é alimentado na rede neural.

3. **Saída**: A rede neural retorna a intenção da frase, como:
   - "previsao_tempo"
   - "fazer_compra"

## Tecnologias Utilizadas

- **TensorFlow**: Framework de aprendizado de máquina usado para construir e treinar o modelo.
- **NLTK (Natural Language Toolkit)**: Biblioteca para o processamento de texto, como tokenização e lematização.

## Requisitos

- Python 3.x
- TensorFlow
- NLTK
- NumPy
- scikit-learn

## Como Rodar

### 1. Instalar as dependências:

```bash
pip install tensorflow nltk numpy scikit-learn
