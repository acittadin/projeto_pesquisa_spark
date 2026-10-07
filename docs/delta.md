# Delta Lake

## Visão Geral
O **Delta Lake** é uma camada de armazenamento de código aberto que traz confiabilidade para os Data Lakes. Construído sobre o formato de arquivos Parquet, ele adiciona uma camada de log de transações em formato JSON que gerencia o estado das tabelas e garante consistência em ambientes de processamento concorrente.

## Principais Mecanismos
O Delta Lake combina o armazenamento econômico de um data lake com a robustez transacional de um data warehouse. Os principais benefícios são:

* **Transações ACID:** Garante atomicidade, consistência, isolamento e durabilidade nas operações de escrita em tabelas no Data Lake.
* **Time Travel e Rollback:** Mantém um histórico de versões das transações, permitindo auditar alterações ou reverter estados em caso de falhas.
* **Otimização de Performance:** Utiliza o formato Parquet otimizado com metadados transacionais em JSON para consultas extremamente rápidas.

## Integração com o Spark
Como o Delta Lake é totalmente integrado ao ecosistema Spark, operações de leitura e escrita (`format("delta")`) tornam-se nativas e altamente otimizadas para fluxos de engenharia de dados modernos (arquitetura Medallion: camadas Bronze, Silver e Gold).
