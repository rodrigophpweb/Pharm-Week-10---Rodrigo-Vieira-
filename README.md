# Documentação da Aplicação Farmácia

Este repositório contém os arquivos necessários para construir e executar a aplicação Farmácia, composta por um serviço MySQL e um serviço de API REST em Java.

## Pré-requisitos

Certifique-se de ter o Docker e o Docker Compose instalados em sua máquina antes de continuar.

- Docker: [Instalação do Docker](https://docs.docker.com/get-docker/)
- Docker Compose: [Instalação do Docker Compose](https://docs.docker.com/compose/install/)

## Construindo e executando a aplicação

Para construir e executar a aplicação, siga estas etapas:

1. Clone este repositório:

    ```
    git clone git@github.com:rodrigophpweb/Pharm-Week-10---Rodrigo-Vieira-.git
    ```

2. Navegue até o diretório clonado:

    ```
    cd Pharm-Week-10---Rodrigo-Vieira-
    ```

3. Execute o Docker Compose para construir e iniciar os contêineres:

    ```
    docker-compose up --build
    ```

Isso iniciará os serviços MySQL e a API da Farmácia.

## Detalhes da Configuração

### Dockerfile

O arquivo Dockerfile define a imagem para a API da Farmácia. Ele baseia-se na imagem openjdk:17-jdk, copia o arquivo JAR da aplicação para o contêiner e define a porta na qual a aplicação será executada.

### docker-compose.yml

O arquivo docker-compose.yml define os serviços necessários para executar a aplicação. Ele configura um serviço MySQL e um serviço para a API da Farmácia. Também define variáveis de ambiente e mapeia as portas necessárias para acessar os serviços.

## Acesso à Aplicação

- A API da Farmácia estará disponível em [http://localhost:8081](http://localhost:8081).
- O MySQL estará disponível em [mysql://localhost:3307](mysql://localhost:3307).

## Variáveis de Ambiente

- `MYSQL_ROOT_PASSWORD`: Senha para o usuário root do MySQL.
- `MYSQL_DATABASE`: Nome do banco de dados MySQL.
- `MYSQL_HOST`: Hostname do serviço MySQL.

## Contribuindo

Se você deseja contribuir para este projeto, por favor, abra uma issue ou envie uma pull request.

