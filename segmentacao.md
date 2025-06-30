# 🧬 Análise de Segmentação – Teste A/B iFood

Este documento detalha a criação e aplicação de segmentações comportamentais para a análise do Teste A/B realizado com usuários da plataforma iFood.

---

## ✅ a) Segmentações Definidas

Foram definidas três dimensões principais de segmentação para avaliar a eficácia da campanha de cupons:

1. **Frequência de Pedidos**
   - Alta frequência: clientes recorrentes
   - Média frequência
   - Baixa frequência: novos ou pouco engajados

2. **Ticket Médio por Pedido**
   - Alto ticket: > R$90  
   - Médio ticket: R$60–90  
   - Baixo ticket: < R$60

3. **Recência**
   - Ativos recentes: últimos 10 dias  
   - Moderadamente ativos: 11 a 30 dias  
   - Inativos: mais de 30 dias sem pedidos

Essas dimensões combinadas possibilitam identificar padrões de comportamento e sensibilidade à campanha.

---

## ✅ b) Critérios e Ferramentas Utilizadas

| Variável      | Faixas Definidas                   | Racional                                                             |
|---------------|------------------------------------|----------------------------------------------------------------------|
| Frequência    | Quantidade de pedidos por cliente  | Define engajamento atual                                             |
| Ticket Médio  | Valor médio gasto por pedido       | Avalia potencial de monetização e sensibilidade à promoção           |
| Recência      | Dias desde o último pedido         | Indica risco de churn e chance de reativação                        |

**Ferramentas e abordagens:**

- Análise exploratória com distribuições e percentis  
- Clusterização com algoritmo `KMeans` (3 a 4 grupos)  
- Visualizações (scatterplots) para interpretação e validação dos clusters  

📌 *Exemplo:*  
Clientes com alta frequência, ticket médio e recência baixa → *Possivelmente engajados e responsivos a incentivos de fidelidade (não necessariamente cupons)*

---

## ✅ c) Resultados do Teste A/B por Segmento

A análise cruzada entre os segmentos e os grupos de Teste A/B revelou que:

- **Baixa frequência + alta recência:** houve leve aumento na taxa de segundo pedido com cupom, **mas sem significância estatística**.
- **Alto ticket médio:** o cupom **não apresentou impacto relevante** — possivelmente esse grupo valoriza mais a experiência do que o desconto.
- **Baixo ticket + média frequência:** observou-se **pequeno aumento no ticket médio** entre os usuários impactados, sugerindo **boa resposta à percepção de valor**.

🔎 *Conclusão:*  
Campanhas aplicadas de forma uniforme **diluem o impacto real**. Os efeitos variam significativamente conforme o perfil do usuário.

---

## 🚀 d) Recomendações Estratégicas

### 1. **Campanhas direcionadas por perfil**
- **Clientes inativos/pouco engajados:** reativação com **descontos fortes**
- **Clientes fiéis:** programa de **fidelidade ou cashback**
- **Clientes premium:** **benefícios exclusivos não monetários** (ex: entrega prioritária)

> 🎯 **Impacto estimado:**  
> Aumentar a retenção em 10% entre clientes inativos pode representar **~R$ 1,2 milhão/mês** em pedidos adicionais (base: ticket médio R$50 e 240 mil usuários).

### 2. **Refinamento do Teste A/B**
- Aplicar testes controlados por cluster
- Analisar a eficácia da campanha por grupo segmentado

### 3. **Automatização de Segmentações**
- Implementar pipeline mensal com atualização dos clusters
- Integrar as segmentações aos fluxos da área de Marketing e CRM

---

🧠 *Essas ações não apenas aumentam o retorno financeiro, mas também elevam a precisão das campanhas e otimizam recursos da operação.*




