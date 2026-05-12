# Jobs & Pipelines

## Encadeamento e Automação das Execuções

Após a construção de todas as camadas da arquitetura Medalhão, foi necessário automatizar a execução completa do pipeline utilizando os recursos de Jobs & Pipelines do Databricks. Cada notebook desenvolvido no projeto foi organizado em uma sequência lógica de execução, garantindo que as etapas fossem processadas na ordem correta.

O fluxo automatizado inicia com a extração dos dados para a camada Landing, seguida pela ingestão para a Bronze, aplicação de regras de qualidade na Silver e, por fim, carregamento das tabelas dimensionais na Gold. Esse encadeamento garante que cada etapa utilize dados já processados e validados pela etapa anterior, reduzindo inconsistências no pipeline.

A utilização de Jobs trouxe maior controle operacional ao projeto, permitindo monitorar execuções, identificar falhas e registrar logs detalhados de cada etapa. Além disso, o Databricks possibilita configurar dependências entre tarefas, criando pipelines mais organizados e próximos de ambientes produtivos utilizados em empresas.

Outro benefício importante da automação foi a redução de processos manuais repetitivos. Com todas as etapas encadeadas automaticamente, o pipeline se tornou mais eficiente, padronizado e escalável. Isso permite futuras melhorias no projeto, como inclusão de novas fontes de dados, novas regras de transformação ou integração com ferramentas analíticas.