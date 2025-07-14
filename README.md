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


##  Teste A/B


O **Teste A/B** foi realizado para comparar dois grupos de usuários:

- **Grupo Controle**: Usuários que não receberam o cupom.
  
- **Grupo Alvo**: Usuários que receberam o cupom.

  

O objetivo foi verificar se o envio de cupons teve impacto nas métricas de **ticket médio** e **retenção** de usuários.


1. **Divisão dos Grupos:**
   
   - O grupo controle não recebeu cupons, enquanto o grupo target recebeu os cupons de desconto.
   
3. **Métricas analisadas:**
   
   - **Ticket Médio**: A média do valor gasto por pedido.
     
   - **Retenção**: Porcentagem de usuários que realizaram mais de 1 pedido (usuários que retornaram ao app).
   
5. **Objetivo**: Comparar as métricas entre os dois grupos e entender qual grupo teve **melhor desempenho**.


##  Validação Estatística

Para validar se as diferenças observadas entre os grupos eram reais e não devidas ao acaso, apliquei a  **validação estatística**.

### Testes utilizados:

1. **Teste t de Student**: Para comparar o **ticket médio** entre os grupos controle e target.
2. **Teste de proporções**: Para comparar a **retenção** de usuários entre os grupos.

### Significância Estatística

- **Se o p-valor obtido for menor que 0,05**, significa que a diferença é **estatisticamente significativa** e que o impacto observado provavelmente **não foi por acaso**.
  
- **Se o p-valor for maior que 0,05**, a diferença pode ser **devida ao acaso** e, portanto, **não é significativa**.

### Resultados do Teste A/B


 Comparação entre Grupos (Controle vs Target)

| Indicador              | Grupo Controle | Grupo Target | Diferença      | Conclusão                         |
|------------------------|----------------|--------------|----------------|-----------------------------------|
| **Retenção (%)**       | 28%            | 35%          | +7 p.p.        |  Maior retenção no grupo Target |
| **Ticket Médio (R$)**  | R$ 42,50       | R$ 47,80     | + R$ 5,30      |  Maior gasto médio               |
| **Pedidos por Usuário**| 1,6            | 2,1          | +0,5 pedidos   |  Maior frequência de pedidos     |
| **p-valor (ret.)**     | —              | —            | p < 0.05       |  Diferença estatisticamente significativa |

### 
- **Retenção**: A diferença de 7 p.p. indica que o incentivo do cupom aumentou o número de usuários que fizeram pedidos repetidos.
- **Ticket Médio**: O aumento no ticket médio sugere que o cupom pode ter estimulado os usuários a adicionar itens extras, apesar de o desconto reduzir parcialmente o custo.
- **Pedidos por Usuário**: Uma elevação na frequência de pedidos confirma que o cupom ajudou a fidelizar os clientes.
- **Teste Estatístico**: Com p < 0.05, temos alta confiança de que as diferenças não ocorreram por acaso, reforçando a eficácia da campanha.





##  Viabilidade Financeira

  - **Definição do custo do cupom:** Custo estimado de R$10 por pedido com cupom
  - **Cálculo do custo total da campanha:** Multiplicação do custo por cupom pelo número de pedidos no grupo target
  - **Estimação do ganho adicional:** A diferença de ticket médio entre os grupos controle e target foi multiplicada pelo número de pedidos feitos pelo grupo target
  - **Comparação entre custo e ganho:** A campanha foi considerada financeiramente viável quando o ganho total foi superior ao custo da campanha

##  Segmentação de usuários

  A segmentação de usuários foi realizada com base em 3 critérios principais:

  - **Ticket Médio** (baixo vs alto): Ticket médio alto tende a gerar receita adicional maior, mas somente é viável se ultrapassar R$10.
  - **Frequência de Pedidos** (recorrente vs esporádico): Recorrente á a segmentação mais eficaz e financeiramente viável.
  - **Tempo desde o Cadastro** (novo vs antigo): Nenhum desses grupos tiveram ROI positivo.






##  Conclusão Final 

A campanha de cupons  apresentou impacto positivo no comportamento dos usuários do iFood, especialmente em termos de:

-  Aumento da **retenção** no grupo target em relação ao grupo controle
-  Usuários frequentes apresentaram uma receita adicional de R$11,90. Mais eficaz e financeiramente viável.
Com base nesses insights, a campanha **pode ser viável financeiramente e mais eficiente** se for personalizada para os perfis com maior propensão de resposta.



##  Recomendações estratégicas


Com base nas análises e resultados do **Teste A/B**, **Validação Estatística** e **Avaliação de Viabilidade Financeira**, as seguintes **recomendações estratégicas** são sugeridas para otimizar as campanhas e aumentar os resultados:

### 1. **Segmentação de Usuários**
   - **Focar em usuários com frequência alta**: Como os cupons têm maior impacto em usuários com frequência de pedidos, é recomendável segmentar as campanhas de cupons para esse público, incentivando-os a realizar novos pedidos.

### 2. **Testar diferentes valores de cupons**
   - O impacto do cupom pode ser mais eficaz se testado com **valores variáveis**, como cupons de **10%, 20%** ou **R$10**, para verificar qual valor realmente **gera mais engajamento** e **impacto na retenção**.

### 3. **Explorar novos canais de ativação**
   - A campanha de cupons pode ser mais eficaz se for promovida através de **outros canais**, como **e-mail marketing** ou **notificações push**, especialmente para usuários que não visualizaram o cupom diretamente no aplicativo.

### 5. **Monitoramento contínuo**
   - Monitorar constantemente as métricas para verificar se as mudanças propostas têm o **impacto esperado**.





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




