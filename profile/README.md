# HOSPETSE

Plataforma que conecta tutores de pets a quem cuida deles. O Tutor encontra e contrata hospedagem (Host), visitas em casa (Pet Sitter) e passeios (Pet Walker). Pelo aplicativo, ele reserva, paga, acompanha a rotina do pet durante o serviço e tira dúvidas com um assistente de IA antes de falar com o prestador. Na web, a área pública apresenta o produto, e o módulo administrativo valida prestadores, modera conteúdo e acompanha a operação financeira.

**Projeto acadêmico — ESOFT 8º semestre — Turma B — 2026.2**

---

## Time

| Nome | Papel |
|-------------------------------|---------------------|
| Amanda Lorena | Scrum Master |
| Brenda Kethleen Cirqueira Lucas | Product Owner |
| Clara Lazaro | Mobile |
| Lucas Neo | Back-end & Banco de Dados |
| Murilo Barbosa | Mobile |
| Raul Lopes Jorge | Back-end & Infraestrutura |

---

## Repositórios

| Repositório | Descrição |
|-------------|-----------|
| [hospetse-mobile](https://github.com/hospetse/hospetse-mobile) | Aplicativo do Tutor e dos prestadores. Expo SDK 58, React Native 0.88, TypeScript e Expo Router. Tem cadastro com PIN, login, busca de Hosts, filtros, resultados e detalhe do Host. Os tokens ficam no armazenamento seguro do aparelho (SecureStore). |
| [hospetse-auth-service](https://github.com/hospetse/hospetse-auth-service) | Serviço de autenticação, separado do back-end e com banco próprio. Confirma o e-mail com PIN, guarda a senha com Argon2id e emite o access token JWT (RS256, 15 minutos) e o refresh token com rotação. Depois do cadastro, cria o usuário no back-end por uma rota interna autenticada. Node.js 22, Express 5, Prisma e PostgreSQL. |
| [hospetse-backend](https://github.com/hospetse/hospetse-backend) | API REST principal, com as regras de negócio. Cuida de usuários, perfil do Tutor, pets, busca e detalhe de Hosts e reservas. Valida o JWT com a chave pública do Auth e nunca recebe senha. Node.js, Express 5, Prisma e PostgreSQL, com contrato OpenAPI em `/docs`. |
| [artefatos](https://github.com/hospetse/artefatos) | Artefatos da primeira etapa do projeto (MVP de 2026.1): documentação, diagramas de sequência, plano de testes, DER e diagrama de classes. |
