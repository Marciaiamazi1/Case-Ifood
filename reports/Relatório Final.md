# 📊 Case iFood – Análise de Dados com Teste A/B e Segmentação Comportamental

## 🧠 Contexto

O iFood, líder em delivery na América Latina, lançou uma campanha de cupons com o objetivo de aumentar a retenção de usuários e incentivar novos pedidos. Para validar sua eficácia, foi conduzido um **Teste A/B**, com divisão entre grupo controle (sem cupom) e grupo teste (com cupom).

Este projeto teve como objetivo avaliar o impacto da campanha com base em métricas de comportamento e propor **ações personalizadas por segmento de usuário**, usando dados reais.

---

## 🔍 O que foi analisado

- 📊 Análise descritiva de pedidos, usuários e restaurantes
- 🧪 Avaliação do impacto da campanha via **Teste A/B**, comparando:
  - Ticket médio por usuário (teste de hipótese)
  - Taxa de retenção (usuários que fizeram +1 pedido)
- 🧬 Segmentação de clientes com **K-Means**, baseada em:
  - Frequência de pedidos
  - Ticket médio individual
- 🧠 Interpretação dos clusters com perfis comportamentais
- 🎯 Geração de **recomendações estratégicas por perfil**, com foco em:
  - Personalização de campanhas
  - Eficiência dos incentivos
  - Otimização de investimento em marketing

---

## 🛠️ Ferramentas e Técnicas

| Tecnologia        | Aplicação                                     |
|-------------------|-----------------------------------------------|
| Python (Google Colab) | Ambiente de análise e prototipagem      |
| Pandas            | Manipulação e tratamento de dados             |
| Seaborn / Matplotlib | Visualizações e gráficos analíticos      |
| Scikit-learn      | Algoritmo K-Means para clusterização          |
| Scipy             | Testes estatísticos (teste de hipóteses)      |

---

## 📦 Entregáveis

- ✅ Notebook interativo (Colab) com todo o processo analítico
- ✅ Relatório visual (PDF) com insights e recomendações
- ✅ Arquivos de dados tratados e organizados
- ✅ Estrutura documentada neste `README.md`

---

## 🎯 Conclusões

- O impacto da campanha variou significativamente conforme o perfil de usuário.
- Campanhas genéricas tendem a diluir os resultados; segmentação é essencial.
- A personalização estratégica pode aumentar a eficiência e reduzir custos promocionais.

> Estima-se que a reativação de 10% dos clientes inativos represente até **R$ 1,2 milhão/mês em pedidos adicionais**, considerando um ticket médio de R$ 50 e 240 mil usuários inativos.

---

📎 *Este case foi desenvolvido como exercício de análise exploratória, segmentação e tomada de decisão orientada por dados. Para detalhes técnicos, consulte o notebook no repositório.*

---








