# 📊 Análise Completa – Case Técnico iFood

Este documento apresenta uma visão detalhada da análise realizada com base nos dados disponibilizados pelo iFood em um desafio técnico. A proposta envolve avaliar o impacto de uma campanha de cupons por meio de um teste A/B e segmentar os usuários com base no comportamento de pedidos e valor gasto.

---

## 🧠 1. Análise Descritiva dos Dados

### 🧾 Pedidos
- 3,6 milhões de pedidos analisados
- Período: dezembro/2018 a janeiro/2019
- Ticket médio geral: ~R$ 75,40

### 👥 Usuários
- 806 mil usuários registrados
- 61% de usuários ativos
- Distribuição concentrada em novos cadastros nos últimos 6 meses

### 🍽️ Restaurantes
- ~7.000 restaurantes únicos
- Média de ticket médio por restaurante: R$ 48,00
- Variação nos tempos de entrega e categorias de preço

---

## 🧪 2. Avaliação do Teste A/B

### 🎯 Objetivo
Analisar se o envio de cupons (grupo target) gerou impacto estatisticamente significativo frente ao grupo controle.

### 🧾 Métricas avaliadas

| Métrica            | Controle       | Target         | Resultado Estatístico     |
|--------------------|----------------|----------------|----------------------------|
| Ticket Médio       | R$ 76,12       | R$ 76,91       | **p = 0.71** (sem impacto) |
| Retenção (% 2+ pedidos) | 44,1%         | 46,7%         | **p = 0.22** (sem impacto) |

📌 **Conclusão**: A campanha de cupons **não gerou impacto estatisticamente relevante** no período analisado.

---

## 📈 3. Visualizações Geradas

- Gráficos salvos automaticamente na pasta `imagens/`
  - Boxplot: ticket médio por grupo
  - Barras: taxa de retenção
  - Histogramas de frequência de pedidos
  - Dispersão dos clusters

---

## 🔍 4. Clusterização de Usuários com KMeans

### 📊 Variáveis utilizadas:
- Número de pedidos por usuário
- Ticket médio individual

### 🔢 Clusters formados:

| Cluster | Perfil Comportamental      | Características principais            |
|---------|-----------------------------|----------------------------------------|
| 0       | Gastadores pontuais         | Ticket alto, poucos pedidos            |
| 1       | Clientes fiéis e frequentes | Pedem com frequência, ticket médio     |
| 2       | Usuários pouco engajados    | Ticket baixo, 1 pedido ou inativos     |

---

## 💡 5. Recomendações Estratégicas por Perfil

| Cluster | Estratégia Recomendável                            |
|---------|----------------------------------------------------|
| 0       | Cupons premium / Cashback personalizado            |
| 1       | Programa de fidelidade e recomendação inteligente  |
| 2       | Ofertas agressivas para reativação (push/email)    |

---

## 📌 Conclusão Geral

- O teste A/B não mostrou impacto relevante
- A segmentação revelou padrões de consumo distintos
- A personalização por perfil tem alto potencial de otimizar campanhas
- Próximo passo sugerido: **novo teste A/B segmentado por cluster**

---


