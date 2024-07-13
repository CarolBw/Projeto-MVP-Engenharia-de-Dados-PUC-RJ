
# Projeto-MVP-Engenharia-de-Dados-PUC-RJ

## MVP - Análise da Variação do Dirham e Correlações com a Temperatura de Dubai ao Longo de 10 Anos

Este projeto visa a criação de um pipeline de dados automatizado para analisar a variação da moeda Dirham (UAE) ao longo de 10 anos, compreendendo seus padrões anuais e a existência de relação de sua variação com a temperatura na cidade de Dubai (UAE). Utilizando um esquema estrela em um Data Warehouse no PostgreSQL, extraímos, limpamos, transformamos e carregamos os dados históricos da moeda e da temperatura. A automatização do pipeline será realizada com o Apache Airflow, garantindo a atualização contínua dos dados.

Os resultados serão apresentados através de dashboards facilitando a visualização e interpretação dos padrões sazonais e anuais, bem como a correlação entre o valor do Dirham e a temperatura. A utilização do GitHub assegura um controle de versão eficiente ao longo do desenvolvimento do projeto.

Esta abordagem integrada foi estabelecida de acordo com os critérios predefinidos para o projeto MVP de Engenharia de Dados da PUC-RJ.

## Objetivo

- Analisar a variação do Dirham (AED) ao longo de 10 anos.
- Identificar padrões anuais e sazonais.
- Verificar se há correlação entre a variação do Dirham e a temperatura em Dubai.
- Converter o Dirham para o Real Brasileiro (BRL) para facilitar a apresentação dos resultados.
- Automatizar o pipeline de dados utilizando Apache Airflow.
- Criar um Data Warehouse com esquema estrela para facilitar análises OLAP.
- Apresentar os resultados de forma clara e visualmente atraente através de dashboards.

## Perguntas do Negócio

- Quais são as variações sazonais do Dirham ao longo dos anos?
- Como a taxa de câmbio do Dirham se relaciona com a temperatura em Dubai?
- Quais são os padrões mensais e anuais na taxa de câmbio do Dirham?
- Há correlação entre a variação do Dirham e a temperatura em Dubai?
- Previsão do valor do Dirham para os próximos meses em relação ao Real Brasileiro.

## Dados Necessários

- Valor da moeda Dirham (UAE) nos últimos 10 anos.
- Dados de temperatura dos últimos 10 anos na cidade de Dubai.

## Escopo

- Extração de dados históricos da moeda.
- Extração dos dados de temperatura.
- Mesclagem de dados.
- Limpeza e transformação dos dados.
- Carga em um Data Warehouse com esquema estrela.
- Realizar análise OLAP.
- Criar Dashboards para visualização.
- Criar um modelo preditivo.
- Apresentação de resultados.

## Ferramentas e Serviços Utilizados

- Google Cloud Storage (GCS): Armazenamento de dados brutos.
- Cloud Composer: Orquestração do pipeline de dados com Apache Airflow.
- Google BigQuery: Data Warehouse para armazenamento e análise de dados.
- PostgreSQL: Banco de dados relacional para armazenar dados no data warehouse.
- Apache Spark: Processamento de dados.
- Google Colab: Ambiente de desenvolvimento em nuvem.
- Bibliotecas Básicas para manipulação e visualização de dados.
- GitHub: Controle de versão.

## Fluxo do Pipeline

- Fonte de Dados: APIs Yahoo Finance (moedas) e Meteostat (temperatura).

1. Extração:
  - Cloud Composer DAG: Inicia a extração periódica de dados.
  - Google Cloud Storage (GCS): Armazenamento de Dados Brutos (Armazena arquivos CSV/JSON com dados extraídos).

2. Processamento e Transformação:
  - Colaboratory com Spark: Lê os dados brutos do GCS, realiza transformações e salva dados transformados no PostgreSQL e BigQuery.

3. Carregamento de Dados Preparados:
  - PostgreSQL: Armazena dados transformados para análises no data warehouse.
  - BigQuery: Importa dados transformados do GCS, cria um esquema estrela para análises OLAP (tabelas de fato e dimensões).

4. Análise e Visualização:
  - BigQuery: Realiza consultas analíticas para análise de correlação entre Dirham, dólar, real e temperaturas de Dubai.
  - Cloud Composer: Gerencia o fluxo de trabalho completo, agendando e orquestrando os processos no Apache Airflow.

## Licença

Este projeto está licenciado sob a Licença Creative Commons Attribution-NonCommercial-ShareAlike (CC BY-NC-SA). Você pode encontrar mais informações em [Creative Commons](https://br.creativecommons.net/?s=CC+BY-NC-SA).
