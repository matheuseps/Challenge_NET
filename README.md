API Challenge
API Challenge é uma aplicação ASP.NET Core para gerenciar usuários e cadastros, com autenticação via Auth0 e funcionalidades de Machine Learning integradas via ML.NET.

				Tecnologias Utilizadas
	ASP.NET Core 8.0
	Entity Framework Core (SQL Server e Oracle)
	Auth0 para autenticação JWT
	Swashbuckle para documentação Swagger
	ML.NET para Machine Learning
	xUnit e Moq para testes
	Configuração do Projeto
	Pré-requisitos
	.NET 8.0 SDK
	Banco de dados SQL Server ou Oracle
	Conta no Auth0


- Passos
1. Clone o repositório e acesse o diretório:

git clone https://github.com/seu-usuario/api-challenge.git
cd api-challenge

2. Execute as migrações do banco de dados:

dotnet ef database update

3. Inicie a aplicação:

dotnet run


Acesse a documentação em http://localhost:5000/swagger.

Endpoints Principais:

GET /api/usuario: Lista todos os usuários.
GET /api/usuario/{id}: Retorna um usuário específico.
POST /api/usuario: Cria um novo usuário.
PUT /api/usuario/{id}: Atualiza um usuário.
DELETE /api/usuario/{id}: Exclui um usuário.

Autenticação

O projeto usa Auth0 para autenticação JWT. Envie o token JWT no header Authorization para acessar endpoints protegidos:

Authorization: Bearer SEU_TOKEN
