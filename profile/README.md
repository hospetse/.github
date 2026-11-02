# HOSPETSE

Plataforma que conecta tutores de pets a quem cuida deles. O Tutor encontra e contrata hospedagem (Host), visitas em casa (Pet Sitter) e passeios (Pet Walker). Pelo aplicativo, ele reserva, paga, acompanha a rotina do pet durante o serviço e tira dúvidas com um assistente de IA antes de falar com o prestador. Na web, a área pública apresenta o produto, e o módulo administrativo valida prestadores, modera conteúdo e acompanha a operação financeira.

**Projeto acadêmico — ESOFT 8º semestre — Turma B — 2026.2**

---

## Sumário

Os documentos ficam no repositório [artefatos](https://github.com/hospetse/artefatos), separados por etapa: [1º semestre](https://github.com/hospetse/artefatos/tree/main/1o-semestre) (MVP de 2026.1) e [2º semestre](https://github.com/hospetse/artefatos/tree/main/2o-semestre) (documentação atual). Cada item abaixo abre o arquivo no GitHub. O link **Wiki #n** abre a mesma página na Wiki do Azure DevOps, que é privada e só abre para quem tem acesso ao projeto.

1. [Visão geral](#1-visão-geral)
   * [Produto, time e repositórios](#produto-time-e-repositórios)
   * [Azure DevOps: o que temos lá e como organizamos o trabalho](#azure-devops)
2. [Produto e requisitos](https://github.com/hospetse/artefatos/tree/main/2o-semestre/02-produto-e-requisitos)
   * [TAP — Termo de Abertura do Projeto](https://github.com/hospetse/artefatos/blob/main/2o-semestre/02-produto-e-requisitos/tap-termo-de-abertura.md) ([PDF](https://github.com/hospetse/artefatos/blob/main/2o-semestre/02-produto-e-requisitos/tap-termo-de-abertura-v2.pdf), [Wiki #62](https://dev.azure.com/escola-ti/Hospetse/_wiki/wikis/Hospetse.wiki/62))
   * [Pesquisa sobre cuidados com pets](https://github.com/hospetse/artefatos/blob/main/2o-semestre/02-produto-e-requisitos/pesquisa-sobre-cuidados-com-pets.pdf)
   * [Documento de Requisitos Funcionais e Não Funcionais v2](https://github.com/hospetse/artefatos/blob/main/2o-semestre/02-produto-e-requisitos/requisitos-funcionais-e-nao-funcionais-v2.md) ([DOCX](https://github.com/hospetse/artefatos/blob/main/2o-semestre/02-produto-e-requisitos/requisitos-funcionais-e-nao-funcionais-v2.docx), [Wiki #109](https://dev.azure.com/escola-ti/Hospetse/_wiki/wikis/Hospetse.wiki/109))
   * [Glossário de Termos de Negócio v2](https://github.com/hospetse/artefatos/blob/main/2o-semestre/02-produto-e-requisitos/glossario-v2.md) ([Wiki #107](https://dev.azure.com/escola-ti/Hospetse/_wiki/wikis/Hospetse.wiki/107))
   * [Especificação dos 73 Casos de Uso v2](https://github.com/hospetse/artefatos/blob/main/2o-semestre/02-produto-e-requisitos/casos-de-uso-v2.md) ([PDF](https://github.com/hospetse/artefatos/blob/main/2o-semestre/02-produto-e-requisitos/casos-de-uso-v2.pdf), [Wiki #78](https://dev.azure.com/escola-ti/Hospetse/_wiki/wikis/Hospetse.wiki/78))
   * [User Stories v2](https://github.com/hospetse/artefatos/blob/main/2o-semestre/02-produto-e-requisitos/user-stories-v2.md) e [detalhadas, com critérios de aceite](https://github.com/hospetse/artefatos/blob/main/2o-semestre/02-produto-e-requisitos/user-stories-detalhadas-v2.md) ([PDF](https://github.com/hospetse/artefatos/blob/main/2o-semestre/02-produto-e-requisitos/user-stories-v2.pdf) e [PDF detalhado](https://github.com/hospetse/artefatos/blob/main/2o-semestre/02-produto-e-requisitos/user-stories-detalhadas-v2.pdf), [Wiki #81](https://dev.azure.com/escola-ti/Hospetse/_wiki/wikis/Hospetse.wiki/81) e [#84](https://dev.azure.com/escola-ti/Hospetse/_wiki/wikis/Hospetse.wiki/84))
   * [Matriz de Rastreabilidade](https://github.com/hospetse/artefatos/blob/main/2o-semestre/02-produto-e-requisitos/matriz-de-rastreabilidade.md) ([XLSX](https://github.com/hospetse/artefatos/blob/main/2o-semestre/02-produto-e-requisitos/matriz-de-rastreabilidade-v2.xlsx), [Wiki #124](https://dev.azure.com/escola-ti/Hospetse/_wiki/wikis/Hospetse.wiki/124))
3. [UX e UI](https://github.com/hospetse/artefatos/tree/main/2o-semestre/03-ux-e-ui)
   * [Protótipo de alta fidelidade das telas (Figma)](https://www.figma.com/design/mw5KHNpIv4u9VFF9AsN8Fe/Hospetse---Design-Telas--Copy-?node-id=0-1&p=f)
   * [Fluxo de telas visual v2](https://github.com/hospetse/artefatos/blob/main/2o-semestre/03-ux-e-ui/fluxo-de-telas-v2.md) ([Wiki #74](https://dev.azure.com/escola-ti/Hospetse/_wiki/wikis/Hospetse.wiki/74))
   * Planilhas de fluxo do [Tutor](https://github.com/hospetse/artefatos/blob/main/2o-semestre/03-ux-e-ui/planilha-fluxo-tutor-v2.xlsx) e do [Web Administrativo](https://github.com/hospetse/artefatos/blob/main/2o-semestre/03-ux-e-ui/planilha-fluxo-web-administrativo.xlsx) (XLSX)
   * [Modelo de identidade visual (Canva)](https://canva.link/t30yyziy9ubzzo3) ([Wiki #76](https://dev.azure.com/escola-ti/Hospetse/_wiki/wikis/Hospetse.wiki/76))
4. [Modelagem](https://github.com/hospetse/artefatos/tree/main/2o-semestre/04-modelagem)
   * [Diagramas de Casos de Uso](https://github.com/hospetse/artefatos/tree/main/2o-semestre/04-modelagem/casos-de-uso): visão completa e 16 por módulo
   * [Diagrama de Classes](https://github.com/hospetse/artefatos/tree/main/2o-semestre/04-modelagem/classes): completo, Auth Server e 5 seções
   * [DER V3.1](https://github.com/hospetse/artefatos/blob/main/2o-semestre/04-modelagem/der/der-v3.1.md) ([Wiki #60](https://dev.azure.com/escola-ti/Hospetse/_wiki/wikis/Hospetse.wiki/60))
   * [8 Diagramas de Sequência e matriz de tipos](https://github.com/hospetse/artefatos/tree/main/2o-semestre/04-modelagem/sequencia) ([Wiki #105](https://dev.azure.com/escola-ti/Hospetse/_wiki/wikis/Hospetse.wiki/105))
5. [Arquitetura (System Design)](https://github.com/hospetse/artefatos/tree/main/2o-semestre/05-arquitetura)
   * [ADR-001 a ADR-015](https://github.com/hospetse/artefatos/blob/main/2o-semestre/05-arquitetura/adrs.md) ([Wiki #55](https://dev.azure.com/escola-ti/Hospetse/_wiki/wikis/Hospetse.wiki/55))
   * [C4 de Contexto, Containers e Componentes](https://github.com/hospetse/artefatos/tree/main/2o-semestre/05-arquitetura/c4)
   * [Ambientes, Deploy e CI/CD](https://github.com/hospetse/artefatos/blob/main/2o-semestre/05-arquitetura/ambientes-e-deploy.md)
   * [Documentação da API REST](https://github.com/hospetse/artefatos/tree/main/2o-semestre/05-arquitetura/api): contratos OpenAPI do Auth Server e do back-end
   * Swagger da API publicada (Auth Server e back-end): [Wiki #88](https://dev.azure.com/escola-ti/Hospetse/_wiki/wikis/Hospetse.wiki/88), acesso restrito ao projeto
   * [Integração de Pagamento](https://github.com/hospetse/artefatos/tree/main/2o-semestre/05-arquitetura/integracao-de-pagamento)
6. [Qualidade](https://github.com/hospetse/artefatos/tree/main/2o-semestre/06-qualidade)
   * [Estratégia de Testes](https://github.com/hospetse/artefatos/tree/main/2o-semestre/06-qualidade): testes automatizados no back-end e no Auth Server rodando no CI, depois testes end-to-end e validação manual dos fluxos
7. [Gestão](https://github.com/hospetse/artefatos/tree/main/2o-semestre/07-gestao)
   * [Fluxo de trabalho e cerimônias](https://github.com/hospetse/artefatos/blob/main/2o-semestre/07-gestao/fluxo-de-trabalho-e-cerimonias.md) ([Wiki #43](https://dev.azure.com/escola-ti/Hospetse/_wiki/wikis/Hospetse.wiki/43))
   * [Definition of Done e critérios de aceite](https://github.com/hospetse/artefatos/blob/main/2o-semestre/07-gestao/definition-of-done.md) ([Wiki #34](https://dev.azure.com/escola-ti/Hospetse/_wiki/wikis/Hospetse.wiki/34))
   * [Epic HSP-EP-001 — Identidade, conta e acesso](https://github.com/hospetse/artefatos/blob/main/2o-semestre/07-gestao/epic-hsp-ep-001.md) ([Wiki #69](https://dev.azure.com/escola-ti/Hospetse/_wiki/wikis/Hospetse.wiki/69))
   * [Compromissos da Sprint 7](https://github.com/hospetse/artefatos/blob/main/2o-semestre/07-gestao/compromissos-sprint-7.md) ([Wiki #86](https://dev.azure.com/escola-ti/Hospetse/_wiki/wikis/Hospetse.wiki/86))
   * [Estimativa inicial em horas por PBI](https://github.com/hospetse/artefatos/blob/main/2o-semestre/07-gestao/estimativa-horas-pbis.md) ([XLSX](https://github.com/hospetse/artefatos/blob/main/2o-semestre/07-gestao/estimativa-pbi-hospetse.xlsx), [Wiki #80](https://dev.azure.com/escola-ti/Hospetse/_wiki/wikis/Hospetse.wiki/80))
   * [Visão macro do backlog: Epics, Features e PBIs](https://github.com/hospetse/artefatos/blob/main/2o-semestre/07-gestao/visao-macro.xlsx) (XLSX)
   * Backlog completo e sprints no [Azure Boards](https://dev.azure.com/escola-ti/Hospetse/_boards)
8. [Termos e políticas](https://github.com/hospetse/artefatos/tree/main/2o-semestre/08-termos-e-politicas)
   * [Política de Privacidade](https://github.com/hospetse/artefatos/blob/main/2o-semestre/08-termos-e-politicas/politica-de-privacidade.md) ([Wiki #94](https://dev.azure.com/escola-ti/Hospetse/_wiki/wikis/Hospetse.wiki/94))
   * Termos de Uso do [Host](https://github.com/hospetse/artefatos/blob/main/2o-semestre/08-termos-e-politicas/termos-de-uso-host.md), do [Pet Sitter](https://github.com/hospetse/artefatos/blob/main/2o-semestre/08-termos-e-politicas/termos-de-uso-pet-sitter.md) e do [Pet Walker](https://github.com/hospetse/artefatos/blob/main/2o-semestre/08-termos-e-politicas/termos-de-uso-pet-walker.md) ([Wiki #96](https://dev.azure.com/escola-ti/Hospetse/_wiki/wikis/Hospetse.wiki/96), [#97](https://dev.azure.com/escola-ti/Hospetse/_wiki/wikis/Hospetse.wiki/97) e [#103](https://dev.azure.com/escola-ti/Hospetse/_wiki/wikis/Hospetse.wiki/103))

Documentos extras, em PDF, Word e Excel, estão na [pasta do projeto no Google Drive](https://drive.google.com/drive/folders/1nrYGjsp7fLBej4jro9sgQZ-MuqHesd78?usp=sharing).

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
| [artefatos](https://github.com/hospetse/artefatos) | Documentos e diagramas do projeto, separados por etapa: `1o-semestre/` (MVP de 2026.1) e `2o-semestre/` (documentação atual, organizada pelas seções do sumário). |

### Azure DevOps

**[dev.azure.com/escola-ti/Hospetse](https://dev.azure.com/escola-ti/Hospetse)** (link externo, acesso por convite)

O GitHub mostra o código. O planejamento e o acompanhamento do trabalho do time ficam no Azure DevOps, que reúne:

| Área | O que tem lá |
|------|--------------|
| **Boards** | O backlog do produto e o quadro de atividades, com a hierarquia de work items descrita abaixo. |
| **Repos** | Onde o código é desenvolvido, com pull requests e merge para a `develop`. O GitHub recebe um espelho a cada push. |
| **Pipelines** | A integração contínua do back-end e do Auth (`azure-pipelines.yml`) e o espelhamento para o GitHub. |
| **Wiki** | Decisões de arquitetura (ADR-001 a ADR-015), metodologia, Definition of Done, requisitos, casos de uso, termos e políticas. Fica só no Azure; o sumário acima aponta para cada página. |

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

