📦 Dados
🗂️ Arquivos
order.json— Histórico de pedidos (dados, valor, cliente, restaurante)
consumer.csv— Cadastro e características dos usuários
restaurant.csv— Informações dos restaurantes (ticket médio, tempo de entrega)
ab_test_ref.csv— Identificação do grupo A/B (controle vs target)
🔍 Amostragem aplicada
A base original continha mais de 3,6 milhões de pedidos , o que torna a execução integral computacionalmente custosa.
Por esse motivo, foi aplicada uma amostragem pesquisada estratificada , geralmente a base para aproximadamente 300 mil registros .

As distribuições de variáveis-chave como ticket médio, taxas de retenção e frequência de pedidos por cliente foram comparadas entre as bases (original e amostrada), garantindo que os padrões estatísticos fossem preservados .

✅ Essa amostra foi utilizada em todas as análises estatísticas, visualizações e segmentações.
## 🗃️ Arquivos de Dados

1. **`order.json`**  
   Dados dos pedidos realizados na plataforma, incluindo:
   - ID do pedido
   - Valor total do pedido
   - Data do pedido
   - Itens comprados (com preço unitário e quantidade)

2. **`consumer.csv`**  
   Informações dos usuários cadastrados:
   - ID do usuário
   - Nome (anonimizado)
   - Status de atividade (ativo/inativo)

3. **`restaurant.csv`**  
   Dados dos restaurantes parceiros:
   - ID do restaurante
   - Cidade, estado e país
   - Classificação de preço
   - Tempo de entrega estimado

4. **`ab_test_ref.csv`**  
   Referência dos grupos do teste A/B:
   - Grupo de Teste (usuários que receberam cupons)
   - Grupo de Controle (usuários que não receberam cupons)

---

## 🔗 Links para os Arquivos de Dados Originais

- [Pedidos (`order.json`)](https://data-architect-test-source.s3-sa-east-1.amazonaws.com/order.json.gz)  
- [Usuários (`consumer.csv`)](https://data-architect-test-source.s3-sa-east-1.amazonaws.com/consumer.csv.gz)  
- [Restaurantes (`restaurant.csv`)](https://data-architect-test-source.s3-sa-east-1.amazonaws.com/restaurant.csv.gz)  
- [Teste A/B (`ab_test_ref.csv`)](https://data-architect-test-source.s3-sa-east-1.amazonaws.com/ab_test_ref.tar.gz)

> Obs.: 🔍 Amostragem aplicada
A base original continha mais de 3,6 milhões de pedidos , o que torna a execução integral computacionalmente custosa.
Por esse motivo, foi aplicada uma amostragem pesquisada estratificada , geralmente a base para aproximadamente 300 mil registros .

As distribuições de variáveis-chave como ticket médio, taxas de retenção e frequência de pedidos por cliente foram comparadas entre as bases (original e amostrada), garantindo que os padrões estatísticos fossem preservados .

✅ Essa amostra foi utilizada em todas as análises estatísticas, visualizações e segmentações.




