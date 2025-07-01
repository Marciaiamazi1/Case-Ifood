#  Teste A/B e Segmentação Comportamental

##  Contexto

O iFood, líder em delivery na América Latina, lançou uma campanha de cupons com o objetivo de aumentar a retenção de usuários e incentivar novos pedidos. Para validar sua eficácia, foi conduzido um **Teste A/B**, com divisão entre grupo controle (sem cupom) e grupo teste (com cupom).

Este projeto teve como objetivo avaliar o impacto da campanha com base em métricas de comportamento e propor **ações personalizadas por segmento de usuário**, usando dados reais.

---

##  Análise

-  Análise descritiva de pedidos, usuários e restaurantes

-  Avaliação do impacto da campanha via **Teste A/B**, comparando:
  
   - Ticket médio por usuário (teste de hipótese)
   - Taxa de retenção (usuários que fizeram +1 pedido)
       
-  Segmentação de clientes com **K-Means**, baseada em:
   - Frequência de pedidos
   - Ticket médio individual
     
-  Interpretação dos clusters com perfis comportamentais
-  Geração de **recomendações estratégicas por perfil**, com foco em:
  - Personalização de campanhas
  - Eficiência dos incentivos
  - Otimização de investimento em marketing

---

##  Etapas 

| Etapa                             | Descrição                                                                                                    |
|----------------------------------|----------------------------------------------------------------------------------------------------------------|
| **1. Análise Descritiva**        | Exploração inicial dos dados de pedidos, usuários e restaurantes, com foco em padrões de consumo e engajamento. |
| **2. Avaliação de Impacto – Teste A/B** | Comparação entre grupo controle e grupo testado em duas frentes:<br>• Ticket médio por usuário (com teste de hipótese)<br>• Taxa de retenção (usuários que realizaram mais de um pedido) |
| **3. Segmentação com K-Means**   | Clusterização baseada em dois parâmetros-chave:<br>• Frequência de pedidos<br>• Ticket médio individual por usuário |
| **4. Interpretação Comportamental** | Análise qualitativa dos clusters gerados, com atribuição de rótulos e perfis comportamentais para orientar decisões. |
| **5. Recomendações Estratégicas por Perfil** | Ações sugeridas para cada tipo de usuário:<br>• Personalização de campanhas promocionais<br>• Aumento da eficiência dos incentivos<br>• Otimização do investimento em marketing com foco em ROI |

---

##  Ferramentas e Técnicas

| Tecnologia        | Aplicação                                     |
|-------------------|-----------------------------------------------|
| Python (Google Colab) | Ambiente de análise e prototipagem      |
| Pandas            | Manipulação e tratamento de dados             |
| Seaborn / Matplotlib | Visualizações e gráficos analíticos      |
| Scikit-learn      | Algoritmo K-Means para clusterização          |
| Scipy             | Testes estatísticos (teste de hipóteses)      |

---

##  Entregáveis

-  Notebook interativo com todo o processo analítico (Google Colab)
-  Relatório visual (PDF) com insights e recomendações
-  Arquivos de dados tratados e organizados
-  Estrutura documentada neste `README.md`

---

##  Conclusões

- O impacto da campanha variou significativamente conforme o perfil de usuário.
- Estratégias genéricas tendem a diluir resultados e aumentar custos.
- A personalização orientada por dados melhora a **eficiência de campanhas**, reduz desperdício e potencializa ROI.

>  Estimativa: reativar 10% da base inativa pode gerar até **R$ 1,2 milhão/mês** em novos pedidos, com ticket médio de R$ 50 e 240 mil usuários inativos.

---

 *Para detalhes técnicos, consulte o notebook e os gráficos no repositório.*


---








