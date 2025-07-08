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
   - O grupo controle não recebeu cupons, enquanto o grupo alvo recebeu os cupons de desconto.
   
2. **Métricas analisadas:**
   - **Ticket Médio**: A média do valor gasto por pedido.
   - **Retenção**: Porcentagem de usuários que realizaram mais de 1 pedido (usuários que retornaram ao app).
   
3. **Objetivo**: Comparar as métricas entre os dois grupos e entender qual grupo teve **melhor desempenho**.


##  Validação Estatística

Para validar se as diferenças observadas entre os grupos eram reais e não devidas ao acaso, apliquei a  **validação estatística**.

### Testes utilizados:

1. **Teste t de Student**: Para comparar o **ticket médio** entre os grupos controle e target.
2. **Teste de proporções**: Para comparar a **retenção** de usuários entre os grupos.

### Significância Estatística

- **Se o p-valor obtido for menor que 0,05**, significa que a diferença é **estatisticamente significativa** e que o impacto observado provavelmente **não foi por acaso**.
- **Se o p-valor for maior que 0,05**, a diferença pode ser **devida ao acaso** e, portanto, **não é significativa**.

### Resultados do Teste A/B

| Métrica                       | Controle   | Alvo      | Resultado Estatístico  |
|-------------------------------|------------|-----------|------------------------|
| **Ticket Médio**              | R$ 76,12   | R$ 76,91  | p = 0,71 (sem impacto)  |
| **Retenção (% 2+ Pedidos)**   | 44,1%      | 46,7%     | p = 0,22 (sem impacto)  |


- O **p-valor** para o **ticket médio** (0,71) e para a **retenção** (0,22) foi **maior que 0,05**, o que **indica que não houve impacto estatisticamente significativo** com o envio de cupons.
- As **diferenças observadas podem ser atribuídas ao acaso**, e, portanto, não podemos concluir que os cupons causaram mudanças significativas nas métricas analisadas.



##  Viabilidade Financeira

  - **Definição do custo do cupom:** Custo estimado de R$10 por pedido com cupom
  - **Cálculo do custo total da campanha:** Multiplicação do custo por cupom pelo número de pedidos no grupo target
  - **Estimação do ganho adicional:** A diferença de ticket médio entre os grupos controle e target foi multiplicada pelo número de pedidos feitos pelo grupo target
  - **Comparação entre custo e ganho:** A campanha foi considerada financeiramente viável quando o ganho total foi superior ao custo da campanha

##  Segmentação de usuários

  A segmentação de usuários foi realizada com base em 3 critérios principais:

  - **Ticket Médio** (baixo vs alto)
  - **Frequência de Pedidos** (recorrente vs esporádico)
  - **Tempo desde o Cadastro** (novo vs antigo)



##  Recomendações estratégicas

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




