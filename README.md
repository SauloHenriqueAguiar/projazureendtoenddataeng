# Projeto de Engenharia de Dados End-to-End com Microsoft Azure

Bem-vindo ao projeto de engenharia de dados end-to-end utilizando Microsoft Azure! Este repositório contém todos os detalhes e scripts necessários para configurar e executar um pipeline completo de engenharia de dados, desde a ingestão e transformação dos dados até a visualização dos resultados.

## Visão Geral

O objetivo deste projeto é criar um pipeline de dados robusto e eficiente, utilizando as seguintes ferramentas e serviços da Microsoft Azure:

- **SQL Server On-Premises**: Fonte primária de dados.
- **Azure Data Factory (ADF)**: Para ingestão e orquestração dos dados.
- **Azure Databricks**: Para transformação dos dados nas camadas Bronze, Prata e Ouro.
- **Azure Synapse Analytics**: Para carregamento e análise de dados.
- **Azure Key Vault e Active Directory (AD)**: Para segurança e governança dos dados.
- **Power BI**: Para visualização e relatórios dos dados.

## Estrutura do Pipeline

O pipeline de dados é dividido nas seguintes etapas:

1. **Ingestão de Dados**:
   - **Fonte**: SQL Server On-Premises.
   - **Ferramenta**: Azure Data Factory.
   - **Descrição**: Dados são extraídos do SQL Server On-Premises e movidos para o Azure Data Factory para orquestração e ingestão.

2. **Transformação de Dados**:
   - **Ferramenta**: Azure Databricks.
   - **Camadas**:
     - **Bronze**: Armazena os dados brutos e não processados.
     - **Prata**: Armazena dados transformados e limpos.
     - **Ouro**: Armazena dados finais, preparados para análises e relatórios.

3. **Carregamento e Análise**:
   - **Ferramenta**: Azure Synapse Analytics.
   - **Descrição**: Dados transformados são carregados no Azure Synapse Analytics para análises avançadas e consultas.

4. **Segurança e Governança**:
   - **Ferramentas**: Azure Key Vault e Active Directory (AD).
   - **Descrição**: Garantia de segurança dos dados e gerenciamento de permissões e credenciais.

5. **Visualização e Relatórios**:
   - **Ferramenta**: Power BI.
   - **Descrição**: Criação de dashboards e relatórios interativos para análise e visualização dos dados.

## Configuração e Implementação

1. **Configuração do SQL Server On-Premises**: Certifique-se de que os dados estejam acessíveis e prontos para serem ingeridos.

2. **Azure Data Factory (ADF)**:
   - Configure pipelines de ingestão para mover dados do SQL Server para o Azure Databricks.
   - Mais informações [aqui](https://docs.microsoft.com/azure/data-factory/).

3. **Azure Databricks**:
   - Configure clusters e notebooks para processar dados nas camadas Bronze, Prata e Ouro.
   - Detalhes disponíveis [aqui](https://docs.microsoft.com/azure/databricks/).

4. **Azure Synapse Analytics**:
   - Carregue os dados transformados para o Azure Synapse para análises e consultas.
   - Saiba mais [aqui](https://docs.microsoft.com/azure/synapse-analytics/).

5. **Azure Key Vault e Active Directory**:
   - Configure o Key Vault para armazenar e gerenciar credenciais e segredos.
   - Gerencie permissões e autenticações com o Active Directory.
   - Mais informações sobre o Key Vault [aqui](https://docs.microsoft.com/azure/key-vault/), e sobre o AD [aqui](https://docs.microsoft.com/azure/active-directory/).

6. **Power BI**:
   - Conecte-se aos dados no Azure Synapse e crie relatórios e dashboards interativos.
   - Detalhes disponíveis [aqui](https://docs.microsoft.com/power-bi/).
