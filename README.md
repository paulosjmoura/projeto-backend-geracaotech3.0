Backend API - Core Project
API robusta desenvolvida em Node.js, estruturada em camadas para garantir escalabilidade, fácil manutenção e clara separação de responsabilidades.

Tecnologias
*Runtime: Node.js

*Framework: Express

*ORM/DB: Sequelize + PostgreSQL

*Segurança: JWT (Autenticação) & Bcrypt (Hashing)

*Testes: Jest & Supertest

*Documentação: Swagger

Arquitetura do Sistema
O projeto utiliza o padrão MVC + Services, isolando a lógica de negócio dos controladores.

Plaintext
src/
├── config/       # Ajustes de Infra/DB
├── controllers/  # Orquestração de Requisições
├── services/     # Regras de Negócio (Core)
├── models/       # Abstração de Dados (Sequelize)
├── routes/       # Definição de Endpoints
└── middleware/   # Filtros e Segurança

Configuração e Instalação
Clone e Instale:

Bash
git clone <url-do-repositorio>
cd project-root
npm install

Variáveis de Ambiente:
Crie um arquivo .env na raiz com as credenciais do banco e a Secret do JWT:
DB_HOST, DB_USER, DB_PASS, DB_NAME, DB_PORT, JWT_SECRET.

Banco de Dados:
Bash
npx sequelize-cli db:migrate

Execução
Desenvolvimento: npm run dev
Produção: npm start
Testes: npm test

Acesse em: http://localhost:3000

Funcionalidades Principais
Auth: Sistema de login com proteção via JWT.
Gerenciamento: CRUD completo de Usuários, Categorias e Produtos.
Produtos: Suporte para variações (opções) e upload de imagens.
Docs: Swagger UI disponível em /api-docs.

Contribuição
Faça o Fork do projeto.
Crie uma Branch (git checkout -b feature/nova-feature).
Dê o Commit (git commit -m 'Adiciona nova feature').
Envie o Push e abra um Pull Request.

Licença: ISC
