# Silver Layer

## Data Quality e Tratamento dos Dados

A camada Silver é responsável pelo tratamento e refinamento dos dados provenientes da camada Bronze. Nessa etapa, foram aplicadas regras de Data Quality com o objetivo de garantir maior consistência, padronização e confiabilidade das informações utilizadas no pipeline.

Entre as validações aplicadas podem estar remoção de valores nulos, tratamento de duplicidades, correção de tipos de dados e aplicação de regras de negócio. Essas verificações são extremamente importantes para evitar problemas futuros durante análises e processos de tomada de decisão. Dados inconsistentes podem comprometer toda a qualidade de um projeto analítico.

Após o processamento, os dados tratados foram gravados em um novo schema chamado SILVER. Diferente da Bronze, a camada Silver já contém dados considerados confiáveis e preparados para consumo interno dentro do ambiente analítico. Essa camada normalmente é utilizada como base para relatórios operacionais e integrações.

A implementação da camada Silver também demonstra a importância do conceito de refinamento gradual presente na arquitetura Medalhão. Em vez de realizar todas as transformações de uma única vez, o pipeline organiza o fluxo em etapas menores e mais controladas, facilitando manutenção, testes e monitoramento.