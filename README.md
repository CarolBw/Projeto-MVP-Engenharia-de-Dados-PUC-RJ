# Projeto-MVP-Engenharia-de-Dados-PUC-RJ
Projeto de Conclusão de Curso Engenharia de Dados PUC-RJ

### MVP - Análise da Variação do Dirham e Correlações com a Temperatura de Dubai ao Longo de 10 Anos 

Este projeto visa a criação de um pipeline de dados robusto e automatizado para analisar a variação da moeda Dirham (UAE) ao longo de 10 anos, compreendendo seus padroes anuais e a existencia de relação de sua variação com a temperatura na cidade de Dubai (UAE). Utilizando um esquema estrela em um Data Warehouse no PostgreSQL hospedado no AWS RDS, extraímos, transformamos e carregamos os dados históricos da moeda e da temperatura. A automatização do pipeline será realizada com o Apache Airflow, garantindo a atualização contínua dos dados. 

Os resultados serão apresentados através de dashboards no Tableau, facilitando a visualização e interpretação dos padrões sazonais e anuais, bem como a correlação entre o valor do Dirham e a temperatura. A utilização do GitHub para controle de versão assegura a reprodutibilidade e a colaboração eficiente ao longo do desenvolvimento do projeto. 

Esta abordagem integrada foi estabelecida de acordo com os critérios  predefinidos para o projeto MVP de Engenharia de Dados da PUC_RJ. 

### Objetivo 

Analisar a variação do Dirham (AED) ao longo de 10 anos. 

Identificar padrões anuais e sazonais. 

Verificar se há correlação entre a variação do Dirham e a temperatura em Dubai. 

Converter o Dirham para o Real Brasileiro (BRL) para facilitar a apresentação dos resultados. 

Automatizar o pipeline de dados utilizando Apache Airflow. 

Criar um Data Warehouse com esquema estrela para facilitar análises OLAP. 

Apresentar os resultados de forma clara e visualmente atraente através de dashboards. 

 
### Perguntas do Negócio 

Quais são as variações sazonais do Dirham ao longo dos anos? 

Como a taxa de câmbio do Dirham se relaciona com a temperatura em Dubai? 

Quais são os padrões mensais e anuais na taxa de câmbio do Dirham? 

Há correlação entre a variação do Dirham e a temperatura em Dubai? 

Previsão do valor do Dirham para os próximos meses em relação ao Real Brasileiro. 


### Dados Necessários 

Valor da moeda Dirham (UAE) nos últimos 10 anos. 

Dados de temperatura dos últimos 10 anos na cidade de Dubai. 


### Escopo 

Extração de dados históricos da moeda. 

Extração dos dados de temperatura. 

Transformação dos dados. 

Carga em um Data Warehouse com esquema estrela. 

Realizar análise OLAP. 

Criar Dashboards para visualização. 

Criar um modelo preditivo. 

Apresentação de resultados 


### Ferramentas  

Ambiente de Desenvolvimento: Google Colab 

Linguagem: Python e SQL 

ETL: Apache Spark e pandas 

Banco de Dados: PostgreSQL no AWS RDS 

Data Warehouse: Esquema Estrela 

OLAP: Abordagem OLAP com consultas SQL 

Dashboards de Visualização: Tableau 

Execução Automatizada: Apache Airflow 

Controle de Versão: GitHub


Este projeto esta licenciado sobre a Licença Creative Commons Attribution-NonCommercial-ShareAlike (CC BY-NC-SA).
Você pode encontrar maiores informações em (https://br.creativecommons.net/?s=CC+BY-NC-SA).
 

 
