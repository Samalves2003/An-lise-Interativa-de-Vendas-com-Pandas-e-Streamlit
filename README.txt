# 📊 Análise Interativa de Vendas

**Análise Interativa de Vendas** é um painel web desenvolvido com **Python**, **Pandas** e **Streamlit**, que permite a análise dinâmica de dados de vendas através de uma interface intuitiva. O sistema utiliza dados simulados para representar cenários reais, oferecendo flexibilidade para exploração e geração de insights.

---

## 🧠 Funcionalidades

- Visualização interativa de vendas por loja, vendedor, produto, cliente e forma de pagamento.
- Cálculo automático de comissão sobre as vendas (5%).
- Geração de dados fictícios com clientes, datas, produtos e formas de pagamento aleatórias.
- Exportação dos dados simulados em formatos `.csv` e `.xlsx`.
- Tabela dinâmica com totalizadores por linha e por coluna.

---

## 🗃️ Sobre os dados fictícios

Este projeto utiliza **dados simulados** gerados automaticamente por um script em Python, com o objetivo de representar um cenário de vendas no varejo de forma realista.

### 📌 O que os dados representam?

- **Compras:** Registros de vendas com data, loja, vendedor, produto, forma de pagamento, nome e gênero do cliente.
- **Produtos:** Lista de 5 produtos eletrônicos com identificadores únicos e preços definidos.
- **Lojas:** Conjunto de 5 lojas distribuídas por diferentes estados brasileiros, cada uma com seus respectivos vendedores.

As datas das compras são distribuídas aleatoriamente ao longo dos últimos 365 dias. Os nomes dos clientes são gerados de forma realista com base no gênero.

### 💡 Por que usar dados fictícios?

- Evita exposição de dados sensíveis ou reais.
- Facilita o teste de funcionalidades e visualizações.
- Permite maior liberdade de manipulação dos dados.

---

## 📁 Arquivos gerados

- `compras.csv` / `compras.xlsx`  
  Contém:
  - `data`: data e hora da compra  
  - `loja`: cidade onde a compra foi realizada  
  - `vendedor`: quem realizou a venda  
  - `produto`: item vendido  
  - `cliente_nome` e `cliente_genero`: dados simulados do cliente  
  - `forma_pagamento`: método de pagamento utilizado  

- `produtos.csv` / `produtos.xlsx`  
  - `id`: identificador do produto  
  - `nome`: nome do produto  
  - `preco`: valor do item  

- `lojas.csv` / `lojas.xlsx`  
  - `estado`, `cidade`: localização da loja  
  - `vendedores`: nomes dos vendedores da loja  

---

## 🧰 Tecnologias utilizadas

- **Python 3**
- **Pandas**
- **Streamlit**
- **names** (gerador de nomes aleatórios realistas)
- **datetime**, **random**, **pathlib**

---

## ⚙️ Como executar o projeto

### 1. Clone o repositório
```bash
git clone https://github.com/seu-usuario/analise-interativa-vendas.git
cd analise-interativa-vendas
