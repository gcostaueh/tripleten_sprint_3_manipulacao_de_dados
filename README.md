# Sprint 3 - Análise Exploratória de Dados (Instacart)

## Descrição do Projeto

Este projeto faz parte do bootcamp de Ciência de Dados da TripleTen e tem como objetivo aplicar técnicas de **Análise Exploratória de Dados (AED)** em um conjunto de dados real da Instacart.

A **Instacart** é uma plataforma de entrega de supermercado onde clientes podem fazer pedidos online e receber suas compras em casa.

Os dados utilizados neste projeto foram originalmente disponibilizados em uma competição do Kaggle (2017) e posteriormente adaptados para fins educacionais, incluindo:
- Redução de volume de dados
- Inserção de valores ausentes
- Inserção de duplicidades

O conjunto de dados fornecido pela TripleTen foi modificado a partir do original. Foi reduzido o tamanho dele para que os cálculos sejam executados mais rapidamente e indluídos valores ausentes e duplicados. Também tiveram o cuidado de preservar as distribuições dos dados originais quando foi feita as alterações.

---

## Objetivo TM
 
Realizar o **pré-processamento** dos dados e conduzir uma análise exploratória para identificar padrões e comportamentos dos clientes, como:
- Frequência de pedidos
- Horários e dias mais comuns de compra
- Produtos mais comprados
- Hábitos de recompra

---

## Conjunto de Dados

O projeto utiliza 5 datasets:

- `instacart_orders.csv` → Informações sobre pedidos
- `products.csv` → Informações sobre produtos
- `order_products.csv` → Produtos incluídos em cada pedido
- `aisles.csv` → Categorias de corredores
- `departments.csv` → Categorias de departamentos

---

## Dicionário de Dados (Resumo)

### instacart_orders.csv
- `order_id` → ID do pedido  
- `user_id` → ID do cliente  
- `order_number` → Número do pedido do cliente  
- `order_dow` → Dia da semana (0 = domingo)  
- `order_hour_of_day` → Hora do pedido (0–23)  
- `days_since_prior_order` → Dias desde o último pedido  

### products.csv
- `product_id` → ID do produto  
- `product_name` → Nome do produto  
- `aisle_id` → ID do corredor  
- `department_id` → ID do departamento  

### order_products.csv
- `order_id` → ID do pedido  
- `product_id` → ID do produto  
- `add_to_cart_order` → Ordem de adição ao carrinho  
- `reordered` → Se já foi comprado antes (0 ou 1)  

### aisles.csv
- `aisle_id` → ID do corredor  
- `aisle` → Nome do corredor  

### departments.csv
- `department_id` → ID do departamento  
- `department` → Nome do departamento  

---

## Etapas do Projeto

### 1 - Leitura e Exploração Inicial
- Carregamento dos dados com `pandas`
- Ajuste de parâmetros no `read_csv()`
- Análise inicial com `.info()` e `.head()`

---

### 2 - Pré-processamento de Dados
- Correção de tipos de dados
- Tratamento de valores ausentes
- Remoção de duplicatas
- Justificativa das decisões tomadas

---

### 3 - Análise Exploratória de Dados (AED)

#### 🔹 Parte A (Obrigatória)
- Validação de valores (`order_hour_of_day` e `order_dow`)
- Pedidos por hora do dia
- Pedidos por dia da semana
- Tempo entre pedidos

#### 🔹 Parte B (Obrigatória)
- Comparação de pedidos (quarta vs sábado)
- Distribuição do número de pedidos por cliente
- Top 20 produtos mais comprados

#### 🔹 Parte C (Opcional - mínimo 2)
- Quantidade de itens por pedido
- Produtos mais recomprados
- Proporção de recompra por produto
- Proporção de recompra por cliente
- Produtos adicionados primeiro ao carrinho

---

## Visualizações

Foram utilizados gráficos para melhor interpretação dos dados, garantindo:
- Títulos claros
- Eixos rotulados
- Legendas (quando necessário)

---

## Principais Insights

- Horários de pico de pedidos  
- Dias com maior volume de compras  
- Produtos mais populares  
- Tendência de recompra dos clientes  

---

## Tecnologias Utilizadas

- Python  
- Pandas  
- Matplotlib / Seaborn  
- Jupyter Notebook  

---

## Conclusão

O projeto permitiu aplicar conceitos essenciais de:
- Limpeza de dados
- Análise exploratória
- Visualização de dados

Além disso, trouxe insights relevantes sobre o comportamento de consumo dos usuários da plataforma.

---