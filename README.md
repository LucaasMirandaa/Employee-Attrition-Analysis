# Employee Attrition Analysis

Solução ponta a ponta de analytics e machine learning projetada para diagnosticar a rotatividade de colaboradores (attrition), identificar fatores críticos de risco e prever a probabilidade de desligamento de funcionários.

---
### Arquitetura de Dados Medalhão
Os dados são processados de forma incremental através de três camadas para garantir a governança e integridade da informação:
* **Bronze**: Armazenamento dos dados brutos originais (`HR_Analytics.csv`) preservando o estado inicial de captura.
* **Silver**: Processo de limpeza, tratamento de valores nulos, conversão de tipos e padronização.
* **Gold**: Tabelas agregadas e preparadas especificamente para o consumo analítico (BI) e treinamento dos modelos de machine learning.

### Engenharia de Recursos e Modelagem Preditiva
* **Fatores de Impacto**: Análise das variáveis mais correlacionadas ao atrito de pessoal, tais como horas extras (*OverTime*), distância da residência (*DistanceFromHome*), nível do cargo (*JobLevel*) e satisfação com o ambiente de trabalho (*EnvironmentSatisfaction*).
* **Modelagem Supervisionada**: Comparação e otimização de algoritmos classificadores como Random Forest, Regressão Logística e XGBoost.
* **Métricas de Avaliação**: Ajuste fino focado no equilíbrio entre Precisão e Sensibilidade (Recall), buscando mitigar falsos negativos na identificação de colaboradores em risco.

---

## Pontos do Projeto

* **Integração Ponta a Ponta**: Ciência de dados aplicada (Jupyter Notebooks) e visualização de dados estratégica (Power BI).
* **Foco em Valor de Negócio**: Tradução de padrões estatísticos complexos em indicadores de risco objetivos para subsidiar planos de retenção do setor de Recursos Humanos.
* **Estrutura Modular**: Arquitetura de código em `/src` projetada de forma modular e reutilizável, facilitando a automação e manutenção do pipeline.
* **Processamento Reprodutível**: Fluxo estruturado que garante que todas as transformações de dados sejam determinísticas e auditáveis de ponta a ponta.

---

## Estrutura de Diretórios

```
├── data/
│   ├── bronze/      # Dataset original bruto
│   ├── silver/      # Dados limpos e tratados
│   └── gold/        # Tabelas agregadas e otimizadas
├── notebooks/       # Jupyter Notebooks para análise exploratória (EDA)
└── src/             # Scripts e módulos reutilizáveis (ETL, Modelagem, Utils)
```
