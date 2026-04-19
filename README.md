# 📊 Olist — Análise de Vendas

Análise do [Brazilian E-Commerce Public Dataset by Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce), utilizando **Excel** e **Power BI** para explorar vendas, comportamento de clientes e performance de entrega no e-commerce brasileiro.

---

## 🎯 Objetivos

Este projeto busca responder três perguntas de negócio:

1. 🗺️ **Quais estados têm o maior volume de pedidos e o maior ticket médio?**
2. ⭐ **Categorias com mais vendas têm melhor avaliação?**
3. 🚚 **O tempo de entrega impacta a nota de avaliação do cliente?**

---

## 🛠️ Ferramentas Utilizadas

- **Excel** — Limpeza de dados, tabelas dinâmicas e análise exploratória
- **Power BI** — Modelagem relacional, medidas DAX e dashboard interativo

---

## 📁 Estrutura do Projeto

```
📦 olist-analise-vendas
 ┣ 📂 dados/
 ┃ ┣ 📂 brutos/           ← CSV originai
 ┃ ┗ 📂 tratados/     ← Dados após limpeza
 ┣ 📂 excel/
 ┃ ┗ analise_olist.xlsx
 ┣ 📂 powerbi/
 ┃ ┗ dashboard_olist.pbix
 ┣ 📂 docs/
 ┃ ┗ relatorio_executivo.pdf
 ┗ README.md
```

---

## 📂 Sobre o Dataset

Dados públicos fornecidos pela **Olist**, maior loja de departamentos nos marketplaces brasileiros. Contém **100 mil pedidos** realizados entre 2016 e 2018, com informações de:

| Arquivo | Descrição |
|---|---|
| `olist_orders_dataset.csv` | Status, datas e tempo de entrega dos pedidos |
| `olist_order_items_dataset.csv` | Produtos, preço e frete |
| `olist_customers_dataset.csv` | Localização dos clientes |
| `olist_order_payments_dataset.csv` | Formas de pagamento e parcelamento |
| `olist_order_reviews_dataset.csv` | Notas e comentários dos clientes |
| `olist_products_dataset.csv` | Categorias de produto |
| `olist_sellers_dataset.csv` | Localização dos vendedores |
| `olist_geolocation_dataset.csv` | Coordenadas geográficas |
| `product_category_name_translation.csv` | Tradução dos nomes das categorias (português → inglês) |

---

## 🔧 Etapas do Projeto

### 1. Limpeza e Exploração — Excel
- Remoção de duplicatas e tratamento de valores nulos
- Criação de colunas calculadas (ex: tempo de entrega em dias)
- Tabelas dinâmicas por região, categoria e período
- Fórmulas utilizadas: `PROCX`, `SOMASES`, `ÍNDICE+CORRESP`

### 2. Modelagem e Dashboard — Power BI
- Modelo relacional conectando todas as tabelas via `order_id` e `customer_id`
- Medidas em DAX: ticket médio, crescimento MoM, NPS simplificado
- Dashboard com 3 páginas: **Visão Geral**, **Clientes**, **Produtos & Entregas**
- Filtros interativos por período, estado e categoria

---

## 📸 Dashboard

> 🚧 Prints serão adicionados após a conclusão do dashboard no Power BI.

<!-- 
![Visão Geral](docs/screenshots/visao_geral.png)
![Análise de Clientes](docs/screenshots/clientes.png)
![Produtos e Entregas](docs/screenshots/produtos_entregas.png)
-->

---

## 💡 Principais Insights

> 🚧 Insights serão adicionados após a análise dos dados.

---

## 📌 Status do Projeto

- [ ] Download e organização dos dados
- [ ] Limpeza e exploração no Excel
- [ ] Modelagem no Power BI
- [ ] Criação do dashboard
- [ ] Documentação final e insights

---

## 📄 Licença

Dataset licenciado sob [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/).
