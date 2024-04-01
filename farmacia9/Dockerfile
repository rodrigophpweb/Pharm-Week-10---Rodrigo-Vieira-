# Dockerfile para Aplicação Java
#
# Este Dockerfile é usado para construir uma imagem Docker para uma aplicação Java.
#
# Instruções Dockerfile:
#
# FROM: especifica a imagem base a ser usada para construir esta imagem.
# WORKDIR: define o diretório de trabalho dentro do contêiner onde os comandos subsequentes serão executados.
# COPY: copia arquivos ou diretórios do contexto de construção para o sistema de arquivos do contêiner.
# ARG: define uma variável que pode ser passada durante o build da imagem Docker.
# ENV: define uma variável de ambiente dentro do contêiner.
# EXPOSE: especifica as portas em que o contêiner está escutando.
# CMD: especifica o comando padrão a ser executado quando o contêiner for iniciado.
#
# Como usar este Dockerfile:
#
# 1. Certifique-se de ter o Docker instalado em sua máquina.
# 2. Coloque o arquivo api-0.0.1-SNAPSHOT.jar no mesmo diretório deste Dockerfile.
# 3. Abra um terminal e navegue até o diretório contendo este Dockerfile e o arquivo JAR.
# 4. Execute o seguinte comando para construir a imagem Docker:
#      docker build -t nome-da-imagem:tag .
#
#    Substitua 'nome-da-imagem:tag' pelo nome e tag desejados para a sua imagem Docker.
#
# Depois de construir a imagem, você pode executar contêineres a partir dela para implantar sua aplicação Java.

FROM openjdk:17-jdk
WORKDIR /app-jdk
COPY target/api-0.0.1-SNAPSHOT.jar .
ARG PORT_BUILD=8080
ENV PORT=$PORT_BUILD
EXPOSE $PORT_BUILD
CMD java -jar api-0.0.1-SNAPSHOT.jar
