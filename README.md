# #  Tech Challenge 2 — Classificação da Qualidade de Vinhos com Machine Learning

##  Objetivo

Este projeto tem como objetivo desenvolver um modelo de Machine Learning capaz de classificar vinhos em duas categorias:

* **Alta qualidade (1):** nota maior ou igual a 7
* **Baixa qualidade (0):** nota inferior a 7

Para isso, são utilizadas técnicas de análise exploratória, tratamento de dados, pré-processamento, balanceamento de classes e comparação entre diferentes algoritmos de classificação.

---

##  Dataset

O projeto utiliza o conjunto de dados **WineQT**.

Antes de executar o notebook, faça o download do dataset e coloque o arquivo na mesma pasta do notebook com o nome:

```text
WineQT.csv
```

---

##  Tecnologias Utilizadas

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* XGBoost
* Imbalanced-Learn (SMOTE)

---

##  Estrutura do Projeto

```text
├── Tech Challenge - 2.ipynb
├── WineQT.csv
├── resultados_modelos.csv
└── README.md
```

---

##  Etapas Desenvolvidas

### 1. Importação das Bibliotecas

Instalação e carregamento das bibliotecas necessárias para análise e modelagem.

### 2. Carregamento dos Dados

Leitura do dataset utilizando o Pandas.

### 3. Definição do Problema

A variável **quality** é transformada em uma variável binária:

| Qualidade Original | Classe              |
| ------------------ | ------------------- |
| ≥ 7                | Alta Qualidade (1)  |
| < 7                | Baixa Qualidade (0) |

---

##  Análise Exploratória (EDA)

Foram realizadas diversas análises para compreender o comportamento dos dados:

* Estatísticas descritivas
* Verificação de valores nulos
* Distribuição das variáveis
* Boxplots por classe
* Heatmap de correlação

---

##  Limpeza dos Dados

Durante o tratamento foram realizadas as seguintes etapas:

* Remoção de registros duplicados
* Verificação de valores ausentes
* Análise de outliers
* Consolidação da qualidade dos dados

---

## Pré-processamento

O pipeline de preparação contempla:

* Separação entre atributos e variável alvo
* Divisão entre treino e teste
* Padronização utilizando **StandardScaler**
* Balanceamento das classes com **SMOTE**

---

## Modelos Avaliados

Foram treinados e comparados diferentes algoritmos de Machine Learning.

Os modelos foram avaliados utilizando métricas como:

* Accuracy
* Precision
* Recall
* F1-Score
* ROC-AUC

Também foram gerados:

* Matrizes de Confusão
* Curvas ROC
* Comparação gráfica das métricas

---

##  Interpretabilidade

Após a avaliação dos modelos, foi realizada a análise da importância das variáveis (**Feature Importance**) para identificar quais atributos possuem maior influência na classificação da qualidade dos vinhos.

---

##  Resultado Final

Ao final da execução, o projeto:

* compara o desempenho dos modelos;
* identifica o melhor algoritmo;
* apresenta um relatório consolidado das métricas;
* exporta os resultados para um arquivo CSV.

---

##  Como Executar

1. Clone o repositório.

```bash
git clone https://github.com/seu-usuario/seu-repositorio.git
```

2. Entre na pasta do projeto.

```bash
cd seu-repositorio
```

3. Instale as dependências.

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost imbalanced-learn
```

4. Coloque o arquivo **WineQT.csv** na pasta do projeto.

5. Execute o notebook **Tech Challenge - 2.ipynb**.

---

##  Fluxo do Projeto

```text
Dataset
    │
    ▼
Análise Exploratória
    │
    ▼
Limpeza dos Dados
    │
    ▼
Pré-processamento
    │
    ├── StandardScaler
    └── SMOTE
          │
          ▼
Treinamento dos Modelos
          │
          ▼
Avaliação
          │
          ▼
Comparação
          │
          ▼
Melhor Modelo
          │
          ▼
Interpretação e Exportação dos Resultados
```

---

Tecnologias: Python • Machine Learning • SQL • Power BI • Databricks
