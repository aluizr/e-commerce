# e-commerce
Modelagem do projeto lógico de banco de dados para o cenário de e-commerce.
Adicionado o modelo EER do e-commerce em formato PDF e PNG;
Adicionado o arquivo gerado pelo aplicatico MySQL Workbench 8.0;
Adicionado arquivo no formato TXT com a criação do SCHEMA do banco de dados e as consultas solicitadas.

# Descrição das tabelas e campos.

## Fornecedor
- **ID Fornecedor:** INT
- **Razão Social:** VARCHAR(45)
- **CNPJ:** VARCHAR(45)

---

## Terceiro - Vendedor
- **ID Terceiro - Vendedor:** INT
- **ID Produto:** INT
- **Razão Social:** VARCHAR(45)
- **Nome Fantasia:** VARCHAR(45)
- **CNPJ:** VARCHAR(45)
- **Descrição:** VARCHAR(45)
- **Local:** VARCHAR(45)
- **Quantidade:** INT

---

## Cliente
- **ID Cliente:** INT
- **Nome Completo:**
  - **Primeiro Nome:** VARCHAR(10)
  - **Nome do Meio:** VARCHAR(3)
  - **Sobrenome:** VARCHAR(20)
- **CPF:** CHAR(11)
- **Endereço:** VARCHAR(45)

---

## Pedido
- **ID Pedido:** INT
- **Status do Pedido:** ENUM(...)
- **Data de Nascimento do Cliente:** DATE

---

## Estoque
- **ID Estoque:** INT
- **Descrição:** VARCHAR(45)
- **Local:** VARCHAR(45)

---

## Pagamento
- **ID Pagamento:** INT
- **Tipo:** VARCHAR(45)

---

## Entrega
- **ID Entrega:** INT
- **Detalhe:** VARCHAR(45)
- **Status de Entrega:** VARCHAR(45)
- **Código de Rastreio:** VARCHAR(45)
- **Observação:** VARCHAR(45)

---

## Produto
- **ID Produto:** INT
- **Produtos por Vendedor:** INT
- **Quantidade:** INT
- **Valor:** VARCHAR(45)
