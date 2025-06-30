## 📦 Dados


### 🗂️ Arquivos 

- `order.json` — Histórico de pedidos (data, valor, cliente, restaurante)
- `consumer.csv` — Cadastro e características dos usuários
- `restaurant.csv` — Informações dos restaurantes (ticket médio, tempo de entrega)
- `ab_test_ref.csv` — Identificação do grupo A/B (controle vs target)

### 🔍 Amostragem aplicada

A base original continha mais de **3,6 milhões de pedidos**, o que torna a execução integral computacionalmente custosa.  
Por esse motivo, foi aplicada uma **amostragem aleatória estratificada**, reduzindo a base para aproximadamente **300 mil registros**. 

As distribuições de variáveis-chave como **ticket médio, taxa de retenção e frequência de pedidos por cliente** foram comparadas entre as bases (original e amostrada), garantindo que **os padrões estatísticos fossem preservados**.  

✅ Essa amostra foi utilizada em todas as análises estatísticas, visualizações e segmentações.




