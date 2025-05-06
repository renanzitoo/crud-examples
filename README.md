# 📚 Example CRUDs in Various Languages

This repository contains **several examples of registration APIs (CRUD)** developed in **different programming languages**, all connected to a **PostgreSQL** database.  
The goal is to **help beginners** or those learning a new language with practical and functional references.

---

## 🚀 Technologies and Standards

- Various languages (e.g., Node.js, Python, Go, etc.)
- Database: **PostgreSQL**
- Standardized `.env` file for easy configuration
- Common structure: `create`, `read`, `update`, `delete` routes

---

## 📂 Repository Structure

<pre> crud / 
    ├── node-crud/ 
    ├── python-crud/ 
    ├── go-crud/ 
    └── ...  </pre>

Each folder contains:
- API source code
- Usage instructions in the internal `README.md`
- Example `.env` file

---

# 🌐 API Endpoints - Person

The API follows the REST pattern and allows the creation, reading, updating, and deletion of people.

---

## 🧾 `Person` resource JSON

### Request (POST / PUT)

```json
{
  "nome": "John Doe",
  "email": "john.doe@example.com",
  "data_nascimento": "1995-07-20"
}
```

### Response (GET / POST / PUT)

```json
{
  "id": 1,
  "nome": "John Doe",
  "email": "john.doe@example.com",
  "data_nascimento": "1995-07-20",
  "idade": 29
}
```

> ⚠️ The `idade` (age) field is calculated in the backend based on `data_nascimento` (date of birth).

---

## 📌 Endpoints

| Method | Route              | Action                          |
|--------|--------------------|---------------------------------|
| GET    | `/pessoas`         | Lists all people                |
| GET    | `/pessoas/:id`     | Returns a specific person       |
| POST   | `/pessoas`         | Creates a new person            |
| PUT    | `/pessoas/:id`     | Updates all data                |
| PATCH  | `/pessoas/:id`     | Updates partial data            |
| DELETE | `/pessoas/:id`     | Deletes a person                |

---

## ✅ Expected HTTP Status

- `200 OK`: Success in the request
- `201 Created`: Resource created successfully
- `400 Bad Request`: Invalid data
- `404 Not Found`: Person not found
- `500 Internal Server Error`: Unexpected server error

---

## 🧪 How to use

1. Choose a language from the corresponding folder
2. Install dependencies (check the `README.md` inside the folder)
3. Configure the PostgreSQL database and the `.env` file
4. Run the API locally and test the endpoints

---

## 🤝 Contributions

Contributions are welcome!  
Feel free to open an issue, suggest improvements, or add CRUDs in new languages.

---

## 📄 License

This project is licensed under the [MIT](LICENSE) license.

# 📚 CRUDs de Exemplo em Diversas Linguagens  - PT-BR

Este repositório contém **diversos exemplos de APIs de registro (CRUD)** desenvolvidos em **diferentes linguagens de programação**, todos conectando a um banco de dados **PostgreSQL**.  
O objetivo é **ajudar iniciantes** ou quem está aprendendo uma nova linguagem com referências práticas e funcionais.

---

## 🚀 Tecnologias e Padrões

- Linguagens diversas (ex: Node.js, Python, Go, etc.)
- Banco de dados: **PostgreSQL**
- Arquivo `.env` padronizado para facilitar a configuração
- Estrutura comum: rotas de `create`, `read`, `update`, `delete`

---

## 📂 Estrutura do Repositório
<pre> crud / 
    ├── node-crud/ 
    ├── python-crud/ 
    ├── go-crud/ 
    └── ...  </pre>

Cada pasta contém:
- Código-fonte da API
- Instruções de uso no `README.md` interno
- Exemplo de `.env`

---

## 🌐 Endpoints da API - Pessoa

A API segue o padrão REST e permite o cadastro, leitura, atualização e remoção de pessoas.

---

## 🧾 JSON do recurso `Pessoa`

### Requisição (POST / PUT)

```json
{
  "nome": "John Doe",
  "email": "john.doe@example.com",
  "data_nascimento": "1995-07-20"
}
```

### Resposta (GET / POST / PUT)

```json
{
  "id": 1,
  "nome": "John Doe",
  "email": "john.doe@example.com",
  "data_nascimento": "1995-07-20",
  "idade": 29
}
```

> ⚠️ O campo `idade` é calculado no backend com base na `data_nascimento`.

---

## 📌 Endpoints

| Método | Rota              | Ação                            |
|--------|-------------------|---------------------------------|
| GET    | `/pessoas`        | Lista todas as pessoas          |
| GET    | `/pessoas/:id`    | Retorna uma pessoa específica   |
| POST   | `/pessoas`        | Cria uma nova pessoa            |
| PUT    | `/pessoas/:id`    | Atualiza todos os dados         |
| PATCH  | `/pessoas/:id`    | Atualiza dados parciais         |
| DELETE | `/pessoas/:id`    | Remove uma pessoa               |

---

## ✅ Status HTTP esperados

- `200 OK`: Sucesso na requisição
- `201 Created`: Recurso criado com sucesso
- `400 Bad Request`: Dados inválidos
- `404 Not Found`: Pessoa não encontrada
- `500 Internal Server Error`: Erro inesperado no servidor

---


## 🧪 Como usar

1. Escolha uma linguagem na pasta correspondente
2. Instale as dependências (consultar o `README.md` da pasta)
3. Configure o banco PostgreSQL e o `.env`
4. Rode a API localmente e teste os endpoints

---

## 🤝 Contribuições

Contribuições são bem-vindas!  
Sinta-se à vontade para abrir uma _issue_, sugerir melhorias ou adicionar CRUDs em novas linguagens.

---

## 📄 Licença

Este projeto está sob a licença [MIT](LICENSE).
