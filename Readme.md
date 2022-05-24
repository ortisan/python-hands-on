# Python + AWS Lambda Hands On

## Python

- Criada em 1991(primeira release), por Guido Van Rossum.
- "Bala de prata" (quase).
- Muito utilizado em:
  - Automatizações - [Selenium](https://selenium-python.readthedocs.io/), [Beautiful Soap](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)
  - Bigdata - [PySpark](http://spark.apache.org/docs/latest/api/python/)
  - Data Science - [Jupyter](https://jupyter.readthedocs.io/en/latest/), Libs estatisticas e analise exploratória
  - Machine Learning / Deep Learning - [NLTK](https://www.nltk.org/), [Scikit-Learn](https://scikit-learn.org/stable/), [Tensor Flow](https://www.tensorflow.org/?hl=pt-br), [Keras](https://keras.io/)
  - Web - [Django](https://www.djangoproject.com/)
  - Hack (Mr. Robot)
    - Vídeos [David Bombal](https://www.youtube.com/channel/UCP7WmQ_U4GB3K51Od9QvM0w)

### Exemplos de script

1. **python/exemplos/1-hello-world.py**
2. **python/exemplos/2-teste-unitario.py**
3. **python/exemplos/3-teste-unitario-pytest.py**

### Preparação do Ambiente

Configuração Proxy:

1. Criar o arquivo **pip.ini** no diretório **USER_HOME/pip/**:

```sh
[global]
trusted-host = pypi.python.org
                pypi.org
                files.pythonhosted.org
http_proxy = <url http proxy>
https_proxy = <url https proxy>
```

Criação do ambiente:

```sh
# Versão >= Python 3.3
python3 -m venv ./venv -p=<CAMINHO_PYTHON_HOME>/python
# Versão < Python 3.3
pip install virtualenv
virtualenv -p=<CAMINHO_PYTHON_HOME>/python ./venv
```

Ativação do ambiente:

```sh
# Linux/Gitbash
source ./venv/bin/activate
# Windows
venv/Script/activate.bat
```

### PIP

- É o gerenciador de pacotes do Python.
- Gradle/Maven/NPM do Python

#### Instalação das dependências

```sh
pip install <NOME DO PACOTE>

# OU

pip install -r requirements.txt
```

### Notebooks

```sh
jupyter notebook notebooks
```

1. [Python Básico](https://github.com/ortisan/python-aws-lambda-hands-on/blob/main/python/notebooks/1-PythonBasico.ipynb)
1. [Bot Bitcoin](https://github.com/ortisan/python-aws-lambda-hands-on/blob/main/python/notebooks/2-BotBitcoinNow.ipynb)
1. [Analise Dados Bitcoin](https://github.com/ortisan/python-aws-lambda-hands-on/blob/main/python/notebooks/3-AnalyticsBitcoinPrice.ipynb)

### Aplicação Web

Na pasta **troubleshooting-webapp**, existe um projeto Web utilizando fastapi com todo ecosistema de monitoração e telemetria.
