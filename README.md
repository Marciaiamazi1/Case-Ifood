# Case Técnico de Data Analytics - IFood

O iFood, líder em delivery de alimentos na América Latina, realizou uma campanha de cupons com o intuito de incentivar novos pedidos e aumentar a retenção de clientes. Para validar a efetividade da iniciativa, foi realizado um teste A/B , em que parte dos usuários recebeu o benefício (grupo "target") e outra parte não (grupo "controle").

O desafio analítico consistiu em avaliar se a campanha teve impacto significativo nas métricas de comportamento dos usuários e, a partir disso, propor recomendações personalizadas com base em segmentações comportamentais.


##  Análises realizadas
- Análise de conversão entre grupo controle e grupo cupom (teste A/B)
- Segmentação de usuários com base em comportamento e ticket médio
- Avaliação de viabilidade financeira dos cupons (ROI)
- Criação de gráficos para suporte às conclusões

##  Como Executar o repositório
1. Clone este repositório:
 https://github.com/Marciaiamazi1/Case-Ifood.git

2. Abra o arquivo case_ifood.ipynb no Jupyter ou Google Colab.


## Estrutura de Arquivos

- `case`
- `dados`
- `imagens`
- `notebook`
- `READ`

##  Resultados
- O grupo que recebeu o cupom A teve uma taxa de conversão 15% maior do que o grupo controle (p-valor < 0.05), indicando que o cupom teve efeito positivo estatisticamente significativo.
  
- Usuários com alto ticket médio responderam melhor à promoção.
  
- A estratégia é viável financeiramente no curto prazo.


##  Bibliotecas e Tecnologias Utilizadas

| Tecnologia               | Finalidade Principal                                       |
|--------------------------|------------------------------------------------------------|
| **Python (Google Colab)**| Ambiente de desenvolvimento e execução em nuvem           |
| **Pandas**               | Manipulação, limpeza e análise de dados tabulares         |
| **Seaborn**              | Visualização estatística com gráficos personalizados       |
| **Matplotlib**           | Criação de gráficos e complementos visuais                 |
| **Scikit-learn**         | Segmentação e clustering (KMeans)                          |
| **Scipy (stats)**        | Testes estatísticos para validação do teste A/B            |



