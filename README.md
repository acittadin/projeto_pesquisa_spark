# PySpark/Delta Lake/Apache Iceberg

Um ambiente simples para aprender e experimentar com **PySpark 3.4.2** e **Delta Lake 2.4.0**, usando **Poetry** para gerenciamento de dependências.

## Requisitos

Antes de começar, certifique-se de ter:

- [Linux / WSL](https://learn.microsoft.com/pt-br/windows/wsl/install)
- [Java 17](https://linuxvox.com/blog/how-to-install-java-on-linux/)
- [Python 3.11](https://python.org.br/instalacao-linux/)
- [Poetry](https://python-poetry.org/docs/)

> Esse Projeto Usa PySpark 3.4.2 e Delta Lake 2.4.0.

## 1. Clone o repositório

```bash
git clone https://github.com/acittadin/projeto_pesquisa_spark.git
cd projeto_pesquisa_spark
```

## 2. Instalar dependencias

Instale as dependencias do projeto com Poetry:

```bash
poetry install
```

As dependências principais  são:

```text
PySpark     3.4.2
Delta Lake  2.4.0
```

Verifique os pacotes com:

```bash
poetry show
```

## 3. JupyterLab
Jupyter não é necessário para PySpark ou Delta Lake, porém sera usado nesse projeto como uma ferramenta.

Instale-o com:

```bash
poetry add jupyterlab
```

E inicie com:

```bash
poetry run jupyter lab
```


## Versões

| Componentes | Versões |
|---|---:|
| Python | 3.11 |
| PySpark | 3.4.2 |
| Delta Lake | 2.4.0 |
| Scala | 2.12 |
| Java | 17 |
| Gerenciador de Dependencias | Poetry |

## License

Add your project's license here.
