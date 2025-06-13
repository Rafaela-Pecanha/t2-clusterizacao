# 📊 Clustering no Conjunto de Dados Iris

## 🎯 Objetivo

Este projeto tem como objetivo explorar algoritmos de **clustering (agrupamento não supervisionado)** aplicados ao conjunto de dados **Iris**, buscando identificar agrupamentos naturais **sem utilizar os rótulos reais** das espécies. Os agrupamentos serão avaliados tanto com métricas **intrínsecas** quanto **extrínsecas**.

---

## 🛠️ Etapas do Projeto

### a) Pré-processamento e Análise Exploratória

- Carregamento do dataset Iris.
- Análise visual com gráficos e técnicas de redução de dimensionalidade (como PCA).
- Normalização dos dados para garantir comparabilidade entre variáveis.
- Identificação visual do número provável de grupos naturais.

---

### b) Algoritmo K-Means

#### i) Escolha do número de clusters (k)
- Utilização do **método do cotovelo**, variando `k` de 1 a 10.

#### ii) Aplicação do KMeans
- Aplicação do algoritmo com o valor de `k` indicado pelo método do cotovelo.
- Consideração do valor `k=3`, por conhecimento externo das 3 espécies (para comparação).

#### iii) Visualização
- Gráficos de dispersão com clusters obtidos.
- Redução de dimensionalidade (PCA) para facilitar visualização.

---

### c) Agrupamento Hierárquico (Agglomerative Clustering)

#### i) Dendrograma
- Geração de dendrograma para ajudar na definição do número de clusters.

#### ii) Aplicação do algoritmo
- Uso do Agglomerative Clustering com número de clusters definido via dendrograma.

#### iii) Visualização
- Gráficos de dispersão para os agrupamentos hierárquicos.

---

### d) Avaliação e Interpretação

#### i) Comparação com classes reais
- Cálculo do **Adjusted Rand Index (ARI)**.
- Cálculo da acurácia com mapeamento de rótulos.

#### ii) Métricas intrínsecas
- Cálculo do **Silhouette Score**.
- Outras métricas: Davies-Bouldin.

#### iii) Visualizações
- Gráficos comparando os agrupamentos obtidos com os rótulos reais.

#### iv) Discussão
- Análise sobre a capacidade do KMeans e do agrupamento hierárquico em separar as espécies.
- Identificação de espécies mais difíceis de separar.
- Interpretação da estrutura hierárquica observada no dendrograma.

---

### e) Comparação com Subconjunto de Features

- Repetição das etapas de clustering usando apenas duas variáveis: **comprimento** e **largura da pétala**.
- Comparação dos resultados com os obtidos usando todas as features.
- Discussão sobre o impacto da escolha das variáveis no desempenho dos algoritmos.

---

## 👨‍💻 Tecnologias e Bibliotecas Utilizadas

- Python 3.x
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib & Seaborn
- Scikit-learn
- Scipy (para dendrogramas)

---

## 👩‍💻 Autores

- Rafaela P. M. Fernandes
- Atharv Nuthi

Instituto de Computação – Universidade Federal Fluminense (UFF)  
Emails: rafaelapecanha@id.uff.br, atharvnuthi@id.uff.br

---

## 📚 Referências

- Scikit-learn Documentation: https://scikit-learn.org
- UCI Machine Learning Repository: Iris Dataset
- Artigos e materiais de apoio do curso

