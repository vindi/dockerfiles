FROM mariadb
MAINTAINER Vindi<comunidade@vindi.com.br>

ENV MYSQL_USER root
ENV MYSQL_DATABASE opencart_db
ENV MYSQL_ROOT_PASSWORD 123

# Install dependencies
RUN apt-get update && apt-get install -y wget

# Copy database
RUN cd /docker-entrypoint-initdb.d/ && wget https://raw.githubusercontent.com/vindi/dockerfiles/master/opencart3/mysql/opencart.sql
