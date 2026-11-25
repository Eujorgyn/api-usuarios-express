# API de usuários com Express

API REST simples em **Node.js + Express** que lista e consulta usuários lidos de um arquivo JSON. Foi um exercício de introdução a rotas, parâmetros de URL e leitura de arquivos com `fs`.

![Node.js](https://img.shields.io/badge/Node.js-339933?logo=node.js&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?logo=express&logoColor=white)

## Rotas

| Método | Rota | Descrição |
|---|---|---|
| GET | `/listUsers` | Retorna todos os usuários |
| GET | `/listUser/:id` | Retorna o usuário com o `id` informado |

## Como executar

```bash
npm install
npm start
```

O servidor sobe em `http://localhost:8081`. Exemplos de teste:

```bash
curl http://localhost:8081/listUsers
curl http://localhost:8081/listUser/2
```

Resposta de `/listUser/2`:

```json
{ "name": "suresh", "profession": "librarian", "id": 2 }
```

## Arquivos

| Arquivo | Descrição |
|---|---|
| `server.js` | Servidor Express e definição das rotas |
| `users.json` | Base de dados de exemplo (fictícia) |

## Autor

**Jorge Gabriel**, estudante de Análise e Desenvolvimento de Sistemas na UNIFOR.
[GitHub](https://github.com/Eujorgyn) · jorgegabrielpinheirofrutuoso@gmail.com
