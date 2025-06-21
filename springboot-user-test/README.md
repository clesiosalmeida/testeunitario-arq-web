# 🧪 Testes Unitários e Mocking em Spring Boot

## 📋 Descrição
Esta prática tem como objetivo implementar **testes unitários** utilizando **JUnit 5 e Mockito** para validar o comportamento de um controlador de usuários em uma aplicação Spring Boot integrada com MariaDB.

O projeto foca em:
- Garantir a qualidade do código através de testes automatizados
- Utilizar o Mockito para criar mocks e isolar dependências
- Validar o comportamento esperado dos endpoints do UserController

---

## 🚀 Tecnologias Utilizadas
- Java 11 ou superior
- Spring Boot
- Spring Web
- Spring Data JPA
- MariaDB
- JUnit 5
- Mockito
- Spring Boot DevTools

---

## 📦 Configuração do Ambiente

### Dependências
Certifique-se de incluir no `pom.xml`:
```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-web</artifactId>
</dependency>
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-data-jpa</artifactId>
</dependency>
<dependency>
    <groupId>org.mariadb.jdbc</groupId>
    <artifactId>mariadb-java-client</artifactId>
</dependency>
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-test</artifactId>
    <scope>test</scope>
</dependency>
<dependency>
    <groupId>org.mockito</groupId>
    <artifactId>mockito-core</artifactId>
    <scope>test</scope>
</dependency>
````

### Banco de Dados

Configurar o `application.yml` ou `application.properties` com a conexão ao MariaDB.

---

## 🛠️ Como Executar o Projeto

### Subir a aplicação

```bash
./mvnw spring-boot:run
```

### Rodar os testes

```bash
./mvnw test
```

---

## ✅ Estrutura de Testes Implementados

* Testes unitários para o UserController.
* Utilização de Mockito para mockar UserService.
* Simulação de cenários de sucesso e falha.

### Exemplos de Testes:

* Retornar usuário por ID com sucesso.
* Retornar erro ao buscar usuário inexistente.
* Criar usuário com sucesso.
* Retornar erro ao criar usuário inválido.

---

## 📖 Relatório de Resultados

| Teste                            | Resultado |
| -------------------------------- | --------- |
| Buscar usuário por ID (válido)   | ✅ Passou  |
| Buscar usuário por ID (inválido) | ✅ Passou  |
| Criar novo usuário               | ✅ Passou  |
| Criar usuário inválido           | ✅ Passou  |

Todos os testes foram executados com sucesso. Foi utilizado Mockito para simular o comportamento do serviço e garantir que o controlador fosse testado isoladamente.

---

## 📝 Notas Adicionais

* O projeto está preparado para ser integrado com outros módulos.
* O MariaDB pode ser substituído por H2 para facilitar os testes unitários sem necessidade de subir banco real.
* Para futuras melhorias, podem ser adicionados testes de integração e testes de carga.

---

