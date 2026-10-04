# PySpark + Delta Lake

A simple environment for learning and experimenting with **PySpark 3.4.2** and **Delta Lake 2.4.0**, using **Poetry** for dependency management.

## Requirements

Before starting, make sure you have:

- [Linux / WSL](https://learn.microsoft.com/pt-br/windows/wsl/install)
- [Java 17](https://linuxvox.com/blog/how-to-install-java-on-linux/)
- Python 3.11
- Poetry

> This project uses PySpark 3.4.2 and Delta Lake 2.4.0.

## 1. Install Java

Check if Java is already installed:

```bash
java -version
```

If it isn't installed, on Ubuntu:

```bash
sudo apt update
sudo apt install openjdk-17-jdk
```

Verify:

```bash
java -version
```

## 2. Install Poetry

If Poetry isn't installed, follow the official installation instructions:

https://python-poetry.org/docs/#installation

Verify the installation:

```bash
poetry --version
```

## 3. Clone the project

```bash
git clone https://github.com/acittadin/projeto_pesquisa_spark.git
cd projeto_pesquisa_spark
```

## 4. Install dependencies

Install the project dependencies with Poetry:

```bash
poetry install
```

The main dependencies are:

```text
PySpark     3.4.2
Delta Lake  2.4.0
```

You can verify the installed packages with:

```bash
poetry show
```

## 5. Verify PySpark

Check the installed PySpark version:

```bash
poetry run python -c "import pyspark; print(pyspark.__version__)"
```

Expected output:

```text
3.4.2
```

## 9. JupyterLab (Optional)

Jupyter isn't required for PySpark or Delta Lake.

It can be useful for experimenting with Spark interactively, especially while learning.

Install it with:

```bash
poetry add jupyterlab
```

Start it with:

```bash
poetry run jupyter lab
```


## Versions

| Component | Version |
|---|---:|
| Python | 3.11 |
| PySpark | 3.4.2 |
| Delta Lake | 2.4.0 |
| Scala | 2.12 |
| Java | 17 |
| Dependency Manager | Poetry |

## License

Add your project's license here.
