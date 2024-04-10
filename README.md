# Repositório do projeto All For One 🤝
 ## Módulo: BACK-END
 
  Repositório possui projeto desenvolvido no período que estive na <b>Trybe</b>, abordando os conceitos de SQL e seus comandos. 
## Informações de aprendizados

- Este é um projeto desenvolvido para me ajudar a aprender os principais conceitos de `SQL`.
- Meu primeiro projeto de `SQL` e `MySQL`;
- Utilizei o `MySQL Workbench` para visualização das tabelas.
## Aprendizados

1) Trabalhar com os conceitos de SQL realizando:
  - Consultas;
  - seleções;
  - realizar operações matemáticas;
  - classificar dados;
  - filtrar resultados;
  - adicionar, atualizar e excluir dados.

2) Utilização da ferramenta gráfica MySQL Workbench, utilizando docker para conteinerização.

## Linguagem usadas

[![Docker][Docker-logo]][Docker-url]
[![MySQL][MySQL-logo]][MySQL-url]
## O que foi desenvolvido

Neste projeto com o codinome All For One praticamos conceitos de SQL, no qual tive que escrever query's para criação de dados, filtragem e manipulação de tabelas.

Temos, nesse projeto, uma série de desafios com diferentes níveis de complexidade que devem ser resolvidos cada um em seu arquivo próprio.

Foi criado na raiz do projeto um arquivo chamado desafioN.sql, em que N é o número do desafio;

O arquivo contem apenas o código SQL do desafio resolvido.

Após a execução dos teste locais, o banco de dados northwind é recriado.

> Banco de dados _northwind_ fornecido pela Trybe.
## Instruções para instalar e rodar

1. Clone o repo:
```
  git clone git@github.com:Ludson96/project-mysql-all-for-one.git
```
2. Instale as suas dependências:
```
  npm install
```
3. Já tem um arquivo `docker-compose.yml` criado. Para executar o container, utilize o seguinte comando (sendo a flag -d para executar em segundo plano):
```
docker-compose up -d
```
4. Utilize o arquivo `northwind.sql` para criar o banco de dados. Recomendo utilizar uma ferramenta de design de banco de dados visual, eu utilizei o [MySQL Workbench]

5. Os arquivos com `desafioN.sql`, sendo N o número do requisito. Copie e cole para testar o comando e verificar o que retornar segundo os requisitos abaixo.
# Requisitos

<details>

## Desafios Iniciais
### 1 - Exiba apenas os nomes dos produtos na tabela `products`.

---
### 2 - Exiba os dados de todas as colunas da tabela `products`.

---
### 3 - Escreva uma query que exiba os valores da coluna que representa a _primary key_ da tabela `products`.

---
### 4 - Conte quantos registros existem na coluna `product_name` da tabela `products`.

  ---
### 5 - Monte uma query que exiba os dados da tabela `products` a partir do quarto registro até o décimo terceiro.

<details>
  <summary>&nbsp;&nbsp;<strong>👀 Observações técnicas</strong></summary>

  - Tanto o quarto quanto o décimo terceiro registros, precisam aparecer na consulta;

  - Não use `where` ou `order by`.

  <br />
</details>

---
### 6 - Exiba os dados das colunas `product_name` e `id` da tabela `products` de maneira que os resultados estejam em ordem alfabética dos nomes.

  ---
### 7 - Mostre apenas os ids dos 5 últimos registros da tabela `products` (a ordem deve ser baseada na coluna `id`).

  ---
### 8 - Faça uma consulta que retorne três colunas, respectivamente, com os nomes 'A', 'Trybe' e 'eh', e com valores referentes a soma de '5 + 6', a string 'de', a soma de '2 + 8'.

<details>
  <summary>&nbsp;&nbsp;<strong>👀 Observações técnicas</strong></summary>

  - Na primeira coluna, exiba a soma de `5 + 6` (essa soma deve ser realizada pelo SQL);

  - Na segunda coluna deve haver a palavra \"de\";

  - E por fim, na terceira coluna, exiba a soma de `2 + 8` (essa soma deve ser realizada pelo SQL);

  - A primeira coluna deve se chamar \"A\", a segunda coluna deve se chamar \"Trybe\" e a terceira coluna deve se chamar \"eh\";

  - Não use colunas pré-existentes, apenas o que for criado na hora.

  <br />
</details>

## Desafios sobre filtragem de dados
### 9 - Mostre todos os valores de `notes` da tabela `purchase_orders` que não são nulos.

  ---
### 10 - Mostre todos os dados da tabela `purchase_orders` em ordem decrescente, ordenados por `created_by` em que o `created_by` é maior ou igual a 3.

  - Ordene também os resultados pelo `id` de forma crescente, como critério de desempate para a ordenação.

  ---
### 11 - Exiba os dados da coluna `notes` da tabela `purchase_orders` em que seu valor de `Purchase generated based on Order` é maior ou igual a 30 e menor ou igual a 39.

  ---
### 12 - Mostre as `submitted_date` de `purchase_orders` em que a `submitted_date` é do dia 26 de abril de 2006.

  ---
### 13 - Mostre o `supplier_id` das `purchase_orders` em que o `supplier_id` seja 1 ou 3.

  ---
### 14 - Mostre os resultados da coluna `supplier_id` da tabela `purchase_orders` em que o `supplier_id` seja maior ou igual a 1 e menor ou igual 3.

  ---
### 15 - Mostre somente as horas (sem os minutos e os segundos) da coluna `submitted_date` de todos registros da tabela `purchase_orders`.

  - No resultado, a hora extraída da coluna `submitted_date` deve ser chamada de `submitted_hour`.

  ---
### 16 - Exiba a `submitted_date` das `purchase_orders` que estão entre `2006-01-26 00:00:00` e `2006-03-31 23:59:59`.

  ---
### 17 - Mostre os registros das colunas `id` e `supplier_id` das `purchase_orders` em que os `supplier_id` sejam tanto 1, ou 3, ou 5, ou 7.

  ---
### 18 - Mostre todos os registros de `purchase_orders` que tem o `supplier_id` igual a 3 e `status_id` igual a 2.

  ---
### 19 - Mostre a quantidade de pedidos que foram feitos na tabela `orders` pelo `employee_id` igual a 5 ou 6, e que foram enviados através do método(coluna) `shipper_id` igual a 2.

  - No resultado, a coluna que contém a contagem de pedidos deve ser chamada de `orders_count`.

  ---

## Desafios de manipulação de tabelas
### 20 - Adicione à tabela `order_details` um registro com `order_id`: 69, `product_id`: 80, `quantity`: 15.0000, `unit_price`: 15.0000, `discount`: 0, `status_id`: 2, `date_allocated`: NULL, `purchase_order_id`: NULL e `inventory_id`: 129.
 
  ---
### 21 - Adicione com um único `INSERT`, duas linhas à tabela `order_details` com os mesmos dados do requisito 20.

<details>
  <summary><strong>👀 Observações técnicas</strong></summary>

  - O `ìd` deve ser incrementado automaticamente.
</details>

  ---
### 22 - Atualize os dados de `discount` do `order_details` para 15.

⚠️ Para testar, pode ser necessário utilização do SAFE UPDATE.

  ---
### 23 - Atualize os dados da coluna `discount` da tabela `order_details` para 30, onde o valor na coluna `unit_price` seja menor que 10.0000.

  ---
### 24 - Atualize os dados da coluna `discount` da tabela `order_details` para 45, onde o valor na coluna `unit_price` seja maior que 10.0000 e o id seja um número entre 30 e 40.

  ---
### 25 - Delete todos os dados em que a `unit_price` da tabela `order_details` seja menor que 10.0000.

  ---
### 26 - Delete todos os dados em que a `unit_price` da tabela `order_details` seja maior que 10.0000.

  ---
### 27 - Delete todos os dados da tabela `order_details`.

</details>

---
> Banco de dados `_northwind_` e `docker-compose.yml` fornecido pela Trybe.


[Docker-logo]: https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white
[Docker-url]: https://www.docker.com
[MySQL-logo]: https://img.shields.io/badge/mysql-%2300f.svg?style=for-the-badge&logo=mysql&logoColor=white
[MySQL-url]: https://www.mysql.com
[MySQL Workbench]: https://dev.mysql.com/downloads/workbench/
