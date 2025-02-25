# Bank-Customer-Churn-Prediction-Kaggle
Este projeto visa prever a saída de clientes de um banco (churn) utilizando técnicas de Machine Learning. O modelo final é um ensemble de LightGBM e Gradient Boosting.

# Bank Customer Churn Prediction

Este projeto tem como objetivo prever a saída de clientes de um banco (churn) utilizando técnicas de Machine Learning. O modelo final foi desenvolvido utilizando um ensemble de LightGBM e Gradient Boosting, com um foco em maximizar o F1-score.

## Estrutura do Projeto

1. **Bibliotecas e Configurações Iniciais**
    - Importação das bibliotecas necessárias para análise de dados, pré-processamento e modelagem.

2. **Tratamento dos Dados**
    - Carregamento e descrição dos dados de treino e teste.
    - Análise descritiva e exploração dos dados.
    - Tratamento de variáveis categóricas e numéricas.

3. **Pré-processamento e Enriquecimento de Dados**
    - Separação dos dados em variáveis independentes (X) e dependentes (y).
    - Aplicação de técnicas de escalonamento e codificação one-hot.
    - Divisão dos dados em conjuntos de treino e teste.

4. **Modelos de Machine Learning**
    - Avaliação de diferentes modelos utilizando validação cruzada.
    - Tuning de hiperparâmetros dos melhores modelos.
    - Seleção de features mais importantes.
    - Criação de ensembles (Voting e Stacking) para melhorar a performance do modelo.

5. **Métricas do Modelo Final**
    - Avaliação do modelo final utilizando métricas como F1-score, matriz de confusão, curva ROC e curva Precision-Recall.

## Resultados

- **Recall (0.63):** O modelo identifica corretamente 63% dos clientes que saíram.
- **Precision (0.81):** 81% dos clientes previstos como churn realmente saíram.
- **ROC-AUC (0.94):** Excelente capacidade de diferenciar entre clientes que saíram e os que não saíram.
- **Average Precision (0.82):** Bom equilíbrio entre precisão e recall, mesmo com desbalanceamento de classes.

## Conclusão

O modelo final, um ensemble de LightGBM e Gradient Boosting, apresentou um desempenho robusto com um F1-score elevado. No entanto, há espaço para melhorias na sensibilidade do modelo para identificar mais clientes que saíram, ajustando o limiar de classificação ou abordando o desbalanceamento de classes.

## Requisitos

- Python 3.x
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- LightGBM
- ydata_profiling
- ipywidgets
- PIL

## Como Executar

1. Clone o repositório:
    ```bash
    git clone https://github.com/seu-usuario/seu-repositorio.git
    ```

2. Navegue até o diretório do projeto:
    ```bash
    cd seu-repositorio
    ```

3. Instale as dependências:
    ```bash
    pip install -r requirements.txt
    ```

4. Execute o Jupyter Notebook:
    ```bash
    jupyter notebook
    ```

5. Abra o notebook e execute as células sequencialmente.

## Autor

- [José Vinícius Tavares](https://github.com/JoseVTavares)

## Licença

Este projeto está licenciado sob a Licença MIT - veja o arquivo [LICENSE](LICENSE) para mais detalhes.
