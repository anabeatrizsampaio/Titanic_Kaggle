# Análise e Previsão de Sobrevivência no Titanic 
Kaggle: https://www.kaggle.com/competitions/titanic/overview 

## Visão Geral

Este projeto aborda o desafio clássico de prever quais passageiros sobreviveram ao naufrágio do Titanic com base em dados como classe de cabine, sexo, idade e outras informações.

## Conjunto de Dados

O conjunto de dados contém informações sobre:
- 891 passageiros no conjunto de treino
- 418 passageiros no conjunto de teste

  Variáveis incluídas:
- `Survived`: Sobreviveu (0 = Não, 1 = Sim) - variável alvo
- `Pclass`: Classe do ticket (1 = 1ª classe, 2 = 2ª classe, 3 = 3ª classe)
- `Name`, `Sex`, `Age`
- `SibSp`: Número de irmãos/cônjuges a bordo
- `Parch`: Número de pais/filhos a bordo
- `Ticket`: Número do ticket
- `Fare`: Tarifa paga
- `Cabin`: Número da cabine
- `Embarked`: Porto de embarque (C = Cherbourg, Q = Queenstown, S = Southampton)

## Bibliotecas utilizadas
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn

## Metodologia

### 1. Análise Exploratória de Dados (EDA)
- Visualização de distribuições e relações entre variáveis
- Identificação de valores faltantes e outliers

### 2. Pré-processamento
- Tratamento de dados faltantes
- Engenharia de features (criação de novas variáveis)
- Codificação de variáveis categóricas
- Normalização/escala de features numéricas

### 3. Modelagem
- Nesse modelo foi utilizado o algoritmo Random Forest 
- Validação cruzada
- Ajuste de hiperparâmetros

### 4. Avaliação
- Métrica principal: Acurácia
- Matriz de confusão

| Modelo               | Acurácia (Validação) | Acurácia (Kaggle) |
|----------------------|---------------------|------------------|
| Random Forest        | 0.80                | 0.78             |

**Melhor score no Kaggle:** 0.79 (Top 12% na competição)
