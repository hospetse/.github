# HOSPETSE

Marketplace mobile de serviços para pets. MVP de hospedagem com busca e reserva de hotel para animais de estimação.

**Projeto acadêmico — ESOFT 7º semestre — 2026.1**

---

## Time

| Nome | Papel |
|-------------------------------|---------------------|
| Lucas Neo | Back-end & Banco de Dados |
| Raul Lopes Jorge | Back-end & Infraestrutura |
| Murilo Barbosa | Mobile |
| Brenda Kethleen Cirqueira Lucas | Produto |
| Amanda Lorena | Gestão |
| Arthur Gorini | QA |
| Clara Lazaro | Mobile |

---

## Repositórios

| Repositório | Descrição |
|-------------|-----------|
| [back-end](https://github.com/hospetse/back-end) | API REST — Node.js, Express, PostgreSQL |
| [mobile-front-end](https://github.com/hospetse/mobile-front-end) | Aplicativo mobile — React Native, Expo SDK 54 |
| [artefatos](https://github.com/hospetse/artefatos) | Diagramas, planos de teste e documentação |

---

## Arquitetura

```
Mobile (Expo) → API REST (Express) → PostgreSQL (Railway)
```

- **API em produção**: `back-end-production-11e9.up.railway.app`
- **Documentação Swagger**: `back-end-production-11e9.up.railway.app/api-docs`
- **Gerenciamento**: Jira — `escola-ti.atlassian.net` — projeto HOS

---

## Escopo do MVP

O MVP contempla exclusivamente os fluxos:

- **UC03 — Buscar Hospedagem**: listagem de hotéis, filtros e visualização de perfil
- **UC04 — Solicitar Reserva**: seleção de pet, período e confirmação da reserva

Pagamento, chat, walker, pet sitter, BI e plataforma web ficam para fases futuras.

---

## Artefatos

| Arquivo | Descrição |
|---------|-----------|
| [HOSPETSE.pdf](https://github.com/hospetse/artefatos/blob/main/HOSPETSE.pdf) | Documentação do MVP — UC03 e UC04 |
| [DIAGRAMAS.pdf](https://github.com/hospetse/artefatos/blob/main/DIAGRAMAS.pdf) | Diagramas de sequência |
| [TESTE HOSPETSE.pdf](https://github.com/hospetse/artefatos/blob/main/TESTE%20HOSPETSE.pdf) | Plano de testes UC03 e UC04 |
| [HOSPETSE-JIRA.pdf](https://github.com/hospetse/artefatos/blob/main/HOSPETSE-JIRA.pdf) | Métricas e cards do Jira |
| [DER_HOSPETSE.png](https://github.com/hospetse/artefatos/blob/main/DER_HOSPETSE.png) | Diagrama Entidade-Relacionamento |
| [DIAGRAMA_CLASSE.png](https://github.com/hospetse/artefatos/blob/main/DIAGRAMA_CLASSE.png) | Diagrama de classes |
