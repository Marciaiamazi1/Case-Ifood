# 📊 Case Técnico – Análise de Campanha iFood

Este repositório contém o desenvolvimento completo de um case técnico de análise de dados para o iFood. O objetivo foi avaliar o impacto de uma campanha de cupons sobre o comportamento dos usuários e propor recomendações com base em clusters identificados via machine learning.

---

## 🎯 Resumo do Projeto

- Análise de dados reais de pedidos e usuários
- Avaliação de impacto via teste A/B (grupo controle vs cuponado)
- Métricas avaliadas: **ticket médio** e **retenção**
- Segmentação dos usuários com **KMeans clustering**
- Geração de **gráficos interpretáveis**
- Recomendações estratégicas baseadas no perfil de cada cluster
- Entregável estruturado para facilitar **interpretação por lideranças**

---


---

## ▶️ Como acessar o notebook no Colab

Execute a análise diretamente no Google Colab:

[![Abrir no Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/SEU_USUARIO/case-ifood-analytics/blob/main/case/analise_ifood_ab_test.ipynb)

---

## 📈 Principais Resultados

- 📉 **Cupom sem impacto significativo no ticket médio**  
- 🔁 **Leve aumento de retenção (Target: 46,7%) – não significativo**
- 👥 **Três perfis distintos de usuários:**
  - Cluster 0: Gastadores pontuais (~R$115/ticket)
  - Cluster 1: Clientes frequentes (~3,7 pedidos)
  - Cluster 2: Pouco engajados (risco de churn)

---

## 💡 Recomendações por Cluster

| Cluster | Perfil                      | Estratégia sugerida                |
|--------|------------------------------|------------------------------------|
| 0      | Gastadores pontuais (VIP)    | Cupom exclusivo / benefícios premium |
| 1      | Clientes fiéis e recorrentes | Cashback por recorrência           |
| 2      | Pouco engajados              | Ofertas agressivas de reativação   |

---

## 💻 Bibliotecas utilizadas

- Python 3
- Google Colab
- Pandas, Seaborn, Matplotlib
- Scikit-learn (KMeans)
- Scipy (teste t para A/B)

---



