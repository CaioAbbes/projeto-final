# Projeto final

## Projeto realizado com base nos dados da Covid - 19 no Brasil.

### Instruções para executar o projeto
\
Os containers do Spark e Elastic devem estar rodando.

~~~
docker-compose -f docker-compose-parcial.yml up -d
docker-compose up -d
~~~

Deve-se entrar no jupyter com a seguinte URL: http://localhost:8889

Para os exercicios que requerem o uso do HDFS, deve-se entrar no cointainer **namenode**
~~~
docker exec -it namenode bash
~~~

Para os exercicios que requerem o uso do Hive, deve-se entrar no cointainer **hive-server** e entrar no **beeline**
~~~
docker exec -it hive-server bash
beeline -u jdbc:hive2://localhost:10000 root
~~~

Para os exercicios que requerem o uso do Kafka, deve-se entrar no cointainer **kafka**
~~~
docker exec -it kafka bash
~~~