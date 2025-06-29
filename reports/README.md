# 📊 Case Técnico de Data Analytics – iFood

Este projeto apresenta a análise de uma campanha de cupons do iFood realizada via teste A/B. A solução explora os efeitos da campanha sobre o comportamento dos usuários (ticket médio e retenção), além de aplicar uma segmentação via KMeans para propor estratégias personalizadas e sustentáveis.

---

## 🎯 Objetivo

Avaliar os efeitos de uma campanha promocional de cupons do iFood a partir de um teste A/B, examinando:

- Diferença no ticket médio por grupo
- Mudança na taxa de retenção
- Perfis de comportamento entre usuários
- Recomendação de estratégias por segmento

---

## 📂 Estrutura do Repositório


---

## ▶️ Execução

1. Acesse o notebook completo no Google Colab:

   [![Abrir no Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/SEU_USUARIO/SEU_REPOSITORIO/blob/main/analise_ifood_ab_test.ipynb)

2. Execute as células passo a passo. Os gráficos são salvos automaticamente na pasta `imagens/`.

---

## 📈 Resultados Visuais

### 🎟️ Ticket Médio por Grupo

![Ticket Médio](imagens/ticket_medio_por_grupo.png)

💡 O grupo que recebeu cupom (target) **não apresentou aumento significativo** no valor médio dos pedidos em relação ao grupo controle.  
📌 *p-valor do teste t ≈ 0.7083*

---

### 🔁 Retenção por Grupo

![Retenção](imagens/retencao_por_grupo.png)

💡 O grupo que recebeu cupom apresentou uma taxa de retenção ligeiramente superior (46,7%) comparado ao grupo controle (44,1%), porém **a diferença não é estatisticamente significativa**.

---

### 👥 Segmentação com K-Means

![Clusters](imagens/segmentacao_kmeans_scatter.png)

**Cluster 0:** Gastadores pontuais – ticket médio elevado, baixa frequência  
**Cluster 1:** Clientes recorrentes – baixo ticket médio, alta frequência  
**Cluster 2:** Pouco engajados – baixo ticket e baixa frequência

---

## 💡 Recomendações Estratégicas

Com base nos dados e clusters comportamentais:

| Segmento         | Estratégia recomendada                  |
|------------------|------------------------------------------|
| Cluster 0 (VIP)  | Benefício premium, cupom de fidelidade   |
| Cluster 1 (Fiel) | Cashback por recorrência                |
| Cluster 2 (Churn)| Cupom agressivo de reativação           |

**Outros testes sugeridos:**
- Testar frete grátis, cashback e descontos percentuais
- Avaliar o impacto de notificações personalizadas
- Medir ROI por segmento no próximo experimento

---

## 💸 Estimativa de impacto

Se recuperarmos 30.000 clientes do Cluster 2 com ticket médio de R$40:

📈 Receita potencial: **R$1.200.000**

---

## 💻 Tecnologias utilizadas

- Python 3 + Google Colab
- Pandas, Seaborn, Matplotlib
- Scikit-learn (KMeans)
- Scipy (teste t de hipótese)

---

## 📄 Licença

Este projeto foi desenvolvido para fins de estudo e avaliação técnica.  
🔐 Uso educacional e não comercial.  
👤 Criado por Paula | Julho/2025

