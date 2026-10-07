# Apache Iceberg

## Visão Geral
O **Apache Iceberg** é um formato de tabela de alto desempenho projetado para grandes conjuntos de dados analíticos em um Data Lake. Ele traz a confiabilidade e a simplicidade de um banco de dados relacional tradicional (como suporte a transações ACID e evolução de esquema) diretamente para arquivos armazenados em object storage (como S3, ADLS ou GCS).

## Características Técnicas
O Iceberg gerencia arquivos através de um catálogo e árvores de metadados, separando o planejamento da consulta dos dados brutos. Suas principais características incluem:

* **Evolução de Esquema:** Permite alterar colunas (adicionar, remover ou renomear) de forma segura sem reescrever os arquivos de dados subjacentes.
* **Gerenciamento de Partições Oculto:** O motor de processamento lida com o particionamento automaticamente, livrando o usuário de especificar filtros rígidos nas consultas.
* **Viagem no Tempo (Time Travel):** Possibilidade de consultar snapshots históricos dos dados para auditoria e reproducibilidade.

## Benefícios no Projeto
A utilização do Apache Iceberg no projeto garante que consultas analíticas pesadas executadas pelo Spark encontrem dados consistentes, particionados de forma eficiente e protegidos contra problemas de concorrência.
