# Contact list API

Este é um projeto simples de uma API para gerenciar contatos utilizando **Node.js**, **TypeScript**, e **Express**. A API permite adicionar, listar e excluir contatos, com os dados sendo armazenados em um arquivo de texto.

## Funcionalidades

- **Criar um novo contato**
- **Listar os contatos**
- **Excluir um contato**

## Endpoints

A API possui os seguintes endpoints:

- **POST /contato**  
  Cria um novo contato.  
  Corpo da requisição: `{ "name": "João" }`

- **GET /contatos**  
  Lista todos os contatos.  
  Retorna: `{ "contatos": ["João", "Maria", "Pedro"] }`

- **DELETE /contato**  
  Exclui um contato com base no nome fornecido na query.  
  Parâmetro de query: `name`  
  Exemplo de requisição: `/contato?name=João`

## Estrutura do Projeto

- src/routes/index.ts: Definição das rotas da API (criar, listar e excluir contatos).
- src/services/contact.ts: Funções para manipulação de dados de contatos, armazenados em um arquivo de texto.
- src/server.ts: Configuração do servidor Express.
- planejamento.txt: Detalhamento das funcionalidades e planejamento das rotas.

## Dependências

- express: Framework web para Node.js.
- helmet: Middleware de segurança para Express.
- typescript: Compilador TypeScript.
- tsx: Executador de código TypeScript no Node.js.
- @types/express: Tipagens para o Express.
- @types/node: Tipagens para o Node.js.

## Instalação

1. Clone o repositório:

```bash
git clone https://github.com/matheuszuge/list-project
cd list-project
```

2. Instale as dependências

```bash
npm install
```

## Execução

Para rodar o servidor localmente em modo de desenvolvimento, execute:

```bash
npm run dev
```

A aplicação estará rodando em: http://localhost:3000
