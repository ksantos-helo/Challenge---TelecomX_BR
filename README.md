# 📊 Análise de Evasão de Clientes (Churn) — Telecom X

## 📌 Sobre o Projeto

Este projeto tem como objetivo analisar os fatores que influenciam a evasão de clientes (Churn) em uma empresa fictícia de telecomunicações chamada Telecom X.

A evasão de clientes é um problema crítico para empresas de serviços recorrentes, pois impacta diretamente:

✔️📉 Receita recorrente

✔️💰 Custos de aquisição de novos clientes

✔️📊 Crescimento do negócio

Através de Análise Exploratória de Dados (EDA), buscamos identificar padrões de comportamento que ajudam a explicar por que clientes cancelam o serviço.

Os insights gerados podem apoiar estratégias de retenção e melhoria da experiência do cliente.

## 🎯 Objetivos da Análise

✔️Identificar fatores que influenciam o cancelamento de clientes

✔️Explorar padrões em dados demográficos, financeiros e de serviços

✔️Avaliar correlações entre variáveis

✔️Gerar insights estratégicos para retenção de clientes

## 📂 Estrutura do Projeto

```
telecom-churn-analysis/
│
├── README.md                     # Documentação do projeto
├── telecom_churn_analysis.ipynb  # Notebook com análise dos dados
│
└── data/
    └── TelecomX_Data.json        # Base de dados utilizada no projeto

```



Descrição dos arquivos:

README.md → documentação do projeto

telecom_churn_analysis.ipynb → notebook com análise completa

TelecomX_Data.json → dataset utilizado

## 🗂️ Dataset

O conjunto de dados contém informações sobre clientes da Telecom X, incluindo dados demográficos, serviços contratados, informações de conta e dados financeiros utilizados para análise de Churn (cancelamento de clientes).

| Categoria               | Variável           | Descrição                                   |
| ----------------------- | ------------------ | ------------------------------------------- |
| 👥 Dados Demográficos   | `gender`           | Gênero do cliente                           |
| 👥 Dados Demográficos   | `SeniorCitizen`    | Indica se o cliente possui 65 anos ou mais  |
| 👥 Dados Demográficos   | `Partner`          | Indica se o cliente possui parceiro(a)      |
| 👥 Dados Demográficos   | `Dependents`       | Indica se o cliente possui dependentes      |
| 📡 Serviços Contratados | `PhoneService`     | Cliente possui serviço telefônico           |
| 📡 Serviços Contratados | `MultipleLines`    | Cliente possui múltiplas linhas telefônicas |
| 📡 Serviços Contratados | `InternetService`  | Tipo de serviço de internet contratado      |
| 📡 Serviços Contratados | `OnlineSecurity`   | Serviço de segurança online                 |
| 📡 Serviços Contratados | `OnlineBackup`     | Serviço de backup online                    |
| 📡 Serviços Contratados | `DeviceProtection` | Proteção de dispositivo                     |
| 📡 Serviços Contratados | `TechSupport`      | Suporte técnico                             |
| 📡 Serviços Contratados | `StreamingTV`      | Serviço de streaming de TV                  |
| 📡 Serviços Contratados | `StreamingMovies`  | Serviço de streaming de filmes              |
| 📑 Informações da Conta | `tenure`           | Tempo de permanência do cliente (meses)     |
| 📑 Informações da Conta | `Contract`         | Tipo de contrato do cliente                 |
| 📑 Informações da Conta | `PaperlessBilling` | Cliente utiliza fatura digital              |
| 📑 Informações da Conta | `PaymentMethod`    | Método de pagamento                         |
| 💰 Dados Financeiros    | `MonthlyCharges`   | Valor cobrado mensalmente                   |
| 💰 Dados Financeiros    | `TotalCharges`     | Valor total pago pelo cliente               |
| 🎯 Variável Alvo        | `Churn`            | Indica se o cliente cancelou o serviço      |

🎯 Interpretação da variável alvo
| Valor | Significado                   |
| ----- | ----------------------------- |
| `0`   | Cliente permaneceu na empresa |
| `1`   | Cliente cancelou o serviço    |



##⚙️ Tecnologias Utilizadas

Este projeto foi desenvolvido utilizando as seguintes ferramentas:

| Tecnologia                             | Descrição                                           |
| -------------------------------------- | --------------------------------------------------- |
| 🐍 **Python**                          | Linguagem principal utilizada para análise de dados |
| 📊 **Pandas**                          | Manipulação e tratamento de dados                   |
| 🔢 **NumPy**                           | Operações numéricas e manipulação de arrays         |
| 📈 **Matplotlib**                      | Criação de gráficos e visualizações de dados        |
| 🎨 **Seaborn**                         | Visualizações estatísticas mais avançadas           |
| 🌐 **Requests**                        | Coleta de dados através de requisições à API        |
| 📓 **Google Colab / Jupyter Notebook** | Ambiente interativo para desenvolvimento e análise  |


## 🔧 Etapas do Projeto

O projeto foi dividido em etapas típicas de um fluxo de Data Science.
| Etapa                                         | Descrição                                                                                                                                                                                                                                                                                                                                             |
| --------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 📥 **1. Ingestão de Dados**                   | ☑️ Coleta de dados via API<br>☑️ Conversão do JSON para DataFrame                                                                                                                                                                                                                                                                                     |
| 🔎 **2. Exploração Inicial**                  | ☑️ Análise da estrutura do dataset<br>☑️ Identificação das variáveis<br>☑️ Verificação de tipos de dados                                                                                                                                                                                                                                              |
| 🧹 **3. Limpeza e Tratamento (ETL)**          | ☑️ Tratamento de valores ausentes<br>☑️ Conversão de variáveis numéricas<br>☑️ Padronização de categorias<br>☑️ Transformação da variável **Churn** em binária                                                                                                                                                                                        |
| 📊 **4. Análise Exploratória de Dados (EDA)** | ☑️ 📊 Distribuição de churn<br>☑️ 📄 Churn por tipo de contrato<br>☑️ 👥 Churn por gênero, dependentes e parceiros<br>☑️ 💳 Churn por método de pagamento<br>☑️ 🌐 Churn por tipo de internet<br>☑️ ⏳ Tempo de contrato vs churn<br>☑️ 💰 Valor mensal vs churn<br>☑️ 🔗 Correlação entre variáveis numéricas<br>☑️ 🛡️ Churn por serviços adicionais |


## 📊 Principais Insights

A análise revelou padrões importantes sobre o comportamento dos clientes.

| Insight                                                     | Evidência Observada                                                                                                                                | Recomendação Estratégica                                                                              |
| ----------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------- |
| 📄 **Contratos mensais apresentam maior churn**             | Clientes com contratos **Month-to-Month** possuem taxas significativamente maiores de cancelamento em comparação com contratos anuais ou bienais.  | ➡ Incentivar contratos de longo prazo com benefícios ou descontos pode reduzir a evasão.              |
| ⏳ **Clientes novos cancelam mais**                          | A maior parte do churn ocorre nos **primeiros meses de contrato**, indicando maior risco no início da jornada do cliente.                          | ➡ Implementar **onboarding estruturado** e acompanhamento nos primeiros meses para aumentar retenção. |
| 💰 **Valores mensais mais altos aumentam o risco de churn** | Clientes com **MonthlyCharges mais elevados** apresentam maior probabilidade de cancelar o serviço.                                                | ➡ Avaliar a **percepção de custo-benefício dos planos** e oferecer alternativas mais atrativas.       |
| 🛡️ **Serviços adicionais reduzem churn**                   | Clientes que possuem serviços como **OnlineSecurity, TechSupport e DeviceProtection** apresentam taxas significativamente menores de cancelamento. | ➡ Oferecer **pacotes de serviços adicionais** pode aumentar o engajamento e reduzir churn.            |



## 🚀 Como Executar o Projeto
1️⃣ Clonar o repositório
```
git clone https://github.com/seu-usuario/telecom-churn-analysis.git
```

2️⃣ Instalar dependências
```
pip install pandas numpy matplotlib seaborn requests
```

3️⃣ Executar o notebook

Abra o notebook em:

Jupyter Notebook

Google Colab

Arquivo:
```
telecom_churn_analysis.ipynb
```


## 📈 Possíveis Melhorias Futuras

Este projeto pode ser expandido com novas análises e ferramentas para aprofundar a compreensão do churn e gerar previsões mais precisas.

| Categoria                    | Possível Melhoria                           | Descrição                                                                                                    |
| ---------------------------- | ------------------------------------------- | ------------------------------------------------------------------------------------------------------------ |
| 🤖 **Machine Learning**      | Modelos de previsão de churn                | Desenvolver modelos preditivos para identificar clientes com maior risco de cancelamento.                    |
| 🧠 **Algoritmos de ML**      | Logistic Regression, Random Forest, XGBoost | Aplicar diferentes algoritmos para comparar desempenho e identificar o modelo mais eficaz para prever churn. |
| 📊 **Dashboard Interativo**  | Power BI ou Streamlit                       | Criar dashboards interativos para facilitar a visualização e acompanhamento dos indicadores de churn.        |
| 🔍 **Análise de Features**   | Feature Importance                          | Identificar quais variáveis possuem maior influência na previsão de churn.                                   |
| 📉 **Métricas de Avaliação** | Acurácia, Recall, F1-score, ROC-AUC         | Avaliar o desempenho dos modelos utilizando métricas adequadas para problemas de classificação.              |


## 👩‍💻 Autora

Projeto desenvolvido por Kelly Costa como parte dos estudos em Data Science e Análise de Dados, com foco em análise exploratória de dados (EDA), visualização e geração de insights estratégicos.

⭐ Se este projeto foi útil para você, considere dar uma estrela no repositório para apoiar o trabalho!
