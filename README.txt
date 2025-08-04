# 📊 Análise Interativa de Vendas

**Análise Interativa de Vendas** é um painel web desenvolvido com **Python**, **Pandas** e **Streamlit**, que permite a análise dinâmica de dados de vendas por meio de uma interface simples e intuitiva.  
A aplicação simula um cenário de varejo com dados realistas e permite ao usuário cruzar informações em tempo real para obter insights detalhados.

---

## 🧠 Funcionalidades

- Visualização interativa por loja, vendedor, produto, cliente e forma de pagamento.
- Cálculo automático de comissão sobre as vendas (5%).
- Geração de dados fictícios e realistas de forma automatizada.
- Consolidação de dados a partir de **três planilhas diferentes**.
- Exportação dos dados simulados em formatos `.csv` e `.xlsx`.
- Tabela dinâmica (pivot table) com totalizadores por linha e coluna.

---

## 🗃️ Sobre os dados fictícios

Este projeto utiliza dados **totalmente simulados**, criados por um script Python para representar um ambiente de vendas realista, com 2.000 registros aleatórios.

### 📌 O que os dados representam?

- **Compras:** Data da venda, loja, vendedor, produto vendido, cliente (nome e gênero) e forma de pagamento.
- **Produtos:** Catálogo com 5 produtos eletrônicos, cada um com um preço.
- **Lojas:** 5 lojas localizadas em estados diferentes, cada uma com uma equipe de vendedores.

Os nomes dos clientes são gerados com base no gênero, as datas variam aleatoriamente ao longo de um ano, e os pagamentos são distribuídos entre cartão, boleto, pix e dinheiro.

---

### 🔗 Consolidação de dados

Durante a execução da aplicação, os dados são **lidos de três planilhas separadas**:

- `compras.csv` / `compras.xlsx`
- `produtos.csv` / `produtos.xlsx`
- `lojas.csv` / `lojas.xlsx`

Esses dados são **unificados em um único DataFrame**, onde:

- As compras são integradas aos produtos (para adicionar o preço).
- Uma coluna de **comissão (5%)** é criada automaticamente.
- As informações de loja, vendedor e forma de pagamento são mantidas para permitir cruzamentos.

Essa união permite gerar análises detalhadas por qualquer dimensão escolhida pelo usuário.

---

## 📁 Estrutura do projeto

analise-interativa-vendas/
│
├── datasets/
│ ├── compras.csv
│ ├── compras.xlsx
│ ├── lojas.csv
│ ├── lojas.xlsx
│ ├── produtos.csv
│ ├── produtos.xlsx
│
├── AIV.py # Aplicação principal (Análise Interativa de Vendas)
├── gera_dataset.py # Script que gera os dados fictícios
└── README.md # Este arquivo