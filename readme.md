## Repositório Pré-configurado para Django com Docker e Docker Compose

Este repositório foi configurado para facilitar o desenvolvimento de aplicações Django utilizando Docker e Docker Compose. Se você possui conhecimentos em Django, Docker e Docker Compose, poderá facilmente utilizar e adaptar este repositório conforme as suas necessidades.

## Pré-requisitos

- Python
- [Docker](https://docs.docker.com/get-docker/)
- [Docker Compose](https://docs.docker.com/compose/install/)

### Estrutura do Projeto

- .docker: Diretório de configuração das imagens docker.
- .github: Diretório de configuração de pipelines com github actions
- docker-compose.yml: Arquivo de configuração do Docker Compose.
- requirements.txt: Arquivo que contém as dependências do projeto.
- requirements-dev.txt: Arquivo que contém as dependências de desenvolvimento.

### Personalização

- Dockerfile: Modifique o Dockerfile para incluir dependências adicionais
- docker-compose.yml: Adicione serviços ou variáveis de ambiente conforme necessário.

### Comandos úteis

Iniciando todos os containers
```bash
docker compose up -d
``` 

Iniciando apenas um container. </br>
Use o nome do serviço no docker compose para iniciar apenas o container que precisar.
```bash
docker compose up -d mysql
```

### Contribuição

Sinta-se à vontade para contribuir com este projeto. Para isso, faça um fork do repositório, crie um branch para suas alterações e abra um pull request.