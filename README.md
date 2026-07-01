# ⚡ App Quarkus 🇧🇷

![Java](https://img.shields.io/badge/Java-17-009C3B?style=flat&logo=openjdk&logoColor=white)
![Quarkus](https://img.shields.io/badge/Quarkus-3.21-FFDF00?style=flat&logo=quarkus&logoColor=black)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-002776?style=flat&logo=postgresql&logoColor=white)

Aplicacao Quarkus com REST endpoint e CRUD via Panache, gerada por code.quarkus.io.

## Visao geral

Projeto Quarkus 3.21.1 com dois recursos REST: um endpoint `/hello` (greeting) e um CRUD automatico de `MyEntity` via **Panache Entity Resource** (Hibernate ORM REST Data). Banco PostgreSQL via JDBC. Suporte a build nativo (GraalVM) e 4 Dockerfiles inclusos.

## Tecnologias

- **Java 17** / **Quarkus 3.21.1**
- **Hibernate ORM + Panache** (REST Data auto-CRUD)
- **RESTEasy + Jackson** (JSON)
- **PostgreSQL** (JDBC)
- **JUnit 5** + Rest Assured (testes)
- **Maven** (wrapper incluso)
- **Docker** (4 Dockerfiles: JVM, legacy-jar, native, native-micro)

## Como executar

```bash
# Modo dev (hot-reload)
./mvnw quarkus:dev

# Build JAR
./mvnw package
java -jar target/quarkus-app/quarkus-run.jar

# Build nativo
./mvnw package -Dnative
./target/app-quarkus-1.0.0-SNAPSHOT-runner
```

## Licenca

Uso interno/educacional.

---
*Feito com 💚💛💙 — cores da bandeira do Brasil 🇧🇷*
