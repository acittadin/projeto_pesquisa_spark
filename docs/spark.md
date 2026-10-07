# Apache Spark e PySpark

## Visão Geral
O **Apache Spark** é um motor de processamento distribuído de código aberto projetado para lidar com cargas de trabalho de Big Data em larga escala. Diferente do modelo tradicional do MapReduce baseados em disco, o Spark utiliza o conceito de **RDD (Resilient Distributed Dataset)** e computação em memória (*in-memory*), o que acelera drasticamente a execução de pipelines analíticos, machine learning e processamento de streams.

## Papel no Arquitetura do Projeto
O **PySpark** (uma API em Python para o Spark) atua como o motor central da nossa arquitetura. Ele é responsável por:

* **Ingestão Distribuída:** Ler grandes volumes de dados brutos de forma paralela.
* **Transformações e Limpeza:** Aplicar regras de negócio, limpeza e normalização utilizando DataFrames otimizados.
* **Escrita em Formatos Modernos:** Persistir os dados processados em camadas otimizadas utilizando os formatos **Delta Lake** e **Apache Iceberg**.

## Vantagens Chave
* **Performance:** Processamento em memória que reduz o I/O de disco.
* **Ecossistema Unificado:** Integração nativa com SQL, streaming, aprendizado de máquina (MLlib) e graph analytics.
* **Escalabilidade:** Capacidade de escalar horizontalmente em clusters para processar terabytes ou petabytes de dados.

