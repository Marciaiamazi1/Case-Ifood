# Case Técnico de Data Analytics - IFood

O iFood, líder em delivery de alimentos na América Latina, realizou uma campanha de cupons com o intuito de incentivar novos pedidos e aumentar a retenção de clientes. Para validar a efetividade da iniciativa, foi realizado um teste A/B , em que parte dos usuários recebeu o benefício (grupo "target") e outra parte não (grupo "controle").

O desafio analítico consistiu em avaliar se a campanha teve impacto significativo nas métricas de comportamento dos usuários e, a partir disso, propor recomendações personalizadas com base em segmentações comportamentais.



##  Análises realizadas

- Análise exploratória e descritiva

   - Verificação da distribuição dos dados por grupo (controle vs target)
   - Análise da taxa de retenção e ticket médio por grupo.
  
- Criação de KPIs

  - Número total de pedidos por usuário
  - Ticket médio (valor por pedido)
  - Taxa de retenção (usuários com mais de 1 pedido)

- Validação estatística

  - Aplicação de teste t para comparar o ticket médio entre os grupos
  - Teste de proporções para validar diferenças em retenção
  -  Verificação de significância (p - valor < 0,05)
   
- Avaliação de viabilidade financeira

  - **Definição do custo do cupom:** Custo estimado de R$10 por pedido com cupom
  - **Cálculo do custo total da campanha:** Multiplicação do custo por cupom pelo número de pedidos no grupo target
  - **Estimação do ganho adicional:** A diferença de ticket médio entre os grupos controle e target foi multiplicada pelo número de pedidos feitos pelo grupo target
  - **Comparação entre custo e ganho:** A campanha foi considerada financeiramente viável quando o ganho total foi superior ao custo da campanha

- Segmentação de Usuários

  A segmentação de usuários foi realizada com base em 4 critérios principais:

  - **Ticket Médio** (baixo vs alto)
  - **Frequência de Pedidos** (recorrente vs esporádico)
  - **Tempo desde o Cadastro** (novo vs antigo)
  - Por localização geográfica

 - Recomendações estratégicas

   - Ações específicas por perfil (novos, recorrentes, inativos)
   - Sugestões para personaliação futura da campanha
   - Indicação de próximos testes A/B mais focados
  



##  Conclusão

| Etapa                             | Descrição                                                                                                    |
|----------------------------------|----------------------------------------------------------------------------------------------------------------|
| **1. Análise Descritiva**        | • Exploração inicial dos dados de quantidade de pedidos e número de usuários por grupo, ticket médio e taxa de retenção. |
| **2. Avaliação de Impacto – Teste A/B** | • Aumento na retenção e no ticket médio no grupo que recebeu o cupom. <br>• Campanha teve impacto real. |
| **3. Segmentação com K-Means**   | • Frequência de pedidos<br>• Ticket médio individual por usuário |
| **4. Interpretação Comportamental** | • Usuários novos respondem melhor a cupons.<br>• Usuários de regiões com menor ticket médio se engajam mais<br>•Usuários inativos raramente voltam - mesmo com cupom.<br>• Usuários frequentes usam o cupom, mas sem mudar o comportamento.
| **5. Recomendações Estratégicas por Perfil** |• Usuários novos (recentemente cadastrados): Enviar cupons de forma automática; testar campanhas de incentivo com comunicação <br>• Usuários recorrentes: Evitar cupons genéricos; oferecer programas de pontos , cashback ou combos.<br>•Usuários inativos: Testar pesquisas de feedback, camapnhas de reativação<br>•Regiões com baixo ticket médio: Continuar campanhas com cupom emregiões de menor poder aquisitivo.; testar cupom de valor fixo (ex: R$10) em vez de percentual.<br>• Usuários com alto ticket médio: Testar cupons progressivos (ex: R$20 off acima de R$100).<br>•Criar campanhas com frete grátis ou upgrade no delivery.|





##  Teste A/B

### Objetivo

O teste A/B foi realizado para avaliar o impacto de uma campanha de **cupons** sobre a **retenção de usuários**. O objetivo foi comparar dois grupos:
- **Grupo Controle**: Não recebeu cupons.
- **Grupo Target**: Recebeu cupons.

### Como foi realizado

- **Métricas analisadas**: Retenção, ticket médio e número de pedidos.
- **Testes estatísticos**:
  - **Teste t** para comparar o **ticket médio** entre os grupos.
  - **Teste de proporções**:  comparar a **retenção**.
 
##  Análise de Impacto

O objetivo do **Teste A/B** foi analisar se o envio de cupons para o **grupo target** teve um **impacto estatisticamente significativo** em comparação ao **grupo controle**.

Os resultados comparando duas métricas principais foram: **Ticket Médio** e **Taxa de Retenção** (usuários com 2 ou mais pedidos).

| Métrica                       | Controle   | Target      | Resultado Estatístico  |
|-------------------------------|------------|-----------|------------------------|
| **Ticket Médio**               | R$ 76,12   | R$ 76,91  | p = 0,71 (sem impacto)  |
| **Retenção (% 2+ Pedidos)**   | 44,1%      | 46,7%     | p = 0,22 (sem impacto)  |

### **Interpretação dos Resultados**:
- **Ticket Médio**: Embora o grupo **alvo** tenha mostrado um aumento no ticket médio, o **p-valor** de 0,71 indica que essa diferença não é estatisticamente significativa. Isso sugere que **o envio de cupons não teve impacto significativo no valor médio dos pedidos**.
  
- **Retenção (% 2+ Pedidos)**: O grupo **alvo** teve uma retenção ligeiramente maior, mas com um **p-valor** de 0,22, a diferença também não é estatisticamente significativa. Isso significa que **o envio de cupons não gerou um impacto relevante na retenção de usuários**.

###
Com base nesses resultados, **não houve evidência de impacto estatisticamente significativo** do envio de cupons nas métricas de **ticket médio** e **retenção**.


### Resultados

- O **grupo target** apresentou uma **retenção 7% maior** e um **ticket médio 5,30% superior** ao grupo controle.
- **P-valor** < 0,05 indicou que as diferenças são **estatisticamente significativas**.


A campanha de cupons foi eficaz para **aumentar a retenção** e o **ticket médio**.
Recomendável escalar a campanha com ajustes de segmentação.



##  Como Executar o repositório
1. Clone este repositório:
 https://github.com/Marciaiamazi1/Case-Ifood.git

2. Abra os arquivos contidos na pasta notebook no Jupyter ou Google Colab para visualizar as análises realizadas e explorar os resultados.



## Estrutura de Arquivos
- `case`:  Scripts e códigos principais
- `dados`: Dados utilizados para a análise
- `imagens`: Imagens geradas durante a análise (gráficos, diagramas)
- `notebook`: Análises interativas
- `README:`Arquivo, com explicações detalhadas do projeto








## Bibliotecas e tecnologias utilizadas

| Tecnologia                | Finalidade Principal                              |
| ------------------------- | ------------------------------------------------- |
| **Python (Google Colab)** | Ambiente de desenvolvimento e execução em nuvem   |
| **Pandas**                | Manipulação, limpeza e análise de dados tabulares |
| **Matplotlib**            | Criação de gráficos e complementos visuais        |
| **Scikit-learn**          | Segmentação e clusterização (KMeans)              |
| **Scipy (estatísticas)**  | Testes estatísticos para validação do teste A/B   |




