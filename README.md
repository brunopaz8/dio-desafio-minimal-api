# 📚 Minimal API – Desafio DIO

API minimalista em .NET/C# desenvolvida como parte do bootcamp da DIO, seguindo o padrão do repositório *Lista-de-tarefas-api* como referência.

---

## ⚒️ Tecnologias utilizadas

* .NET 7 Minimal API
* C# 11
* Entity Framework Core (MySQL Server)
* Swagger / OpenAPI para documentação automática

---

## 🔧 Funcionalidades

* Operações de CRUD para entidade principal 

  * `GET /entities` – lista todos os itens
  * `GET /entities/{id}` – consulta item por ID
  * `POST /entities` – cria um novo item
  * `PUT /entities/{id}` – atualiza item existente
  * `DELETE /entities/{id}` – remove item

---

## 📄 Endpoints

| Método | Endpoint         | Descrição                  |
| ------ | ---------------- | -------------------------- |
|🔵 GET    | `/entities`      | Retorna todos os itens     |
|🔵 GET    | `/entities/{id}` | Retorna um item por ID     |
|🟢 POST   | `/entities`      | Cria um novo item          |
|🟠 PUT    | `/entities/{id}` | Atualiza um item existente |
|🔴 DELETE | `/entities/{id}` | Remove um item             |

---

## 🚀 Como Executar o Projeto

1️⃣. Clone o repositório

```bash
git clone https://github.com/brunopaz8/dio-desafio-minimal-api.git
cd dio-desafio-minimal-api.git
```

2️⃣. Restaure os pacotes e rode as migrations

```bash
dotnet restore
dotnet ef database update
```

3️⃣. Execute o projeto

```bash
dotnet run
```

> Certifique-se de ter o [.NET SDK](https://dotnet.microsoft.com/download) instalado em sua máquina.

A API estará disponível em: `https://localhost:5001` ou `http://localhost:5000`

---

### 📗 Documentação **Swagger**
A API conta com documentação interativa via **Swagger UI**, facilitando testes e visualização dos endpoints. Após iniciar a aplicação, acesse:

🟢 **Swagger UI:** [http://localhost:5226/swagger/index.html](http://localhost:5226/swagger/index.html)

---

## 🚫 Observações

* Certifique-se de configurar corretamente a `connectionString` no `appsettings.json`.
* O projeto está configurado para rodar em modo `Development` por padrão.
