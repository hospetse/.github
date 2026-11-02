# HOSPETSE

Plataforma que conecta tutores de pets a quem cuida deles. O Tutor encontra e contrata hospedagem (Host), visitas em casa (Pet Sitter) e passeios (Pet Walker). Pelo aplicativo, ele reserva, paga, acompanha a rotina do pet durante o serviço e tira dúvidas com um assistente de IA antes de falar com o prestador. Na web, a área pública apresenta o produto, e o módulo administrativo valida prestadores, modera conteúdo e acompanha a operação financeira.

**Projeto acadêmico — ESOFT 8º semestre — Turma B — 2026.2**

---

## Sumário

1. [Visão geral](#1-visão-geral)
   * Produto, time e repositórios
   * Azure DevOps: o que temos lá e como organizamos o trabalho
2. Produto e requisitos _(em elaboração)_
   * TAP — Termo de Abertura do Projeto (`TAP_HOSPETSE - V2.pdf`, Wiki #62)
   * Pesquisa sobre cuidados com pets (`Pesquisa sobre cuidados com pets.pdf`)
   * Documento de Requisitos Funcionais e Não Funcionais v2 (`.docx`, Wiki #109)
   * Glossário de Termos de Negócio (Wiki #107)
   * Especificação dos 73 Casos de Uso v2 (`CASOS_DE_USO__HOSPETSE.md`, Wiki #78)
   * User Stories V2 e detalhadas, com critérios de aceite (PDFs, Wiki #81 e #84)
   * Matriz de Rastreabilidade (`Matriz_Rastreabilidade_HOSPETSE_V2.xlsx`, `docs/backlog/04-matriz-rastreabilidade.md`)
3. [UX e UI](#3-ux-e-ui)
   * Protótipo de alta fidelidade das telas (Figma, link externo)
4. Modelagem _(em elaboração)_
   * Diagrama de Casos de Uso completo (`HOSPETSE_Diagrama_Casos_de_Uso.puml` e `.svg`)
   * Diagramas de Casos de Uso por módulo, 16 arquivos (`docs/diagramas-de-casos-de-uso/`)
   * Diagrama de Classes: completo, Auth e 5 seções (`docs/diagrama-de-classes/`)
   * DER V3.1 (Wiki #60, `Banco de Dados DER - Overview.pdf`)
   * 8 Diagramas de Sequência e matriz de tipos (`docs/diagramas-de-sequencia/diagramas-finais/`)
5. Arquitetura (System Design) _(em elaboração)_
   * ADR-001 a ADR-015 (Wiki #55)
   * C4 de Contexto, Containers e Componentes (`docs/diagrama-c4/`)
   * Documento de Ambientes, Deploy e CI/CD (`docs/ambientes.md`)
   * Documentação da API REST: OpenAPI do Auth e do back-end, Swagger em `/docs` e Wiki #88
   * Documento de Integração de Pagamento (`docs/integracao-de-pagamento/`)
6. Qualidade _(em elaboração)_
   * Estratégia de Testes:
     * Hoje: testes unitários e de integração automatizados no back-end e no Auth (`node:test`), rodando no CI.
     * O mobile tem testes com Jest.
     * Próximos passos: testes end-to-end e execução manual dos fluxos principais.
7. Gestão _(em elaboração)_
   * Metodologia, Definition of Done e cerimônias (Wiki #41, #34 e #43)
   * Backlog, épicos e roadmap (`docs/backlog/` e Azure Boards)
   * Estimativas (`docs/estimativas/`, `estimativa-pbi-hospetse.xlsx`)
   * Compromissos da sprint (Wiki #101)
   * Não conformidades ETI 2026 (`NaoConformidades_ETI_2026.xlsx`)
8. Termos e políticas _(em elaboração)_
   * Política de Privacidade (Wiki #94)
   * Termos de Uso do Host, do Pet Sitter e do Pet Walker (Wiki #96, #97 e #103)

---

## 1. Visão geral

### Produto, time e repositórios

#### Time

| Nome | Papel |
|-------------------------------|---------------------|
| Amanda Lorena | Scrum Master |
| Brenda Kethleen Cirqueira Lucas | Product Owner |
| Clara Lazaro | Mobile |
| Lucas Neo | Back-end & Banco de Dados |
| Murilo Barbosa | Mobile |
| Raul Lopes Jorge | Back-end & Infraestrutura |

#### Repositórios

| Repositório | Descrição |
|-------------|-----------|
| [hospetse-mobile](https://github.com/hospetse/hospetse-mobile) | Aplicativo do Tutor e dos prestadores. Expo SDK 58, React Native 0.88, TypeScript e Expo Router. Tem cadastro com PIN, login, busca de Hosts, filtros, resultados e detalhe do Host. Os tokens ficam no armazenamento seguro do aparelho (SecureStore). |
| [hospetse-auth-service](https://github.com/hospetse/hospetse-auth-service) | Serviço de autenticação, separado do back-end e com banco próprio. Confirma o e-mail com PIN, guarda a senha com Argon2id e emite o access token JWT (RS256, 15 minutos) e o refresh token com rotação. Depois do cadastro, cria o usuário no back-end por uma rota interna autenticada. Node.js 22, Express 5, Prisma e PostgreSQL. |
| [hospetse-backend](https://github.com/hospetse/hospetse-backend) | API REST principal, com as regras de negócio. Cuida de usuários, perfil do Tutor, pets, busca e detalhe de Hosts e reservas. Valida o JWT com a chave pública do Auth e nunca recebe senha. Node.js, Express 5, Prisma e PostgreSQL, com contrato OpenAPI em `/docs`. |
| [artefatos](https://github.com/hospetse/artefatos) | Artefatos da primeira etapa do projeto (MVP de 2026.1): documentação, diagramas de sequência, plano de testes, DER e diagrama de classes. |

### Azure DevOps

**[dev.azure.com/escola-ti/Hospetse](https://dev.azure.com/escola-ti/Hospetse)** (link externo, acesso por convite)

O GitHub mostra o código. O planejamento e o acompanhamento do trabalho do time ficam no Azure DevOps, que reúne:

| Área | O que tem lá |
|------|--------------|
| **Boards** | O backlog do produto e o quadro de atividades, com a hierarquia de work items descrita abaixo. |
| **Repos** | Onde o código é desenvolvido, com pull requests e merge para a `develop`. O GitHub recebe um espelho a cada push. |
| **Pipelines** | A integração contínua do back-end e do Auth (`azure-pipelines.yml`) e o espelhamento para o GitHub. |
| **Wiki** | Decisões de arquitetura (ADR-001 a ADR-015), metodologia, Definition of Done, requisitos, casos de uso, termos e políticas. |

#### Como organizamos o trabalho

Usamos o processo Scrum do Azure Boards, em quatro níveis. Cada nível quebra o de cima em partes menores que cabem numa sprint:

```text
Epic  →  Feature  →  PBI (Product Backlog Item) / Bug  →  Task
```

| Nível | Para que serve | Exemplo |
|-------|----------------|---------|
| **Epic** | Um grande objetivo do produto, que atravessa várias sprints. | `HSP-EP-001` — Fundação da plataforma, fluxo principal (mínimo produto viável) |
| **Feature** | Uma capacidade do produto dentro de um épico. | Agrupa os PBIs de uma funcionalidade, como o cadastro ou a busca de Hosts |
| **PBI** | Uma entrega que o usuário percebe, escrita como história de usuário com critérios de aceite. Defeitos entram como **Bug**. | `HSP-PBI-078` — Autenticação do cadastro |
| **Task** | O trabalho técnico para entregar o PBI, atribuído a uma pessoa. | `HSP-PBI-078-TSK-01` — Arquitetura e contratos |

Os épicos de hoje:

| Épico | Tema |
|-------|------|
| `HSP-EP-001` | Fundação da plataforma — fluxo principal (mínimo produto viável) |
| `HSP-EP-001.1` | Fundação da plataforma — fluxo secundário |
| `HSP-EP-002` | Marketplace e contratação |
| `HSP-EP-003` | Execução, comunicação e suporte |
| `HSP-EP-004` | Pagamentos e operações financeiras |
| — | Demandas desejáveis |

**Como o código se liga ao board.** Todo work item tem um número. Branches seguem o padrão `feature/<número>-descrição`, e os commits e PRs citam o item com `AB#<número>` (por exemplo, `AB#516`). Assim, qualquer mudança no código pode ser rastreada até o PBI e o épico de origem.

---

## 3. UX e UI

### Protótipo de alta fidelidade das telas

**[Abrir o protótipo no Figma](https://www.figma.com/design/mw5KHNpIv4u9VFF9AsN8Fe/Hospetse---Design-Telas--Copy-?node-id=0-1&p=f)** (link externo)

O design das telas fica no Figma, não neste repositório nem no Azure DevOps. O link abre uma página externa, e o acesso depende da permissão de compartilhamento do arquivo. Se o link não abrir, peça acesso ao time.
