# PySpark / Delta Lake / Apache Iceberg

Um ambiente de pesquisa e experimentação construído para demonstrar e comparar o uso de **PySpark 3.4.2** com **Delta Lake 2.4.0** e **Apache Iceberg 1.4.1**, utilizando **Poetry** para o gerenciamento de dependências.

## Requisitos

Ambas as tecnologias (Delta e Iceberg) rodam sobre o mesmo motor (Apache Spark) e requerem a mesma infraestrutura base. Antes de começar, certifique-se de ter:

- [Linux / WSL](https://learn.microsoft.com/pt-br/windows/wsl/install)
- [Java 17](https://linuxvox.com/blog/how-to-install-java-on-linux/)
- [Python 3.11](https://python.org.br/instalacao-linux/) *(Nota: PySpark 3.4.2 é incompatível com Python 3.12+)*
- [Poetry](https://python-poetry.org/docs/)

> **Stack do Projeto:** PySpark 3.4.2 | Delta Lake 2.4.0 | Apache Iceberg 1.4.1

## 1. Clone o repositório

```bash
git clone [https://github.com/acittadin/projeto_pesquisa_spark.git](https://github.com/acittadin/projeto_pesquisa_spark.git)
cd projeto_pesquisa_spark
```

## 2. Instalar dependências (Poetry)

O gerenciamento de pacotes Python é feito exclusivamente com o Poetry. Crie o ambiente e instale as dependências com:

```bash
poetry env use python3.11
poetry install
```

### 💡 Diferença crucial: Como o Delta e o Iceberg são carregados?
Para que as duas ferramentas funcionem no mesmo projeto, adotamos abordagens diferentes e complementares:
*   **Delta Lake:** Instalado como um pacote Python (`delta-spark 2.4.0`) diretamente pelo Poetry.
*   **Apache Iceberg:** Não requer um pacote Python separado no Poetry. Ele é baixado dinamicamente em tempo de execução via dependência Maven (`org.apache.iceberg:iceberg-spark-runtime-3.4_2.12:1.4.1`) nas configurações da `SparkSession` dentro do notebook.

Verifique os pacotes Python instalados com:
```bash
poetry show
```

## 3. JupyterLab e Organização do Código

O JupyterLab não é obrigatório para o PySpark, mas será usado neste projeto como a interface interativa para documentar os Modelos ER, os códigos DDL e as operações DML.

Adicione e inicie o JupyterLab no ambiente do Poetry:
```bash
poetry add jupyterlab
poetry run jupyter lab
```

### 📂 Estrutura de Testes
O projeto está dividido em notebooks distintos para separar os contextos:
*   `delta.ipynb`: Demonstração da criação de tabelas e operações DML utilizando a API de DataFrames do Delta Lake.
*   `iceberg.ipynb`: Demonstração equivalente utilizando Spark SQL puro focado no formato Apache Iceberg.

## Versões

| Componente | Versão |
|---|---:|
| **Python** | 3.11 |
| **PySpark** | 3.4.2 |
| **Delta Lake** | 2.4.0 |
| **Apache Iceberg** | 1.4.1 |
| **Scala** | 2.12 |
| **Java** | 17 |
| **Gerenciador de Dependências** | Poetry |

## Licença

Adicione a licença do projeto aqui.