<h1 align="center">
    Spring Security JWT
</h1>

Tutorial para ilustrar como implementar uma autenticação com Spring Security e JWT.

## Tecnologias

- [Spring Boot](https://spring.io/projects/spring-boot)
- [Spring MVC](https://docs.spring.io/spring-framework/reference/web/webmvc.html)
- [Spring Security](https://spring.io/projects/spring-security)
- [Spring Data JDBC](https://spring.io/projects/spring-data-jdbc)
- [H2](https://www.h2database.com)

## Como Executar
- Clonar repositório git:
```
git@github.com:rdgoliveiraa/jwt.git
```

- Construir o projeto:
```
./mvnw clean package
```

- Executar:
```
java -jar ./target/jwt-0.0.1-SNAPSHOT.jar
```

- Testar ( com [httppie](https://httpie.io))
```
http -a username:password POST :8080/authenticate
JWT = <token>
http :8080/private -A bearer -a ${JWT}
```