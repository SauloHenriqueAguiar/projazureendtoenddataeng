# Projeto de Engenharia de Dados End-to-End com Microsoft Azure

Bem-vindo ao projeto de engenharia de dados end-to-end utilizando Microsoft Azure! Este repositório contém todos os detalhes e scripts necessários para configurar e executar um pipeline completo de engenharia de dados, desde a ingestão e transformação dos dados até a visualização dos resultados.

## Visão Geral

O objetivo deste projeto é criar um pipeline de dados robusto e eficiente, utilizando as seguintes ferramentas e serviços da Microsoft Azure:

- **Azure Data Factory (ADF)**: Para orquestração e automação de fluxos de dados.
- **Azure Key Vault**: Para gerenciamento seguro de segredos e credenciais.
- **Azure Subscription e Azure Storage Account**: Para gerenciar e armazenar dados.
- **Azure Databricks**: Para processamento e transformação avançada dos dados.
- **Power BI**: Para visualização e análise dos dados.

## Estrutura dos Containers

O pipeline de dados está dividido em três camadas principais de containers de armazenamento, representando diferentes estágios do processo de ETL (Extração, Transformação e Carga):

1. **Container Bronze**: Armazena os dados brutos e não processados. Aqui, os dados são ingeridos diretamente de suas fontes e armazenados para processamento futuro.

2. **Container Prata**: Armazena dados transformados e limpos. Após a transformação e limpeza, os dados são movidos para este container, onde podem ser usados para análises mais detalhadas e agregações.

3. **Container Ouro**: Armazena dados prontos para análise e relatórios. Este container contém os dados finais, preparados e otimizados para relatórios e dashboards em Power BI.

## Componentes do Projeto

- **Azure Data Factory (ADF)**: Configurado para orquestrar a movimentação de dados entre os containers, realizar transformações e garantir a execução dos pipelines de ETL.

- **Azure Key Vault**: Utilizado para armazenar e gerenciar credenciais e segredos necessários para acessar recursos e serviços Azure de forma segura.

- **Azure Databricks**: Utilizado para processamento de dados, criação de modelos de dados e execução de tarefas de transformação complexas.

- **Power BI**: Usado para criar dashboards e relatórios interativos, permitindo a visualização e análise dos dados processados.

## Configuração e Implementação

1. **Azure Subscription e Storage Account**: Configure uma conta de armazenamento e defina os containers Bronze, Prata e Ouro. Detalhes sobre a configuração podem ser encontrados [aqui](https://docs.microsoft.com/azure/storage/).

2. **Azure Key Vault**: Configure um cofre de chaves e adicione as credenciais necessárias. Mais informações estão disponíveis [aqui](https://docs.microsoft.com/azure/key-vault/).

3. **Azure Data Factory**: Crie e configure pipelines de ETL para mover dados entre os containers e executar transformações. Consultar a documentação [aqui](https://docs.microsoft.com/azure/data-factory/).

4. **Azure Databricks**: Configure clusters e notebooks para processamento de dados. Detalhes estão disponíveis [aqui](https://docs.microsoft.com/azure/databricks/).

5. **Power BI**: Conecte-se aos dados no container Ouro e crie relatórios e dashboards. Veja mais informações [aqui](https://docs.microsoft.com/power-bi/).
