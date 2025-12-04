# Laboratório de Banco de Dados

Este repositório contém os scripts e documentação desenvolvidos para a disciplina de Laboratório de Banco de Dados. O projeto abrange desde a modelagem e criação do banco de dados relacional até a implementação de auditoria, historiamento e criação de um Data Warehouse para Business Intelligence.

---

## Credenciais de Acesso

Para execução inicial e configuração do ambiente:

| Usuário | Senha |
| :--- | :--- |
| **system** | `12345` |

---

## Estrutura do Projeto e Entregas

O desenvolvimento do projeto foi dividido em 5 entregas estratégicas, conforme detalhado abaixo:

### Entrega 1: Modelagem e Implementação Relacional
Foco na estruturação inicial do banco de dados e garantia da integridade dos dados.
- **Normalização:** Tratamento do dataset original para adequação às formas normais.
- **Dicionário de Dados:** Documentação completa dos metadados.
- **Estrutura:** Criação de tabelas, *sequences* e *triggers* básicas.
- **Carga de Dados:** Povoamento inicial da base.
- **Consultas:** Implementação de consultas estratégicas operacionais.

### Entrega 2: Historiamento de Dados
Implementação de mecanismos para rastrear mudanças nos dados ao longo do tempo.
- **Tabelas de Histórico:** Estruturas espelho para armazenar versões anteriores dos registros.
- **Automação:** Criação de *triggers* específicas para controlar o fluxo de historiamento.
- **Carga Histórica:** Processamento das cargas de dados subsequentes mantendo o rastro temporal.

### Entrega 3: Auditoria de Sistema
Desenvolvimento de uma camada de segurança e monitoramento para rastrear operações de usuários.
- **Ambiente Dedicado:** Criação de usuário e tabelas específicas para auditoria.
- **Monitoramento:** Implementação de *triggers* e *procedures* (`PROC_AUDITORIA`) para registrar operações de `INSERT`, `UPDATE` e `DELETE`.
- **Validação:** Testes de auditoria para garantir que todas as modificações críticas sejam logadas.

### Entrega 4: Data Warehouse (DW)
Preparação do ambiente para análise de dados e suporte à decisão.
- **Usuário DW:** Configuração do ambiente para o Data Warehouse (`DWUSER`).
- **Views Dinâmicas:** Criação de visualizações para simplificar o acesso aos dados (`VIEW_TODOS_VEICULOS_ENVOLVIDOS`, etc.).
- **Views Materializadas:** Otimização de consultas pesadas através de *Materialized Views* para relatórios de performance (ex: Acidentes por Rodovia, Condições Climáticas).
- **Consultas Analíticas:** Desenvolvimento de consultas complexas focadas em inteligência de dados.

### Entrega 5: Business Intelligence
Visualização e análise final dos dados processados.
- **Dashboard:** Desenvolvimento de painéis interativos utilizando Power BI.
- **Certificação:** Validação de conhecimentos na ferramenta de BI.

---

## Processo de Instalação e Configuração

Para configurar o ambiente de desenvolvimento, siga a ordem de execução dos scripts disponíveis na pasta `scripts/` ou `Entrega_X/`:

### 1. Configuração Inicial
Execute o script de configuração para preparar o ambiente e o usuário principal.
> Arquivo: `scripts/00_database_config.sql`

### 2. Importação de Dados
Para realizar a carga dos dados:
1.  Certifique-se de que os arquivos `.csv` (Datasets) estão acessíveis.
2.  Execute os scripts de criação de tabelas e importação na ordem numérica fornecida nas pastas de entrega.

## Desenvolvedores

- **Daniel Andrade**  
- **Bruno Rodrigues**
