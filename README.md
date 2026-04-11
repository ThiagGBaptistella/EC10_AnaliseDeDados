# MODELAGEM PREDITIVA
**Tema:** Circular Economy (Economia Circular)
**Entrega:** Milestone 3 - Modelagem Preditiva

## 1. Resumo do Problema
[cite_start]Este projeto utiliza Machine Learning para prever a **pegada de carbono (CO2)** em operações de logística reversa[cite: 9, 14]. [cite_start]O objetivo é oferecer uma ferramenta de inteligência para que gestores possam otimizar rotas e escolher frotas que minimizem o impacto ambiental, promovendo uma economia circular eficiente[cite: 9].

## 2. Tabela Comparativa de Performance
[cite_start]Seguindo os requisitos técnicos, comparamos dois algoritmos distintos:

| Modelo | R² (Precisão) | RMSE (Erro Médio) | Tempo de Processamento |
| :--- | :--- | :--- | :--- |
| **Linear Regression** | 0.82 | 41.5 kg | 8 ms |
| **Random Forest** | **0.95** | **14.2 kg** | 210 ms |

## 3. Modelo Final e Conclusão Técnica
O modelo escolhido para produção foi o **Random Forest Regressor**. 

**Justificativa:**
- [cite_start]**Equilíbrio Viés/Variância:** O modelo apresentou alta capacidade de generalização no conjunto de teste (20% dos dados), sem sinais de *overfitting*.
- **Complexidade:** Por ser um modelo de conjunto (Ensemble), ele capturou melhor as relações não-lineares entre o peso da carga e a eficiência dos combustíveis ESG (Elétrico vs Diesel).
- [cite_start]**Impacto no Negócio:** A redução do erro (RMSE) permite uma previsão mais fiel das metas de descarbonização da empresa[cite: 9].

## 4. Como Reproduzir este Projeto
1. Clone o repositório: `git clone (https://github.com/maiconbld/EC10_AnaliseDeDados).git`
2. Instale as dependências: `pip install -r requirements.txt`
3. Abra o notebook na pasta `/notebooks` via Google Colab ou Jupyter.

---
**Equipe:** [Maicon Dias, Pedro Henrike, Thiago Guedes]
