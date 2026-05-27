# MODELAGEM PREDITIVA
**Tema:** Circular Economy (Economia Circular)
**Entrega:** Milestone 3 - Modelagem Preditiva

## 1. Resumo do Problema e Objetivos
Este projeto desenvolve uma solução de Business Analytics hospedada no Google Colab para resolver desafios de rastreabilidade de pegada de carbono e eficiência logística. O objetivo desta Milestone (M3) foi implementar, treinar e validar modelos de Machine Learning para prever as emissões de $CO_2$ em operações de logística reversa, transformando dados brutos em inteligência para tomada de decisão estratégica.

## 2. Metodologia de Modelagem
A fase de modelagem seguiu o ciclo completo de ciência de dados conforme os requisitos técnicos:
* **Pré-processamento**: Aplicação de *One-Hot Encoding* para variáveis categóricas de frota e *StandardScaler* para normalização de variáveis numéricas.
* **Divisão de Dados**: Separação rigorosa entre conjuntos de treino (80%) e teste (20%) para garantir a validade estatística dos resultados.
* **Algoritmos**: Implementação comparativa entre modelos lineares e modelos de conjunto baseados em árvores (Random Forest).

## 3. Relatório de Performance (Tabela Comparativa)
Abaixo, os resultados obtidos na validação dos modelos, destacando a superioridade do algoritmo selecionado:

| Métrica | Linear Regression | **Random Forest (Escolhido)** |
| :--- | :--- | :--- |
| **RMSE** (Erro Médio Quadrático) | 1530.96 | **614.91** |
| **MAE** (Erro Médio Absoluto) | 1097.67 | **292.25** |
| **$R^2$** (Precisão) | 0.6881 | **0.9496** |
| **Tempo de Processamento** | 40.53 ms | 468.69 ms |

## 4. Conclusão Técnica e Escolha do Modelo
O algoritmo **Random Forest Regressor** foi selecionado para a solução final.

* **Equilíbrio Viés e Variância**: O modelo apresentou um $R^2$ de aproximadamente **0.95**, indicando que a inteligência explica 95% da variabilidade das emissões de $CO_2$ nos dados de teste, sem sinais de *overfitting*.
* **Complexidade**: Por ser um modelo *Ensemble*, o Random Forest capturou com precisão as relações não-lineares entre peso da carga, distância e tipo de combustível ESG.
* **Impacto no Negócio**: A redução de mais de 50% no erro médio (RMSE) em relação ao baseline permite previsões confiáveis para metas de descarbonização e retorno sobre investimento (ROI) em logística circular.

## 5. Estrutura do Repositório
* `/notebooks`: Notebook Python (.ipynb) com o ciclo completo de modelagem.
* `/models`: Modelo final exportado (`modelo_final.joblib`).
* `requirements.txt`: Lista de bibliotecas utilizadas (pandas, scikit-learn, joblib).
* `README.md`: Documentação executiva do projeto.

## 6. Instruções de Reprodução
1. Clone este repositório: `git clone https://github.com/maiconbld/EC10_AnaliseDeDados.git`
2. Instale as dependências necessárias: `pip install -r requirements.txt`
3. Execute o notebook presente na pasta `/notebooks` para visualizar o treinamento e a validação.

---
**Equipe (Grupo 03 - Circular Economy):**
* Maicon Dias 082210032
* Pedro Henrike 082210025
* Thiago Guedes 082210010
  
