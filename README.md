# Análise exploratória de dados íris
Este código é um exemplo de análise exploratória de dados usando bibliotecas em Python. Ele inclui a leitura e limpeza 
dos dados, o cálculo de estatísticas descritivas, a criação de histogramas e boxplots, a análise de correlações e a 
realização de testes de normalidade com foco em um conjunto de dados de íris ('iris.csv'). Explicação das seções do 
código para fornecer uma compreensão clara de suas funcionalidades:

## 1. Importação de bibliotecas

* pandas é usada para manipulação de dados.
* seaborn e matplotlib são usadas para visualização de dados.
* scipy.stats é usada para realizar o teste de normalidade.

## 2. Carregamento dos dados
* Os dados são lidos a partir do arquivo 'iris.csv' usando pd.read_csv.
* Algumas linhas do DataFrame são exibidas com df.head(150) para visualização.

## 3. Limpeza dos dados:
* Linhas com valores nulos são removidas com df.dropna().
* Linhas duplicadas são removidas com df.drop_duplicates().

## 4. Análise das estatísticas básicas
* Média, variância, desvio padrão e mediana são calculados para as colunas 'sepal_length' e 'sepal_width'.

## 5. Histogramas
* Histogramas das colunas 'sepal_length' e 'sepal_width' são plotados usando plt.hist.

## 6. Boxplots
* Boxplots das colunas 'sepal_length' e 'sepal_width' são plotados usando sns.boxplot.

## 7. Coeficiente de correlação
* A matriz de correlação entre todas as colunas numéricas é calculada com df.corr().
* Um gráfico de dispersão entre 'sepal_length' e 'sepal_width' é criado usando sns.scatterplot.

## 8.Teste de normalidade
* O teste de normalidade é realizado para as colunas 'sepal_length' e 'sepal_width' usando normaltest. O resultado 
inclui o valor de estatística K² e o valor p.
* O valor p é comparado com um nível de significância (alpha) para determinar se os dados seguem uma distribuição 
normal.

## 9. Gráfico do teste de normalidade junto com o histograma
* Os gráficos de histograma são plotados novamente junto com as curvas de distribuição para visualizar a normalidade dos
dados.
