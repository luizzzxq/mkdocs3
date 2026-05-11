# Início

Este projeto tem como objetivo implementar uma arquitetura Lakehouse utilizando o Databricks Free Edition e o modelo medalhão (Medallion Architecture).

O pipeline realiza a extração de dados de um banco de dados relacional ou não relacional, armazenando inicialmente os arquivos na camada LANDING/DADOS nos formatos CSV ou JSON. Em seguida, os dados são convertidos para Delta Lake na camada BRONZE, permitindo maior organização e desempenho no processamento.

Na camada SILVER, são aplicadas regras de qualidade de dados (Data Quality), garantindo maior consistência e confiabilidade das informações. Posteriormente, os dados tratados são estruturados na camada GOLD utilizando modelagem dimensional baseada em Ralph Kimball.

Todo o fluxo é automatizado através de Jobs & Pipelines do Databricks, permitindo a execução sequencial dos notebooks responsáveis por cada etapa do processo.

## Estrutura do Projeto

- LANDING: armazenamento inicial dos arquivos CSV/JSON
- BRONZE: dados brutos em Delta Lake
- SILVER: dados tratados e validados
- GOLD: tabelas fato e dimensão para análise