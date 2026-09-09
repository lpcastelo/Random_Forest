# Random_Forest
Aqui você irá encontrar a atividade do módulo 32 do curso de Cientista de Dados da Ebac.

A atividade consiste em aplicar o modelo de Machine Learning Random Forest para problemas de classificação, além de realizar o ajuste e otimização dos hiperparâmetros do modelo.

Durante a atividade serão abordados temas como:

* Modelo Random Forest
* Classificação supervisionada
* Treinamento e avaliação de modelos
* Ajuste de hiperparâmetros
* Utilização do RandomizedSearchCV
* Comparação e melhoria de desempenho do modelo

O objetivo é compreender o funcionamento do algoritmo Random Forest e aprender técnicas de otimização que permitem melhorar a performance e a capacidade preditiva dos modelos de Machine Learning.

## Dados

Base `winequality-red.csv` (1.599 vinhos), com características físico-químicas (acidez, açúcar residual, cloretos, sulfatos, álcool, etc.) e variável alvo multiclasse `quality` (notas de 3 a 8), fortemente desbalanceada — as notas 5, 6 e 7 concentram mais de 94% das amostras.

## Resultados

O modelo Random Forest alcançou **69% de acurácia**, com bom desempenho nas classes majoritárias (5 e 6) mas **nenhum acerto nas classes minoritárias (3 e 4)**. A otimização de hiperparâmetros via `RandomizedSearchCV` (100 combinações, 5-fold) **não trouxe melhora** — acurácia permaneceu em 69%, confirmando que o principal fator limitante é o forte desbalanceamento da variável alvo, não a configuração do modelo.

## Tecnologias

- Python, pandas, numpy
- scikit-learn (RandomForestClassifier, RandomizedSearchCV, métricas)
- matplotlib, seaborn

## Como executar

1. Instale as dependências: `pip install pandas numpy scikit-learn matplotlib seaborn`.
2. Coloque `winequality-red.csv` no mesmo diretório do notebook.
3. Execute `Cientista de Dados Pratique M32.ipynb` em ordem (a etapa de `RandomizedSearchCV` pode demorar alguns minutos).
