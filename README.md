# kurt-demo-app

API REST de cadastro de usuários — projeto de demo para o Kurt.

Usado na demo de dezembro/2026 para demonstrar o fluxo:
ticket Jira → Kurt pergunta no Slack → implementa → PR.

## Stack

- Java 21
- Spring Boot 3.3
- H2 (em memória)
- Maven

## Como rodar

```bash
mvn spring-boot:run
```

API disponível em `http://localhost:8080`.

## Endpoints existentes

| Método | Path | Descrição |
|--------|------|-----------|
| GET | /api/users | Lista todos os usuários |
| GET | /api/users/{id} | Busca usuário por ID |
| POST | /api/users | Cria novo usuário |

## Tickets de demo (projeto KS no Jira)

- **KS-11** — Adicionar campo `departamento` na entidade UserProfile
- **KS-12** — Endpoint de busca por departamento
- **KS-13** — Validar unicidade de email ao criar usuário
