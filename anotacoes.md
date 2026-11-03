# Anotações – API de Produtos

## Sobre a atividade

Nesta atividade, foi desenvolvida uma API para cadastrar, consultar, atualizar e excluir produtos, utilizando Node.js, Express e MongoDB.

## Tecnologias utilizadas

- **Node.js:** ambiente utilizado para executar o JavaScript.
- **Express:** utilizado para criar as rotas da API.
- **MongoDB:** banco de dados não relacional utilizado para armazenar os produtos.
- **MongoDB Atlas:** serviço utilizado para hospedar o banco de dados.

## Principais comandos e recursos

- `require()`: importa os módulos utilizados no projeto.
- `express()`: cria a aplicação Express.
- `express.json()`: permite receber dados no formato JSON.
- `MongoClient`: permite realizar a conexão com o MongoDB.
- `insertOne()`: cadastra um novo produto.
- `find().toArray()`: consulta todos os produtos.
- `findOne()`: consulta um produto específico.
- `updateOne()`: atualiza um produto.
- `deleteOne()`: exclui um produto.
- `ObjectId`: permite trabalhar com os identificadores dos documentos do MongoDB.
- `process.env.MONGO_URI`: acessa o endereço de conexão armazenado na variável de ambiente.

## Rotas da API

| Método | Rota | Função |
|---|---|---|
| POST | `/produtos` | Cadastrar produto |
| GET | `/produtos` | Listar produtos |
| GET | `/produtos/:id` | Consultar produto pelo ID |
| PUT | `/produtos/:id` | Atualizar produto |
| DELETE | `/produtos/:id` | Excluir produto |

## Banco de dados

- Banco de dados: `loja`
- Coleção: `produtos`

Os produtos são armazenados como documentos dentro da coleção.

## Execução do projeto

Para executar a API, é necessário instalar as dependências com:

```bash
npm install
```

Depois, iniciar o servidor com:

```bash
node --env-file=.env index.js
```

A API utiliza a porta `3000`.

## Conclusão

Com esta atividade, foi possível praticar a criação de uma API utilizando Node.js, aprender a trabalhar com as rotas do Express e realizar operações CRUD em um banco de dados não relacional MongoDB.