# Apache Spark (PySpark)

O **Apache Spark** é um motor de processamento unificado, ultrarrápido e de código aberto, projetado para processamento de dados em larga escala e computação em cluster.

## Papel no Projeto
O **PySpark** (a API em Python para o Spark) atua como o motor central da nossa arquitetura. Ele é responsável por:
* **Ingestão Distribuída:** Ler grandes volumes de dados brutos de forma paralela.
* **Transformações e Limpeza:** Aplicar regras de negócio, limpeza e normalização utilizando DataFrames otimizados.
* **Escrita em Formatos Modernos:** Persistir os dados processados em camadas otimizadas utilizando os formatos **Delta Lake** e **Apache Iceberg**.

## Vantagens Arquiteturais
* **Processamento em Memória (In-Memory):** Reduz drasticamente as operações de I/O em disco comparado ao MapReduce tradicional.
* **Tolerância a Falhas:** O RDD (Resilient Distributed Dataset) garante a recuperação automática de partições perdidas em nós do cluster.# Apache Spark (PySpark)

O Apache Spark é um motor de processamento unificado, ultrarrápido e de código aberto, voltado para processamento de dados em larga escala. 

O **PySpark** é a interface (API) em Python para o Apache Spark. Ele é o "coração" do nosso projeto, sendo o responsável por ler os conjuntos de dados, executar as transformações necessárias e escrevê-los nos formatos otimizados de forma distribuída.
