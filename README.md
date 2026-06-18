# Employee Attrition Analysis & HR Analytics

<div align="center">
  
  [![GitHub License](https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge)](LICENSE)
  [![Python](https://img.shields.io/badge/Python-3.9+-blue.svg?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org)
  [![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=power-bi&logoColor=black)](https://powerbi.microsoft.com)
  [![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org)
  [![Jupyter Notebook](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org)

  <p align="center">
    <strong>Uma solução ponta a ponta em ciência de dados para entender a rotatividade de talentos, identificar fatores de risco e fornecer insights acionáveis para o setor de Recursos Humanos.</strong>
  </p>

  ---

  **Status do Projeto:** *Em Desenvolvimento / Construção* 
  
</div>

---

## Data Visualization & Dashboard Interativo

Como primeira etapa fundamental deste projeto, foi desenvolvido um dashboard interativo no **Power BI** utilizando o dataset de HR Analytics. Este painel permite explorar os principais indicadores de rotatividade (Attrition), facilitando a tomada de decisão estratégica pelas lideranças de Recursos Humanos.

Você pode interagir diretamente com o relatório abaixo:

<div align="center" style="margin: 25px 0;">
  <iframe title="HR Analytics Dashboard" width="100%" height="541.25" src="https://app.powerbi.com/reportEmbed?reportId=df046530-7bf9-45e7-84f5-49835a33f354&autoAuth=true&ctid=da49a844-e2e3-40af-86a6-c3819d704f49" frameborder="0" allowFullScreen="true" style="max-width: 1140px; border-radius: 8px; box-shadow: 0 4px 15px rgba(0,0,0,0.15);"></iframe>
</div>

---

## Sobre o Projeto & Contexto de Negócio

A rotatividade de funcionários (ou *employee attrition*) representa um dos desafios mais custosos e complexos para qualquer organização. Além dos custos financeiros de demissão, recrutamento e treinamento, a perda de talentos-chave impacta a produtividade, a moral das equipes e a retenção do conhecimento institucional.

### **Objetivos Principais**
1. **Identificar Perfis de Risco:** Descobrir as variáveis demográficas e corporativas mais correlacionadas com a saída de funcionários.
2. **Análise de Fatores Críticos:** Investigar o impacto de horas extras (*OverTime*), distância do trabalho (*DistanceFromHome*), nível de cargo (*JobLevel*) e satisfação com o ambiente de trabalho (*EnvironmentSatisfaction*).
3. **Engenharia de Dados (Medalhão):** Implementar um pipeline limpo que move os dados da camada Bronze (brutos) até a Gold (prontos para consumo).
4. **Machine Learning Preditivo:** Desenvolver um classificador supervisionado para prever a probabilidade de um colaborador deixar a empresa.

---

## Estrutura e Arquitetura de Dados

O projeto segue a arquitetura **Medallion (Bronze/Silver/Gold)** para garantir a integridade, reprodutibilidade e governança dos dados trabalhados:

```
📁 Employee Attrition Analysis/
├── 📁 data/                  # Estrutura de armazenamento de dados
│   ├── 📁 bronze/            # Dados brutos originais (HR_Analytics.csv)
│   ├── 📁 silver/            # Dados limpos e pré-processados (em desenvolvimento)
│   └── 📁 gold/              # Tabelas agregadas e otimizadas para BI/Modelagem (em desenvolvimento)
├── 📁 notebooks/             # Jupyter Notebooks de desenvolvimento
│   └── 📓 01_eda.ipynb       # Análise Exploratória de Dados (EDA)
├── 📁 src/                   # Módulos Python reutilizáveis (ETL, Modelagem, Utils)
├── 📁 venv/                  # Ambiente virtual Python
└── 📝 README.md              # Documentação do projeto (este arquivo)
```

---

## Tecnologias & Ferramentas Utilizadas

* **Business Intelligence:**
  * **Power BI & DAX:** Criação de métricas, e visualizações de dados interativas.
* **Ciência & Engenharia de Dados (Python):**
  * **Pandas:** Manipulação de dados e engenharia de recursos.
  * **Matplotlib & Seaborn:** Geração de gráficos estatísticos durante a análise exploratória.
  * **Jupyter Notebook:** Prototipagem rápida e análise iterativa dos dados.

---

## Roadmap de Desenvolvimento

Abaixo estão listadas as etapas concluídas e o cronograma para as próximas fases do projeto:

* [x] **Fase 1: Ingestão de Dados & Estruturação**
  * Configuração da estrutura de pastas.
  * Armazenamento do dataset original na camada `bronze`.
* [x] **Fase 2: Business Intelligence**
  * Modelagem dos dados para dashboard.
  * Criação do relatório interativo no Power BI e incorporação no portfólio.
* [/] **Fase 3: Análise Exploratória (EDA)**
  * Análise estatística descritiva no notebook `notebooks/01_eda.ipynb`.
  * Identificação de correlações e padrões iniciais de atrito.
* [ ] **Fase 4: Pipeline de Engenharia (Bronze -> Silver -> Gold)**
  * Criação de scripts em Python para limpeza e tratamento de dados.
  * Feature Engineering para criação de novas variáveis relevantes.
* [ ] **Fase 5: Modelagem Preditiva (Machine Learning)**
  * Treinamento de algoritmos supervisionados (como Random Forest, Regressão Logística e XGBoost).
  * Otimização de hiperparâmetros e validação de métricas de avaliação (Precisão, Recall, F1-Score).
* [ ] **Fase 6: Implantação & Web App**
  * Desenvolvimento de uma aplicação web (Streamlit ou similar) para permitir que gestores simulem cenários de risco de rotatividade em tempo real.

---


