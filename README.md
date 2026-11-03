# API de Produtos – Banco de Dados Não Relacional

## Sobre o projeto

Este projeto consiste no desenvolvimento de uma API REST para gerenciamento de produtos, utilizando um banco de dados não relacional.

A API permite realizar operações de cadastro, consulta, atualização e exclusão de produtos, utilizando os métodos HTTP.

## Tecnologias utilizadas

- **Node.js:** ambiente de execução JavaScript.
- **Express:** biblioteca utilizada para criar a API.
- **MongoDB:** banco de dados não relacional.
- **MongoDB Atlas:** serviço utilizado para hospedar o banco de dados.

## Funcionalidades

A API possui as seguintes operações:

| Método HTTP | Rota | Funcionalidade |
|---|---|---|
| POST | `/produtos` | Cadastrar um produto |
| GET | `/produtos` | Listar todos os produtos |
| GET | `/produtos/:id` | Consultar um produto específico |
| PUT | `/produtos/:id` | Atualizar um produto |
| DELETE | `/produtos/:id` | Excluir um produto |

## Organização do projeto

```text
api-produtos-naorelacional/
│
├── node_modules/
├── .env
├── .gitignore
├── index.js
├── package.json
├── package-lock.json
└── README.md
```

## Como executar o projeto

1. Abra a pasta do projeto no Visual Studio Code.
2. Abra o terminal.
3. Instale as dependências:

```bash
npm install
```

4. Configure a variável `MONGO_URI` no arquivo `.env`, utilizando a conexão do MongoDB Atlas.
5. Inicie a API:

```bash
node --env-file=.env index.js
```

Após iniciar, a API ficará disponível na porta **3000**.

## Testando a API

As requisições podem ser realizadas utilizando o Thunder Client ou outra ferramenta de testes de API.

Endereço principal:

```text
http://localhost:3000
```

Exemplo de cadastro de produto:

```json
{
    "nome": "Notebook",
    "preco": 2500,
    "quantidade": 10
}
```

## Banco de dados

O projeto utiliza o banco de dados chamado `loja`, com uma coleção chamada `produtos`.

Os dados são armazenados no formato de documentos, característica dos bancos de dados não relacionais.

## Objetivo

O objetivo da atividade é praticar a criação de uma API utilizando Node.js e Express, além de aprender a realizar operações CRUD (Create, Read, Update e Delete) utilizando o MongoDB.

---

**Projeto desenvolvido para fins educacionais.**