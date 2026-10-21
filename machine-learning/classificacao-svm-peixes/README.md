# Classificação Morfológica de Peixes com Support Vector Machines (SVM)

Este projeto aplica técnicas de Machine Learning para classificar a família de peixes com base em suas características morfológicas. Foi desenvolvido com foco em boas práticas de Engenharia de Software, código limpo e prevenção de vieses de dados.

## Objetivo
Construir um pipeline robusto de classificação utilizando a biblioteca `scikit-learn`, passando por todas as etapas: desde a ingestão automatizada de dados até a otimização de hiperparâmetros.

## Tecnologias e Ferramentas
*   **Linguagem:** Python
*   **Manipulação de Dados:** Pandas, NumPy
*   **Visualização:** Matplotlib, Seaborn
*   **Machine Learning:** Scikit-Learn (SVM, GridSearchCV, StandardScaler)
*   **Ingestão:** Kagglehub

## Destaques Técnicos do Projeto
*   **Automação de Ingestão:** Download direto via API do Kaggle para garantir reprodutibilidade.
*   **Tratamento de Dados:** Remoção de duplicatas, tratamento de nulos (imputação pela média) e filtragem de classes sub-representadas (Long Tail).
*   **Prevenção de Data Leakage:** Separação estrita de escalonamento (StandardScaler) entre conjuntos de treino e teste.
*   **Otimização:** Uso de `GridSearchCV` com Validação Cruzada (K-Fold cv=5) e processamento paralelo (`n_jobs=-1`) testando 64 combinações de hiperparâmetros (Kernel, C e Gamma).

## Autor
Felipe Pontes - *Estudante de Engenharia de Software*
