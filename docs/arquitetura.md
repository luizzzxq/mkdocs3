# Arquitetura do Projeto

O projeto segue a arquitetura medalhão utilizando Databricks e Delta Lake.

O fluxo inicia com a extração dos dados de um banco de dados relacional ou não relacional. 
Esses dados são armazenados no schema LANDING/DADOS nos formatos CSV (relacional) ou JSON (não relacional).

Na camada BRONZE, os arquivos CSV ou JSON são lidos e convertidos para o formato Delta Lake, mantendo os dados em estado bruto para persistência e rastreabilidade.

Na camada SILVER, são aplicadas regras de Data Quality, como remoção de valores nulos, tratamento de duplicidades e padronização de dados, garantindo maior confiabilidade das informações.

Na camada GOLD, os dados tratados são organizados em modelo dimensional, contendo tabelas fato e dimensão conforme a abordagem de Ralph Kimball.

Todo o processo é executado de forma sequencial através de Jobs & Pipelines do Databricks, garantindo automação do pipeline de dados.