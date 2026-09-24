# Detecção de Fraude em Transações

## Objetivo

Desenvolver e comparar modelos de Machine Learning para identificação de transações fraudulentas, utilizando técnicas de seleção de variáveis, clusterização e otimização de métricas para bases desbalanceadas.

## Tecnologias

- Python
- Pandas
- NumPy
- Scikit-Learn
- XGBoost
- LightGBM
- Matplotlib
- NLTK

## Metodologia

### Pré-processamento

- Tratamento de valores ausentes
- Winsorização de outliers
- Padronização de variáveis
- Codificação de variáveis categóricas

### Seleção de Variáveis

Foram avaliados diferentes conjuntos de variáveis:

- top5
- top10
- top15
- top20
- top_total
- di_top10
- di_top15
- di_top20

### Clusterização

Foram avaliados:

- KMeans
- KMedoids

Utilizando:

- Silhouette Score
- Davies-Bouldin Index
- Calinski-Harabasz Index
- Estabilidade dos clusters

### Modelos Testados

- Logistic Regression
- Decision Tree
- Random Forest
- XGBoost
- LightGBM

## Métricas Avaliadas

- Average Precision (AP)
- AUC ROC
- F1-Score
- Precisão
- Cobertura (Recall)
- Erros por Acerto

## Principais Resultados

Melhor resultado:

| Modelo | Feature Set | AUC |
|----------|----------|---------:|
| Logistic Regression | top_total | 0.8296 |

## Estrutura do Projeto

```text
.
├── main.py
├── requirements.txt
├── README.md
├── models/
└── outputs/
```

## Instalação

```bash
pip install -r requirements.txt
```

## Execução

```bash
python main.py
```

## Autor

Erick Da Silva Florentino
