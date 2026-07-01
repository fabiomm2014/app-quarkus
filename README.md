<h1 align="center">⚡ App Quarkus 🇧🇷</h1>

<p align="center">
  <b>Aplicação Quarkus com REST endpoint e CRUD automático via Panache.</b><br>
  Projeto gerado por code.quarkus.io com Hibernate ORM REST Data Panache,
  PostgreSQL e suporte a build nativo (GraalVM).
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Java-17-009C3B?style=for-the-badge&logo=openjdk&logoColor=white" alt="Java 17">
  <img src="https://img.shields.io/badge/Quarkus-3.21-FFDF00?style=for-the-badge&logo=quarkus&logoColor=black" alt="Quarkus">
  <img src="https://img.shields.io/badge/PostgreSQL-002776?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL">
  <img src="https://img.shields.io/badge/Panache-CRUD-009C3B?style=for-the-badge&logoColor=white" alt="Panache">
  <img src="https://img.shields.io/badge/Docker-4%20profiles-FFDF00?style=for-the-badge&logo=docker&logoColor=black" alt="Docker">
  <img src="https://img.shields.io/badge/GraalVM-Native-002776?style=for-the-badge&logo=oracle&logoColor=white" alt="GraalVM">
</p>

<p align="center">
  <img src="https://img.shields.io/badge/-009C3B?style=flat-square&color=009C3B" height="6" width="120" alt="">
  <img src="https://img.shields.io/badge/-FFDF00?style=flat-square&color=FFDF00" height="6" width="120" alt="">
  <img src="https://img.shields.io/badge/-002776?style=flat-square&color=002776" height="6" width="120" alt="">
</p>

---

## 📑 Sumário

- [🔎 Visão geral](#-visão-geral)
- [🛠️ Tecnologias](#️-tecnologias)
- [🚀 Como executar](#-como-executar)
- [📦 Empacotamento](#-empacotamento)
- [🔧 Build nativo](#-build-nativo)
- [📚 Guias relacionados](#-guias-relacionados)
- [📄 Licença](#-licença)

---

## 🔎 Visão geral

Projeto **Quarkus 3.21.1** com dois recursos REST:

| Recurso | Descrição |
| :------ | :-------- |
| 🏷️ `/hello` | Endpoint greeting (GET → texto) |
| 📦 `MyEntity` | CRUD automático via **Panache Entity Resource** (Hibernate ORM REST Data) |

Banco **PostgreSQL** via JDBC. Inclui **4 Dockerfiles** (JVM, legacy-jar, native, native-micro) e perfil Maven para build nativo com **GraalVM**.

---

## 🛠️ Tecnologias

| Camada | Tecnologia |
| :----- | :--------- |
| 💻 **Linguagem** | Java 17 |
| ⚡ **Framework** | Quarkus 3.21.1 |
| 🗄️ **Banco de dados** | PostgreSQL (JDBC) |
| 📦 **ORM** | Hibernate ORM + Panache (auto-CRUD) |
| 🔌 **REST** | RESTEasy + Jackson |
| 🧪 **Testes** | JUnit 5 + Rest Assured |
| 🐳 **Container** | Docker (4 perfis) |
| 🔧 **Build** | Maven (wrapper incluso) |

---

## 🚀 Como executar

<details open>
<summary><b>▶️ Modo dev (hot-reload)</b></summary>

```bash
./mvnw quarkus:dev
```

> **Dev UI** disponível em: http://localhost:8080/q/dev/

</details>

---

## 📦 Empacotamento

<details open>
<summary><b>📦 JAR padrão</b></summary>

```bash
./mvnw package
java -jar target/quarkus-app/quarkus-run.jar
```

</details>

<details>
<summary><b>📦 Über-JAR</b></summary>

```bash
./mvnw package -Dquarkus.package.jar.type=uber-jar
java -jar target/*-runner.jar
```

</details>

---

## 🔧 Build nativo

<details>
<summary><b>🖥️ Com GraalVM instalado</b></summary>

```bash
./mvnw package -Dnative
./target/app-quarkus-1.0.0-SNAPSHOT-runner
```

</details>

<details>
<summary><b>🐳 Sem GraalVM (via container)</b></summary>

```bash
./mvnw package -Dnative -Dquarkus.native.container-build=true
./target/app-quarkus-1.0.0-SNAPSHOT-runner
```

</details>

Mais sobre builds nativos: https://quarkus.io/guides/maven-tooling

---

## 📚 Guias relacionados

| Guia | Descrição |
| :--- | :-------- |
| [REST Data with Panache](https://quarkus.io/guides/rest-data-panache) | Gerar recursos Jakarta REST para entidades Panache |
| [REST Jackson](https://quarkus.io/guides/rest#json-serialisation) | Serialização JSON com Quarkus REST |
| [JDBC PostgreSQL](https://quarkus.io/guides/datasource) | Conexão com PostgreSQL via JDBC |

---

## 📄 Licença

Projeto de uso interno/educacional.

<p align="center">
  <img src="https://img.shields.io/badge/-009C3B?style=flat-square&color=009C3B" height="6" width="120" alt="">
  <img src="https://img.shields.io/badge/-FFDF00?style=flat-square&color=FFDF00" height="6" width="120" alt="">
  <img src="https://img.shields.io/badge/-002776?style=flat-square&color=002776" height="6" width="120" alt="">
</p>

<p align="center"><sub>Feito com 💚💛💙 — cores da bandeira do Brasil 🇧🇷</sub></p>
