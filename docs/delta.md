# Delta Lake

O Delta Lake é um projeto de código aberto que adiciona uma camada de confiabilidade e desempenho em cima de Data Lakes existentes. 

Suas principais características que estamos demonstrando neste projeto incluem:
* **Delta Log:** Um log de transações que rastreia todas as alterações feitas na tabela, garantindo a confiabilidade dos dados.
* **Operações DML Seguras:** Graças ao log, podemos executar comandos robustos de UPDATE, DELETE e MERGE sem risco de quebrar o sistema.
