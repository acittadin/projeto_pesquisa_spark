# Delta Lake

O **Delta Lake** é uma camada de armazenamento de código aberto que traz confiabilidade, segurança e desempenho para Data Lakes baseados em nuvem ou ambientes locais.

## Pilares Tecnológicos
* **Transações ACID:** Garante consistência total (Atomicidade, Consistência, Isolamento e Durabilidade) em operações de leitura e escrita concorrentes.
* **Delta Log (Log de Transações):** Um registro JSON ordenado que rastreia atômicamente todas as adições e remoções de arquivos, eliminando visualizações parciais ou corrompidas.
* **Otimização e Compactação:** Oferece recursos nativos como *OPTIMIZE* (compactação de arquivos pequenos) e *VACUUM* (limpeza de versões antigas obsoletas).

## Aplicação no Projeto
Utilizamos o Delta Lake para viabilizar operações **DML seguras** (como `UPDATE`, `DELETE` e `MERGE INTO`), permitindo gerenciar atualizações incrementais de dados com a mesma facilidade de um banco de dados relacional tradicional.# Delta Lake

O Delta Lake é um projeto de código aberto que adiciona uma camada de confiabilidade e desempenho em cima de Data Lakes existentes. 

Suas principais características que estamos demonstrando neste projeto incluem:
* **Delta Log:** Um log de transações que rastreia todas as alterações feitas na tabela, garantindo a confiabilidade dos dados.
* **Operações DML Seguras:** Graças ao log, podemos executar comandos robustos de UPDATE, DELETE e MERGE sem risco de quebrar o sistema.
