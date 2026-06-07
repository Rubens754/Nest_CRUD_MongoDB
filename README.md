# CRUD de Usuários com NestJS e MongoDB Atlas

## 📌 Sobre o Projeto

Este projeto consiste em uma API REST desenvolvida utilizando NestJS e MongoDB Atlas. O objetivo é demonstrar a implementação de operações CRUD (Create, Read, Update e Delete) para gerenciamento de usuários.

A aplicação foi construída utilizando boas práticas de desenvolvimento backend, incluindo organização modular, variáveis de ambiente e integração com banco de dados em nuvem.

---

## 🚀 Tecnologias Utilizadas

* NestJS
* TypeScript
* MongoDB Atlas
* Mongoose
* Node.js
* Thunder Client

---

## 📂 Estrutura do Projeto

```text
src/
│
├── users/
│   ├── dto/
│   ├── schemas/
│   ├── users.controller.ts
│   ├── users.service.ts
│   └── users.module.ts
│
├── app.module.ts
└── main.ts
```

---

## ⚙️ Configuração do Ambiente

### Clonar o repositório

```bash
git clone https://github.com/SEU_USUARIO/Nest_CRUD_MongoDB.git
```

### Entrar na pasta do projeto

```bash
cd Nest_CRUD_MongoDB
```

### Instalar dependências

```bash
npm install
```

---

## 🔐 Variáveis de Ambiente

Crie um arquivo `.env` na raiz do projeto:

```env
PORT=3000

MONGODB_URI=sua_string_de_conexao_mongodb
```

---

## ▶️ Executando o Projeto

Modo desenvolvimento:

```bash
npm run start:dev
```

A aplicação ficará disponível em:

```text
http://localhost:3000
```

---

## 📚 Endpoints Disponíveis

### Criar usuário

```http
POST /users
```

Exemplo:

```json
{
  "nome": "Rubens",
  "email": "rubens@gmail.com",
  "idade": 26
}
```

---

### Listar usuários

```http
GET /users
```

---

### Buscar usuário por ID

```http
GET /users/:id
```

---

### Atualizar usuário

```http
PATCH /users/:id
```

Exemplo:

```json
{
  "idade": 27
}
```

---

### Remover usuário

```http
DELETE /users/:id
```

---

## 🗄️ Banco de Dados

Este projeto utiliza o MongoDB Atlas como banco de dados em nuvem.

Coleção principal:

```text
users
```

Campos armazenados:

| Campo | Tipo   |
| ----- | ------ |
| nome  | String |
| email | String |
| idade | Number |

---

## 🧪 Testes

Os endpoints podem ser testados utilizando:

* Thunder Client
* Postman
* Insomnia

---

## 👨‍💻 Autor

Rubens Melo

Projeto desenvolvido para fins de estudo e aprendizado de NestJS, MongoDB Atlas e APIs REST.
