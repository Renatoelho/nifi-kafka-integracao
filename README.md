# Nifi + Kafka: Integrando de Forma Simples

Vou mostrar como realizar a integração entre o ***Apache Nifi*** e o ***Apache Kafka*** de maneira simples e eficiente. Ao combinar essas duas poderosas ferramentas, é possível otimizar o fluxo de dados entre sistemas de forma escalável e sem complicações.

As ferramentas utilizadas neste projeto são o Apache Nifi e o Apache Kafka. O Nifi oferece uma interface gráfica intuitiva para criação e ***gerenciamento de fluxos de dados*** em tempo real, enquanto o Kafka é uma plataforma distribuída para ***armazenamento e transmissão*** de mensagens. Essas ferramentas são ideais para simplificar a arquitetura de processamento de dados e melhorar a comunicação entre sistemas.


# Apresentação em vídeo

<p align="center">
  <a href="https://youtu.be/xxxxxxxxxx" target="_blank"><img src="deploy/thumbnail/Nifi_Kafka_Youtube.png" alt="Vídeo de apresentação"></a>
</p>


### Requisitos

+ ![Docker](https://img.shields.io/badge/Docker-23.0.3-E3E3E3)

+ ![Docker-compose](https://img.shields.io/badge/Docker--compose-1.25.0-E3E3E3)

+ ![Git](https://img.shields.io/badge/Git-2.25.1%2B-E3E3E3)

+ ![Ubuntu](https://img.shields.io/badge/Ubuntu-20.04-E3E3E3)


### Ativando o serviço

```bash
docker compose -p nifi_kafka -f docker-compose.yaml up -d
```


### Acesso às ferramentas

+ Apache Nifi

|Tipo|Valor|
|------------------|--------------|
|Usuário|nifi|
|Senha|mkYUQBJ9BBhc38RWa1p3E76xUR1rhYGR|
|URL|[https://localhost:8443/nifi/](https://localhost:8443/nifi/)|

+ Apache Kafka

|Tipo|Valor|
|------------------|--------------| 
|Broker interno/porta|kafka:9002    |
|Broker externo/porta|localhost:9004|

+ Control Center

|Tipo|Valor|
|------------------|--------------| 
|URL|[http://localhost:19021](http://localhost:19021)|


### Desativando os serviços

```bash
docker compose -p nifi_kafka -f docker-compose.yaml down
```


# Referências

NiFi System Administrator’s Guide, ***Apache NiFi***. Disponível em: <https://nifi.apache.org/docs/nifi-docs/html/administration-guide.html>. Acesso em: 28 mar. 2024.

Expression Language Guide, ***Apache NiFi Expression Language Guide***. Disponível em: <https://nifi.apache.org/docs/nifi-docs/>. Acesso em: 28 mar. 2024.

Install Docker Desktop on Ubuntu, ***docs.docker.com***. Disponível em: <https://docs.docker.com/desktop/install/ubuntu/>. Acesso em: 28 mar. 2024.

The Compose file, ***docs.docker.com***. Disponível em: <https://docs.docker.com/compose/compose-file/03-compose-file/>. Acesso em: 28 mar. 2024.

bitnami/kafka, ***Docker Hub***. Disponível em: <https://hub.docker.com/r/bitnami/kafka>. Acesso em: 28 mar. 2024.

INTRODUCTION, ***Apache Kafka***. Disponível em: <https://kafka.apache.org/intro>. Acesso em: 28 mar. 2024.

bitnami/zookeeper, ***Docker Hub***. Disponível em: <https://hub.docker.com/r/bitnami/zookeeper>. Acesso em: 28 mar. 2024.

Welcome to Apache ZooKeeper, ***Apache Zookeeper***. Disponível em: <https://zookeeper.apache.org/>. Acesso em: 28 mar. 2024.

Control Center, ***Docker Hub***. Disponível em: <https://hub.docker.com/r/confluentinc/cp-enterprise-control-center>. Acesso em: 28 mar. 2024.

A Complete Comparison of Apache Kafka vs Confluent, ***Confluent***. Disponível em: <https://www.confluent.io/apache-kafka-vs-confluent/>. Acesso em: 28 mar. 2024.
