API Sistema Hospitalar

API REST desenvolvida para simular o gerenciamento de um sistema hospitalar fictício, aplicando conceitos de desenvolvimento de APIs, operações CRUD e organização de projetos com Spring Boot.

O projeto utiliza **Spring Boot 3**, **MySQL** e **Flyway** para gerenciamento e versionamento do banco de dados, além do **SpringDoc OpenAPI** para documentação da API.

## Tecnologias utilizadas

* **Java**
* **Spring Boot 3**
* **Spring Data JPA**
* **MySQL**
* **Flyway** — versionamento e gerenciamento das migrações do banco de dados
* **SpringDoc OpenAPI** — documentação da API
* **Maven**

## Funcionalidades

* Operações CRUD para gerenciamento dos recursos do sistema
* Integração com banco de dados MySQL
* Persistência de dados utilizando Spring Data JPA
* Versionamento do banco de dados com Flyway
* Documentação dos endpoints utilizando SpringDoc/OpenAPI
* Estrutura organizada seguindo boas práticas de desenvolvimento com Spring Boot

## Banco de dados

O projeto utiliza **MySQL** como banco de dados relacional.

As alterações na estrutura do banco são controladas pelo **Flyway**, permitindo manter um histórico das migrações e garantir maior controle sobre a evolução do banco de dados.

As migrações ficam organizadas no diretório:

```text
src/main/resources/db/migration
```

## Documentação da API

A documentação dos endpoints é disponibilizada através do **SpringDoc OpenAPI**, permitindo visualizar e testar as operações da API de forma mais prática.

Após executar a aplicação, a documentação pode ser acessada através da interface do Swagger UI disponibilizada pelo projeto.

## Como executar o projeto

### Pré-requisitos

Antes de executar o projeto, certifique-se de possuir instalado:

* Java
* Maven
* MySQL

### 1. Clone o repositório

```bash
git clone <https://github.com/RafaelNagel/api-spring.git>
```

### 2. Configure o banco de dados

Crie um banco de dados MySQL para a aplicação e configure as credenciais no arquivo:

```text
src/main/resources/application.properties
```

Exemplo:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/nome_do_banco
spring.datasource.username=seu_usuario
spring.datasource.password=sua_senha
```

> Não versione credenciais reais no repositório. Para projetos públicos, prefira variáveis de ambiente ou um arquivo de configuração local.

### 3. Execute a aplicação

Utilizando Maven:

```bash
./mvnw spring-boot:run
```

No Windows, também pode ser utilizado:

```bash
mvnw.cmd spring-boot:run
```

As migrações do Flyway serão executadas conforme a configuração da aplicação.

## Objetivo do projeto

Este projeto foi desenvolvido com o objetivo de praticar e consolidar conhecimentos em **desenvolvimento de APIs REST com Java e Spring Boot**, trabalhando conceitos como:

* Arquitetura de aplicações Spring
* Operações CRUD
* Persistência de dados
* Integração com banco de dados relacional
* Versionamento de banco de dados
* Documentação de APIs
* Organização e boas práticas de código

## Próximos passos

Algumas possíveis evoluções para o projeto incluem:

* Implementação de autenticação e autorização
* Adição de testes automatizados
* Implementação de paginação e filtros
* Melhorias no tratamento de exceções
* Containerização da aplicação com Docker
* Expansão dos recursos do sistema hospitalar

## Autor

**Rafael Nagel de Souza**

Estudante de Ciência da Computação e desenvolvedor de software em formação, com foco em desenvolvimento backend utilizando **Java e Spring Boot**.
**
