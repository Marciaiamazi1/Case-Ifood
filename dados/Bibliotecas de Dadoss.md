# 📚 Catálogo de Dados – Case iFood

Este diretório contém os conjuntos de dados utilizados para análise do case técnico, com origem e dicionário de variáveis de cada tabela.

---

## 📦 Tabelas Disponíveis

### 1. `order.json` — 📍 [Download](https://data-architect-test-source.s3-sa-east-1.amazonaws.com/order.json.gz)

**Total aproximado:** 3,6 milhões de pedidos entre dezembro/2018 e janeiro/2019.

**Principais colunas:**
- `order_id`: ID único do pedido
- `customer_id`: Identificador do usuário
- `order_created_at`: Data e hora do pedido
- `order_total_amount`: Valor total (R$)
- `order_scheduled`: Se o pedido foi agendado (`true` ou `false`)
- `items`: Lista de produtos (quantidade, preço unitário, etc.)
- `delivery_address_*`: Informações detalhadas de entrega
- `merchant_id`: Restaurante responsável pelo pedido
- `origin_platform`: Plataforma usada para o pedido (ex: iOS, Android)

---

### 2. `consumer.csv` — 👤 [Download](https://data-architect-test-source.s3-sa-east-1.amazonaws.com/consumer.csv.gz)

**Total aproximado:** 806 mil usuários.

**Principais colunas:**
- `customer_id`: ID do usuário
- `created_at`: Data de criação da conta
- `active`: Se o usuário está ativo
- `language`: Idioma preferido
- `customer_name`, `customer_phone_area`, `customer_phone_number`: Dados de identificação (anonimizados)

---

### 3. `restaurant.csv` — 🍽️ [Download](https://data-architect-test-source.s3-sa-east-1.amazonaws.com/restaurant.csv.gz)

**Total aproximado:** 7 mil restaurantes.

**Principais colunas:**
- `id`: Identificador do restaurante
- `created_at`: Data de cadastro
- `enabled`: Restaurante ativo na base (`true` ou `false`)
- `average_ticket`: Valor médio dos pedidos
- `price_range`: Faixa de preço (nível 1 a 3)
- `delivery_time`: Tempo estimado de entrega
- `minimum_order_value`: Pedido mínimo (R$)
- `merchant_city`, `merchant_state`, `merchant_country`: Localização

---

### 4. `ab_test_ref.csv` — 🧪 [Download](https://data-architect-test-source.s3-sa-east-1.amazonaws.com/ab_test_ref.tar.gz)

**Descrição:** Indica se o usuário participou da campanha de cupons.

**Colunas:**
- `customer_id`: ID do usuário
- `is_target`: Grupo designado — `target` (recebeu cupom) ou `control` (grupo de controle)

---

## ⚠️ Observações

- Todos os dados são públicos e utilizados exclusivamente para fins educacionais no contexto de um desafio técnico.
- Recomenda-se o uso de amostragem ou filtragem para manuseio local devido ao tamanho das bases.






