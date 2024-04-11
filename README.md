## Configuração do Ambiente de Desenvolvimento

Certifique-se de ter as seguintes ferramentas instaladas em seu computador antes de começar:

- **Python 3.8**: A linguagem de programação necessária para executar a aplicação.
- **Docker e Docker Compose**: Ferramentas para criar e gerenciar contêineres, úteis para configurar o ambiente de desenvolvimento.

## 1. Criando e ativando o ambiente virtual

Para isolar as dependências do seu projeto, crie um ambiente virtual e o ative executando os seguintes comandos no terminal:

```
python -m venv .venv
source .venv/bin/activate
```

## 2. Instalando as dependências

Instale as dependências do projeto executando os seguintes comandos:

```
pip install -r requirements.txt
pip install -r requirements-dev.txt
```

## 3. Executando os contêineres Docker

Os contêineres Docker fornecem um ambiente consistente para a aplicação. Para iniciá-los, execute:

```
docker compose up -d
```

## 4. Executando a aplicação

Com as dependências instaladas e os contêineres em execução, agora você pode iniciar a aplicação. Execute o seguinte comando:

```
uvicorn settings.asgi:application
```