# Case Técnico de Data Analytics - IFood

O iFood, líder em delivery de alimentos na América Latina, realizou uma campanha de cupons com o intuito de incentivar novos pedidos e aumentar a retenção de clientes. Para validar a efetividade da iniciativa, foi realizado um teste A/B , em que parte dos usuários recebeu o benefício (grupo "target") e outra parte não (grupo "controle").

O desafio analítico consistiu em avaliar se a campanha teve impacto significativo nas métricas de comportamento dos usuários e, a partir disso, propor recomendações personalizadas com base em segmentações comportamentais.



##  Análises realizadas
- Análise de conversão entre grupo controle e grupo cupom (teste A/B)

- Segmentação de usuários com base em comportamento e ticket médio

- Avaliação de viabilidade financeira dos cupons (ROI)

- Criação de gráficos para suporte às conclusões

##  Etapas 

| Etapa                             | Descrição                                                                                                    |
|----------------------------------|----------------------------------------------------------------------------------------------------------------|
| **1. Análise Descritiva**        | • Exploração inicial dos dados de pedidos, usuários e restaurantes, com foco em padrões de consumo e engajamento. |
| **2. Avaliação de Impacto – Teste A/B** | • Ticket médio por usuário (com teste de hipótese)<br>• Taxa de retenção (usuários que realizaram mais de um pedido) |
| **3. Segmentação com K-Means**   | • Frequência de pedidos<br>• Ticket médio individual por usuário |
| **4. Interpretação Comportamental** | • Análise qualitativa dos clusters gerados, com atribuição de rótulos e perfis comportamentais para orientar decisões. |
| **5. Recomendações Estratégicas por Perfil** |• Personalização de campanhas promocionais<br>• Aumento da eficiência dos incentivos<br>• Otimização do investimento em marketing com foco em ROI |

---
## Avaliação do Teste A/B
Analisar o envio de cupons (grupo alvo) gerou impacto estatisticamente significativo frente ao grupo controle.

| Métrica                       | Controle   | Alvo      | Resultado Estatístico  |
|-------------------------------|------------|-----------|------------------------|
| **Bilhete Médio**              | R$ 76,12   | R$ 76,91  | p = 0,71 (sem impacto)  |
| **Retenção (% 2+ Pedidos)**   | 44,1%      | 46,7%     | p = 0,22 (sem impacto)  |

 **Conclusão**: A campanha de cupons não gerou impacto estatisticamente relevante no período analisado.


---
##  Como Executar o repositório
1. Clone este repositório:
 https://github.com/Marciaiamazi1/Case-Ifood.git

2. Abra os arquivos contidos na pasta notebook no Jupyter ou Google Colab para visualizar as análises realizadas e explorar os resultados.

---


## Estrutura de Arquivos
- `case`:  Scripts e códigos principais
- `dados`: Dados utilizados para a análise
- `imagens`: Imagens geradas durante a análise (gráficos, diagramas)
- `notebook`: Análises interativas
- `README:`Arquivo, com explicações detalhadas do projeto




---



## Bibliotecas e tecnologias utilizadas

| Tecnologia                | Finalidade Principal                              |
| ------------------------- | ------------------------------------------------- |
| **Python (Google Colab)** | Ambiente de desenvolvimento e execução em nuvem   |
| **Pandas**                | Manipulação, limpeza e análise de dados tabulares |
| **Matplotlib**            | Criação de gráficos e complementos visuais        |
| **Scikit-learn**          | Segmentação e clusterização (KMeans)              |
| **Scipy (estatísticas)**  | Testes estatísticos para validação do teste A/B   |




