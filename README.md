# Aplicação Java 21 com Spring Boot 3.3.2

## Visão Geral

Esta é uma aplicação Java 21 desenvolvida com o framework Spring Boot 3.3.2. Seu objetivo principal é fornecer uma API REST simples que retorna o timestamp atual do sistema.

## Estrutura do Projeto

projeto-java
├── app
│   └── src
│       └── main
│           └── java
│               └── com
│                   └── suaempresa
│                       └── suaaplicacao
│                           └── TimestampController.java
├── infra
│   └── terraform
│       ├── main.tf
│       └── variables.tf
└── pom.xml

* **app:** Contém o código fonte da aplicação Java, incluindo os controladores, serviços e entidades.
* **infra:** Contém arquivos de infraestrutura, como os scripts Terraform para provisionamento de recursos na nuvem.
* **pom.xml:** Arquivo de configuração do Maven que define as dependências e plugins do projeto.

## Funcionamento

A aplicação expõe uma única endpoint:

* **GET http://localhost:8080:** 
    Retorna o timestamp atual do sistema no formato ISO-8601.

## Pré-requisitos

* **Java Development Kit (JDK) 21:** Instale o JDK 21 a partir do site oficial do Oracle ou OpenJDK.
* **Maven:** Um gerenciador de dependências para projetos Java.
* **Terraform:** Uma ferramenta de infraestrutura como código para provisionar recursos na nuvem.

## Instalação e Execução

1. **Clone o repositório:**
   ```bash
   git clone https://seu-repositorio.git
   ```

2. **Acesse o projeto:**
    cd projeto-java

3. **Construa o projeto:**
    mvn clean package

4. **Execute a aplicação:**
    java -jar target/deploy-0.0.1-SNAPSHOT.jar