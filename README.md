🗂️ TaskManagerApp

Projeto prático de gerenciamento de tarefas desenvolvido com C# e .NET aplicando os princípios de DDD (Domain-Driven Design) e CQRS (Command Query Responsibility Segregation).

📚 Sobre o Projeto

Este projeto tem como objetivo demonstrar uma aplicação estruturada com os padrões de arquitetura DDD + CQRS. Ele implementa um sistema simples de gerenciamento de tarefas com as operações básicas de:

Criar tarefa (POST /api/tasks)

Listar tarefas (GET /api/tasks)

As tarefas são armazenadas em memória (para fins de demonstração) e possuem título, descrição, status e data de criação.

🧱 Arquitetura

O projeto está dividido nas seguintes camadas:

TaskManagerApp/
│
├── Domain/         → Entidades, enums e interfaces (regra de negócio)
├── Application/    → Comandos, consultas (CQRS) e DTOs
├── Infrastructure/ → Repositório em memória
├── API/            → Controller e endpoints REST

🔄 Tecnologias e Padrões Usados

✅ .NET 6 / .NET 7

✅ C#

✅ ASP.NET Core Web API

✅ DDD (Domain-Driven Design)

✅ CQRS (Command Query Responsibility Segregation)

✅ Repository Pattern

✅ Injeção de dependência

✅ Programação orientada a objetos

🚀 Como executar o projeto

Pré-requisitos:

.NET SDK instalado

Passos:

# Clone o repositório
git clone https://github.com/seu-usuario/TaskManagerApp.git
cd TaskManagerApp

# Execute a aplicação
dotnet run --project API

Depois disso, acesse:

http://localhost:5000/api/tasks

🔍 Exemplos de uso

Criar uma tarefa

POST /api/tasks

{
  "title": "Estudar CQRS",
  "description": "Entender os conceitos e aplicar em um projeto prático"
}

Listar tarefas

GET /api/tasks

[
  {
    "id": "xxxxxx",
    "title": "Estudar CQRS",
    "description": "Entender os conceitos e aplicar em um projeto prático",
    "status": "Pending",
    "createdAt": "2025-04-13T14:30:00Z"
  }
]

✍️ Autor

Feito com 💻 por Juan Diniz



📌 Observações

Este projeto tem fins educacionais para demonstração dos padrões DDD e CQRS. 
Para ambientes reais, recomenda-se o uso de banco de dados, validações, logging, versionamento de API, etc.
