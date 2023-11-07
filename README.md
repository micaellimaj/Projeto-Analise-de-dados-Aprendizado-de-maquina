# Projeto Análise de dados: Aprendizado de Máquina

O conjunto de dados utilizados para a realização desse projeto nos traz dados relevantes sobre pacientes que podem desenvolver diabete com base em vários atributos.Com o conjunto de dados, criamos dois modelos de aprendizado de máquina, um de agrupamento e outro de classificação, para realizar predições dos pacientes com base em seu histórico médico. Acabei abordando na parte do agrupamento algumas técnicas como o K-Medias para alocar os dados para o seu grupo mais próximo; além de separa os dados em treino e teste; e utilizar método de avaliação para melhor generalizar as predições. E na parte da classificação abordei técnica semelhantes ao anterior, como, separar os dados em treino e teste e o método de avaliação para melhorar a capacidade de predição do modelo, no entanto, além desses, utilizei a matriz de confusão, que resume as predições feitas por um modelo e a acuária para verificar a porcentagem de acertos do modelo. 

O conjunto de dados utilizados para esse projeto pode ser encontrado no seguinte link: 
https://www.kaggle.com/datasets/iammustafatz/diabetes-prediction-dataset

### Painel:

Para a realização desse projeto eu também decidir criar um dashboard no power Bi para auxiliar na análise do conjunto de dados, com a implementalção de visuais para entender a distribuição e o comportamento dos dados e em especial para o visual de IA que mostrar a probabilidade do paciente ter diabetes com base em alguns atributos que selecionamos no gráfico. Link do dashboard: https://bit.ly/Micael-Lima-Analista-de-dados-Dashboard-Diabetes

### Tecnologias utilizadas:

* <img src="https://img.shields.io/badge/Python-000000?style=for-the-badge&logo=python&logoColor=yellow1" alt="icon python" > 
* <img src="https://img.shields.io/badge/Power_BI-000000?style=for-the-badge&logo=powerbi&logoColor=yellow" alt="icon power bi">
* <img src="https://img.shields.io/badge/Colab-F9AB00?style=for-the-badge&logo=googlecolab&color=525252" alt="icon colab">

### Atributos dos dados:

O dataset utilizado para esse projeto de análise de dados utilizando técnicas de aprendizado de máquina: classificação e agrupamento, possui as seguintes colunas:

* gender: refere-se ao sexo biológico do indivíduo, o que pode ter impacto na sua suscetibilidade ao diabetes. Existem três categorias nele: masculino, feminino e outros.
* age: é um fator importante, pois o diabetes é mais comumente diagnosticado em adultos mais velhos. A idade varia de 0 a 80 em nosso conjunto de dados.
* hypertesion: é uma condição médica na qual a pressão sanguínea nas artérias é persistentemente elevada. Tem valores 0 ou 1 onde 0 indica que não tem hipertensão e 1 significa que tem hipertensão.
* heart_disease: é outra condição médica que está associada a um risco aumentado de desenvolver diabetes. Tem valores 0 ou 1 onde 0 indica que não tem doença cardíaca e 1 significa que tem doença cardíaca.
* smoking_history: O histórico de tabagismo também é considerado um fator de risco para diabetes e pode exacerbar as complicações associadas ao diabetes. Em nosso conjunto de dados, temos 5 categorias, ou seja, não atual, anterior, sem informações, atual, nunca e sempre.
* bmi: IMC (Índice de Massa Corporal) é uma medida de gordura corporal com base no peso e na altura. Valores mais altos de IMC estão associados a um maior risco de diabetes. A faixa de IMC no conjunto de dados é de 10,16 a 71,55. IMC inferior a 18,5 é baixo peso, 18,5-24,9 é normal, 25-29,9 é sobrepeso e 30 ou mais é obeso.
* HbA1c_level: O nível de HbA1c (Hemoglobina A1c) é uma medida do nível médio de açúcar no sangue de uma pessoa nos últimos 2-3 meses. Níveis mais altos indicam um risco maior de desenvolver diabetes. Principalmente mais de 6,5% do nível de HbA1c indica diabetes.
* blood_glucose_level: O nível de glicose no sangue refere-se à quantidade de glicose na corrente sanguínea em um determinado momento. Níveis elevados de glicose no sangue são um indicador chave de diabetes.
* diabetes: é a variável alvo prevista, com valores de 1 indicando a presença de diabetes e 0 indicando a ausência de diabetes.

### Desenvolvimento:

Foram aplicadas diversas técnicas na construção desse projeto como:

* Verificação da estrutura dos dados e possíveis correções de erros para valores incorretos
* Análise da distribuição dos valores na base de dados e geração de insights
* Agrupamento de dados para seu grupo mais próximo mediante o conjunto de clusters
* Separação dos dados em treino e teste para evitar que os dados só sejam decorados e não realize as predições corretamente
* Utilização do método do cotovelo para uma boa generalização dos dados
* Manipulação e alteração no formato da dat para melhor se adequar ao objetivo da análise de dados
* Utilização de uma árvore de decisão para segmentar os dados
* Uso de uma matriz de confusão para comparar os dados com a realidade e a acuária para medir a exatidão do modelo de aprendizado de máquina
* Realização de predição dos dados conforme os objetivos das análises
* Criação de um dashboard de análise de pacientes do hospital com os dados do dataset desse caderno
### Importações python:

```
import numpy as np
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt
import plotly.express as px
import seaborn.objects as so
from IPython.display import Image, display
import graphviz
from sklearn import tree
from sklearn.metrics import confusion_matrix
from sklearn.metrics import accuracy_score
```

### Referências:

Alguns sites que serviram de auxílio para a construção desse projeto:

* https://ebaconline.com.br/
* https://www.kaggle.com/
* https://seaborn.pydata.org/tutorial/introduction.html
* https://br.freepik.com/
* https://scikit-learn.org/stable/

--------

