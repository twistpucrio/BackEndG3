# BackEndG3

## Getting started

To make it easy for you to get started with GitLab, here's a list of recommended next steps.

Already a pro? Just edit this README.md and make it your own. Want to make it easy? [Use the template at the bottom](#editing-this-readme)!

## Add your files

- [ ] [Create](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#create-a-file) or [upload](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#upload-a-file) files
- [ ] [Add files using the command line](https://docs.gitlab.com/topics/git/add_files/#add-files-to-a-git-repository) or push an existing Git repository with the following command:
# 📦 Store Backend API

Uma API REST completa para uma loja virtual, construída com Node.js, Express e JSON DB.

## 📋 Descrição

Este projeto fornece uma API backend para gerenciar produtos de uma loja virtual, incluindo operações CRUD. Os dados são persistidos em um arquivo JSON usando JSON DB.


## 📁 Estrutura do Projeto

```
ecommerce-backend/
├── package.json
├── server.js
├── data/
│  └── products.json (a ser customizado para cada loja)
└── routes/
   └── products.js
```

## ⚙️ Instalação

1. **Clone o repositório:**
```bash
git clone <url-do-repositorio>
cd furniture-store-backend
```

2. **Instale as dependências:**
```bash
npm install
```

3. **Inicie o servidor:**
```bash
npm start
```
## 📚 Endpoints da API

### 🔍 Produtos

#### Listar todos os produtos

```
GET /api/products
```

Resposta:
```json
{
  "produtos": [
    {
        "id": 1,
        "nome": "produto",
        (...)
    },
     {
        "id": 2,
        "nome": "produto",
        (...)
    },
    (...)
  ]
}
```

#### Buscar produto por id

```
GET /api/products/:id
```

```
// Exemplo para busca com identificador 10
GET /api/products/10
```

Resposta:
```json
{ 
    "id": 10,
    "nome": "produto",
    (...)
}
```


## 📝 Exemplos de Uso
```bash
curl -X GET http://localhost:8000/api/products
```


## 🎯 Modelo de Produto
```json
{
  "id": 000,
  "nome": "Nome do Produto",
  (...)
}
```
