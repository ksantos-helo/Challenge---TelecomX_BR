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

O conjunto de dados contém informações sobre clientes da Telecom X, incluindo:

👥 Dados Demográficos

✔️gender

✔️SeniorCitizen

✔️Partner

✔️Dependents

📡 Serviços Contratados

✔️PhoneService

✔️MultipleLines

✔️InternetService

✔️OnlineSecurity

✔️OnlineBackup

✔️DeviceProtection

✔️TechSupport

✔️StreamingTV

✔️StreamingMovies

📑 Informações da Conta

✔️tenure (tempo como cliente)

✔️Contract

✔️PaperlessBilling

✔️PaymentMethod

💰 Dados Financeiros

✔️MonthlyCharges

✔️TotalCharges

🎯 Variável alvo

✔️Churn

0 → cliente permaneceu

1 → cliente cancelou

## ⚙️ Tecnologias Utilizadas

Este projeto foi desenvolvido utilizando as seguintes ferramentas:

✔️🐍 Python

✔️📊 Pandas

✔️🔢 NumPy

✔️📈 Matplotlib

✔️🎨 Seaborn

✔️🌐 Requests

✔️📓 Google Colab / Jupyter Notebook

## 🔧 Etapas do Projeto

O projeto foi dividido em etapas típicas de um fluxo de Data Science.

1️⃣ Ingestão de Dados

☑️Coleta de dados via API

☑️Conversão do JSON para DataFrame

2️⃣ Exploração Inicial

☑️Análise da estrutura do dataset

☑️Identificação de variáveis

☑️Verificação de tipos de dados

3️⃣ Limpeza e Tratamento (ETL)

☑️Tratamento de valores ausentes

☑️Conversão de variáveis numéricas

☑️Padronização de categorias

☑️Transformação da variável Churn em binária

4️⃣ Análise Exploratória de Dados (EDA)

Foram analisados diversos aspectos do comportamento dos clientes:

☑️📊 Distribuição de churn

☑️📄 Churn por tipo de contrato

☑️👥 Churn por gênero, dependentes e parceiros

☑️💳 Churn por método de pagamento

☑️🌐 Churn por tipo de internet

☑️⏳ Tempo de contrato vs churn

☑️💰 Valor mensal vs churn

☑️🔗 Correlação entre variáveis numéricas

☑️🛡️ Churn por serviços adicionais

## 📊 Principais Insights

A análise revelou padrões importantes sobre o comportamento dos clientes.

📄 Contratos mensais apresentam maior churn

Clientes com contratos month-to-month possuem taxas de cancelamento significativamente maiores.

➡ Incentivar contratos anuais pode reduzir a evasão.

⏳ Clientes novos cancelam mais

Grande parte dos cancelamentos ocorre nos primeiros meses de contrato.

➡ Melhorar o onboarding do cliente pode aumentar retenção.

💰 Valores mensais mais altos aumentam o risco de churn

Clientes com MonthlyCharges mais altos apresentam maior tendência a cancelar.

➡ Avaliar percepção de custo-benefício dos planos.

🛡️ Serviços adicionais reduzem churn

Clientes com serviços como:

OnlineSecurity

TechSupport

DeviceProtection

apresentam taxas muito menores de cancelamento.

➡ Oferecer pacotes de serviços adicionais pode aumentar retenção.

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

Este projeto pode ser expandido com:

👉🤖 Modelos de Machine Learning para previsão de churn

👉📊 Dashboard interativo com Power BI ou Streamlit

👉🔍 Análise de feature importance

🧠 Modelos como:

👉Logistic Regression

👉Random Forest

👉XGBoost

## 👩‍💻 Autor

Projeto desenvolvido como parte de estudos em Data Science e Análise de Dados.

⭐ Se este projeto foi útil para você, considere dar uma estrela no repositório!
