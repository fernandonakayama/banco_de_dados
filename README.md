[![ITR](https://github.com/fernandonakayama/banco_de_dados/blob/main/logo-instituto-tres-rios-ufrrj-old%20(1).png "ITR")](https://github.com/fernandonakayama/banco_de_dados/blob/main/logo-instituto-tres-rios-ufrrj-old%20(1).png "ITR")


# Projeto de Banco de Dados: Sistema de E-Commerce (TechStore)
Projeto prático desenvolvido para a disciplina de Banco de Dados. O objetivo foi modelar,
implementar e validar um banco de dados relacional para um e-commerce com suporte a
transações ACID e consultas analíticas.
## Integrantes do Grupo
* Nome do Aluno 1 - Matrícula
* Nome do Aluno 2 - Matrícula
## Tecnologias Utilizadas
* **SGBD:** MySQL (phpMyAdmin)
* **Linguagem de Consulta:** SQL (DDL e DML)
* **Linguagem de Aplicação:** Python
* **Bibliotecas:** `mysql-connector-python`, `gradio`
* **Ambiente de Execução:** Google Colab
## Estrutura do Repositório
* `docs/`: Diagrama Entidade-Relacionamento (`modelo_ER.png`).
* `sql/`: Script de definição de esquema e carga inicial (`database_setup.sql`).
* `scripts/`: Script de autoteste estrutural e integridade referencial
(`autoteste_ecommerce.py`).
* `app/`: Interface interativa Gradio com checkout ACID e consulta de pedidos
(`app_vendas.ipynb`).
## Modelo Relacional e Regras de Negócio
O sistema atende exclusivamente clientes Pessoa Física e possui 7 tabelas normalizadas:
1. `CATEGORIA` e `MARCA`: Domínios para catalogação de produtos.
2. `PRODUTO`: Itens comercializáveis com controle de estoque e preço atual.
3. `CLIENTE` e `ENDERECO`: Relação 1:N com entidade fraca para múltiplos endereços de
entrega.
4. `PEDIDO`: Cabeçalho transacional de compras.
5. `CONTEM` / `ITENS_PEDIDO` (Tabela Associativa): Resolução da cardinalidade N:M entre
`PEDIDO` e `PRODUTO`, registrando quantidade e preço unitário histórico.
## Como Executar o Projeto
1. Execute o script `database_setup.sql` no phpMyAdmin para criar as tabelas e popular a
base.
2. Abra o notebook `app_vendas.ipynb` no Google Colab e execute o código para iniciar o
Gradio.
3. Na interface gráfica gerada, digite o nome do banco de dados e a senha de acesso nos
campos apropriados para estabelecer a conexão segura.
4. Execute o script `autoteste_ecommerce.py` para validar a estrutura relacional.
5. Teste as abas de **Realizar Compra (ACID)** e **Consultar Venda (JOINs)**.

# Projeto de Banco de Dados: Sistema de E-Commerce (TechStore)
Projeto prático desenvolvido para a disciplina de Banco de Dados. O objetivo foi modelar,
implementar e validar um banco de dados relacional para um e-commerce com suporte a
transações ACID e consultas analíticas.
## Integrantes do Grupo
* Nome do Aluno 1 - Matrícula
* Nome do Aluno 2 - Matrícula
## Tecnologias Utilizadas
* **SGBD:** MySQL (phpMyAdmin)
* **Linguagem de Consulta:** SQL (DDL e DML)
* **Linguagem de Aplicação:** Python
* **Bibliotecas:** `mysql-connector-python`, `gradio`
* **Ambiente de Execução:** Google Colab
## Estrutura do Repositório
* `docs/`: Diagrama Entidade-Relacionamento (`modelo_ER.png`).
* `sql/`: Script de definição de esquema e carga inicial (`database_setup.sql`).
* `scripts/`: Script de autoteste estrutural e integridade referencial
(`autoteste_ecommerce.py`).
* `app/`: Interface interativa Gradio com checkout ACID e consulta de pedidos
(`app_vendas.ipynb`).
## Modelo Relacional e Regras de Negócio
O sistema atende exclusivamente clientes Pessoa Física e possui 7 tabelas normalizadas:
1. `CATEGORIA` e `MARCA`: Domínios para catalogação de produtos.
2. `PRODUTO`: Itens comercializáveis com controle de estoque e preço atual.
3. `CLIENTE` e `ENDERECO`: Relação 1:N com entidade fraca para múltiplos endereços de
entrega.
4. `PEDIDO`: Cabeçalho transacional de compras.
5. `CONTEM` / `ITENS_PEDIDO` (Tabela Associativa): Resolução da cardinalidade N:M entre
`PEDIDO` e `PRODUTO`, registrando quantidade e preço unitário histórico.
## Como Executar o Projeto
1. Execute o script `database_setup.sql` no phpMyAdmin para criar as tabelas e popular a
base.
2. Abra o notebook `app_vendas.ipynb` no Google Colab e execute o código para iniciar o
Gradio.
3. Na interface gráfica gerada, digite o nome do banco de dados e a senha de acesso nos
campos apropriados para estabelecer a conexão segura.
4. Execute o script `autoteste_ecommerce.py` para validar a estrutura relacional.
5. Teste as abas de **Realizar Compra (ACID)** e **Consultar Venda (JOINs)**.
