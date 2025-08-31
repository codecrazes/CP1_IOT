# Projeto IoT - Redução de Dimensionalidade e Análises

Este repositório contém os exercícios relacionados à disciplina de **IoT**, incluindo análise e redução de dimensionalidade utilizando **PCA**.

## Instruções para Clonar o Repositório

Para obter uma cópia local do projeto, utilize o comando abaixo:

```bash
git clone <URL_DO_REPOSITORIO>
```

Substitua `<URL_DO_REPOSITORIO>` pela URL do repositório Git.

## Integrantes do Projeto

* Caroline Assis Silva (RM557596)
* Enzo de Moura Silva (RM556532)
* Luis Henrique Gomes Cardoso (RM558883)

---

## Bibliotecas Necessárias

Para executar os exercícios, você precisará instalar as seguintes bibliotecas Python:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn statsmodels
```

### Bibliotecas utilizadas nos exercícios

* **pandas** – manipulação de dados
* **numpy** – operações numéricas
* **matplotlib.pyplot** – visualização de dados
* **seaborn** – visualização estatística
* **sklearn.preprocessing.MinMaxScaler** – normalização de dados
* **sklearn.preprocessing.StandardScaler** – padronização de dados
* **sklearn.cluster.KMeans** – clustering
* **sklearn.decomposition.PCA** – redução de dimensionalidade
* **sklearn.linear\_model.LinearRegression** – regressão linear
* **sklearn.linear\_model.LogisticRegression** – regressão logística
* **sklearn.ensemble.RandomForestRegressor / RandomForestClassifier** – modelos de Random Forest
* **sklearn.preprocessing.PolynomialFeatures** – regressão polinomial
* **sklearn.model\_selection.train\_test\_split** – divisão de dados em treino e teste
* **sklearn.metrics** – métricas como MSE, R², acurácia, precisão, recall, F1, ROC AUC, matriz de confusão
* **statsmodels.tsa.seasonal.seasonal\_decompose** – decomposição de séries temporais
* **statsmodels.graphics.tsaplots.plot\_acf** – autocorrelação
* **pandas.plotting.autocorrelation\_plot** – plot de autocorrelação rápida

---

## Instruções para os Datasets

Os exercícios utilizam datasets que **não estão incluídos no repositório** devido ao tamanho. Você deve baixar os arquivos e colocá-los na pasta `DataSet/`:

* **Dataset 1 (df1)**: [Individual Household Electric Power Consumption](https://archive.ics.uci.edu/dataset/235/individual+household+electric+power+consumption)
* **Dataset 2 (df2)**: [Appliances Energy Prediction](https://archive.ics.uci.edu/dataset/374/appliances+energy+prediction)

⚠️ **Importante:** Altere os caminhos nos exercícios de acordo com a localização dos arquivos baixados.

* O parâmetro **`caminho_arquivo`** é utilizado no **exercício 1**.
* O parâmetro **`caminho_arquivo_2`** é utilizado no **exercício 26**.

---

## Projeto Realizado no Orange

Para este exercício, utilizamos o software **Orange** para realizar análise de clustering e visualização de dados. O dataset utilizado foi o **Individual Household Electric Power Consumption**, que contém informações detalhadas sobre o consumo elétrico de uma residência.

A análise incluiu:

* Amostragem de 1% do dataset para análise exploratória.
* Observação da distribuição de consumo.
* Verificação de correlação entre variáveis como Voltage e Global\_intensity.
* Aplicação de **k-Means** para identificar padrões de consumo doméstico.

---

## Respostas dos Exercícios

1. 2075259
2. Sim, a distribuição da amostra de 1% é semelhante à da base completa, concentrada em valores baixos com poucos registros de alto consumo.
3. O consumo é concentrado em valores baixos, com poucos registros de alto consumo.
4. Não existe correlação visível clara entre Voltage e Global\_intensity; os pontos se concentram em baixa intensidade, enquanto a tensão permanece estável.
5. Sim, cada cluster representa um padrão distinto de consumo doméstico — desde momentos de baixo consumo, passando por uso específico de um ambiente/aparelho, até picos de consumo mais altos.
