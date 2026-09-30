# Análise de Vendas de Chocolate

Projeto desenvolvido em Python para realizar o tratamento, organização e análise de uma base de dados de vendas de chocolates.

O projeto utiliza **Pandas** para manipulação dos dados e **Plotly** para criação de visualizações, permitindo analisar a evolução das vendas ao longo do tempo e o desempenho dos produtos.

## Objetivo

O objetivo do projeto é explorar uma base de dados de vendas e obter informações sobre:

* Evolução das vendas por mês;
* Evolução das vendas por ano;
* Ticket médio anual;
* Crescimento percentual do valor das vendas;
* Desempenho dos produtos ao longo dos anos.

## Base de Dados

A base `Vendas_Chocolate.csv` contém informações sobre as vendas realizadas, incluindo:

* **Vendedor**
* **País**
* **Produto**
* **Data**
* **Valor**
* **Caixas Enviadas**
* **Data de Hoje**

A base original possui **3.282 registros** e, após o processo de tratamento, são utilizados **3.155 registros** para a análise.

## Tecnologias e Bibliotecas

* Python
* Pandas
* Plotly

## Tratamento dos Dados

Antes das análises, foram realizados alguns procedimentos de limpeza e preparação dos dados:

1. Identificação das informações da base;
2. Remoção da coluna `Data de Hoje`;
3. Remoção de registros com valores vazios;
4. Conversão da coluna `Data` para o formato de data;
5. Tratamento da coluna `Valor`, removendo o símbolo `$` e separadores;
6. Conversão dos valores de vendas para o formato numérico;
7. Remoção de registros duplicados;
8. Reorganização dos índices da tabela.

## Criação de Variáveis

Foram criadas duas novas colunas para facilitar a análise:

* **Mes** — representa o mês da venda;
* **Ano** — representa o ano da venda.

## Análises Realizadas

### Vendas por mês

Os valores das vendas são agrupados por mês para analisar a evolução das vendas ao longo do período.

Um gráfico de barras é utilizado para visualizar os valores de vendas de cada mês.

### Vendas por ano

As vendas são agrupadas por ano, permitindo analisar:

* Valor total das vendas;
* Quantidade de caixas enviadas;
* Ticket médio;
* Crescimento percentual do valor das vendas.

O **Ticket Médio** é calculado pela relação entre o valor total das vendas e a quantidade de caixas enviadas:

```text
Ticket Médio = Valor Total / Caixas Enviadas
```

Também é calculado o crescimento percentual do valor das vendas entre os anos.

### Vendas por produto

As vendas são agrupadas por **ano e produto**, permitindo comparar o valor vendido por cada produto ao longo dos anos.

Um gráfico de barras é utilizado para visualizar essa comparação.

## Estrutura do Projeto

```text
projeto-analise-vendas-chocolate
│
├── codigo_chocolate.ipynb
├── Vendas_Chocolate.csv
└── README.md
```

## Como Executar

### 1. Clone o repositório

```bash
git clone URL_DO_SEU_REPOSITORIO
```

### 2. Instale as bibliotecas necessárias

```bash
pip install pandas plotly
```

### 3. Abra o notebook

Abra o arquivo:

```text
codigo_chocolate.ipynb
```

## Principais conceitos utilizados

Este projeto permite praticar conceitos importantes de análise de dados, como:

* Leitura de arquivos CSV;
* Limpeza e tratamento de dados;
* Tratamento de valores ausentes;
* Conversão de tipos de dados;
* Remoção de duplicidades;
* Manipulação de datas;
* Agrupamento de dados com `groupby()`;
* Criação de novas variáveis;
* Cálculo de métricas;
* Visualização de dados com gráficos;
* Análise de crescimento de vendas.

## Autora

Cristina Yuki Yokomizo

🤝 Contribuições são sempre bem-vindas!
