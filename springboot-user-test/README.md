# Projeto: Testes Unitários com JUnit e Mockito

## Descrição
Este projeto Spring Boot implementa um controlador de usuários (`UserController`) e testes unitários usando JUnit 5 e Mockito.

## Tecnologias
- Java 11
- Spring Boot (Web, Data JPA, DevTools)
- MariaDB (não necessário para testes unitários)
- JUnit 5
- Mockito

## Estrutura
- `User`: Entidade de usuário.
- `UserRepository`: Interface de persistência.
- `UserService`: Camada de negócio.
- `UserController`: Camada de controle com endpoints REST.
- `UserControllerTest`: Testes unitários simulando o comportamento do serviço.

## Resultados
Os testes foram executados e retornaram sucesso para os cenários de:
- Buscar todos os usuários
- Buscar usuário por ID

---
