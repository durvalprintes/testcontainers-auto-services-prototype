# Projeto para automatizar ambientes com Testcontainers

## Sobre

Projeto Springboot para criar automaticamente um ambiente de desenvolvimento, com os serviços necessários em containeres utilizando Testcontainers. 

## Começando

Siga as próximas instruções para instalar e importar no seus projetos Maven.

### Pré-requisitos

Maven instalado.

### Instalação

Execute o seguinte comando para instalar no seu diretório local Maven:

```
mvn clean install -DskipTests
```

## Uso

Para utilizar nos demais projetos, adicione no ```pom.xml```:
```
<dependency>
  <groupId>org.springframework.boot</groupId>
  <artifactId>spring-boot-devtools</artifactId>
  <scope>runtime</scope>
  <optional>true</optional>
</dependency>

<dependency>
  <groupId>org.testcontainers</groupId>
  <artifactId>testcontainers</artifactId>
  <version>${testcontainers.version}</version>
</dependency>

<dependency>
  <groupId>org.testcontainers</groupId>
  <artifactId>postgresql</artifactId>
  <version>${testcontainers.version}</version>
</dependency>

<dependency>
  <groupId>org.springframework.boot</groupId>
  <artifactId>spring-boot-devtools-autoservices</artifactId>
  <version>0.0.1-SNAPSHOT</version>
</dependency>
```