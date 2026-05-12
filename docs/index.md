# Introdução

## Visão Geral do Projeto

Este projeto teve como objetivo desenvolver um pipeline de dados completo utilizando a arquitetura Medalhão dentro da plataforma Databricks. A solução foi construída seguindo um modelo de processamento em múltiplas camadas, permitindo separar dados brutos, dados tratados e dados analíticos de maneira organizada e escalável. O fluxo foi estruturado utilizando as camadas Landing, Bronze, Silver e Gold, além da automação com Jobs & Pipelines.

A arquitetura Medalhão é amplamente utilizada em projetos modernos de Engenharia de Dados por oferecer maior controle sobre o ciclo de vida das informações. Cada camada possui uma responsabilidade específica dentro do pipeline, permitindo melhor governança, rastreabilidade e qualidade dos dados. Essa divisão também facilita manutenção, monitoramento e futuras expansões do projeto.

O pipeline foi implementado no Databricks utilizando Delta Lake como tecnologia principal de armazenamento. A utilização do Delta Lake trouxe vantagens importantes, como suporte a transações ACID, versionamento de dados e melhor desempenho em operações analíticas. Além disso, o ambiente Databricks permitiu integrar notebooks, automações e processamento distribuído em uma única plataforma.

Durante o desenvolvimento, foram aplicados conceitos de ingestão de dados, transformação, Data Quality, modelagem dimensional e automação de workflows. O projeto buscou reproduzir um cenário próximo de ambientes corporativos reais, demonstrando como pipelines modernos podem transformar dados brutos em informações organizadas e preparadas para análise estratégica.