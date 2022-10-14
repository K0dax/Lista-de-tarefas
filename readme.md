## Lista de tarefas
Essa aplicação foi feita com NodeJS. Uma simples <b>lista de tarefas</b> para me organizar no dia-a-dia.

## Tecnologias 
Aqui estão as tecnologias utilizadas neste projeto.

* Node JS
* Express
* Mongoose
* MongoDB


## Serviços usados

* Github
* MongoDB Atlas


## Começando

Dependências
 - Dotenv
 - Express
 - Mongoose
 - Nodemon

Para clonar o projeto:
```bash
git clone https://github.com/K0dax/Lista-de-tarefas.git
```

Para rodar o projeto:
```bash
npm start
```

Home do app
```
http://localhost:3000
```

## Endpoints e Features
### GET /api/v1/tasks
Ver todas as tarefas
```json
{
  "tasks": [
    {
      "completed": true,
      "_id": "1",
      "name": "comprar abacate",
      "__v": 0
    },
    {
      "completed": false,
      "_id": "2",
      "name": "fazer vitamina",
      "__v": 0
    }
  ]
}
```

### POST /
Adicionar nova tarefa
```
Content-Type: application/json
{
    "name": "Estudar DB",
    "completed": "false"
}
```

### GET /api/v1/tasks/:id
Ver uma Tarefa

Response
```json
{
  "task": {
    "completed": true,
    "_id": "1",
    "name": "teste",
    "__v": 0
  }
}
```

### PATCH /api/v1/tasks/:id
Atualizar a tarefa

Request
```
Content-Type: application/json
{
    "name": "outro teste"
}
```
Response
```json
{
  "task": {
    "completed": true,
    "_id": "2",
    "name": "outro teste",
    "__v": 0
 }
}
```

### DELETE /api/v1/tasks/:id
Deleta uma tarefa

Response
```json
{
  "task": {
    "completed": false,
    "_id": "1",
    "name": "delete teste",
    "__v": 0
 }
}
```

## Links
  - Repositório: https://github.com/K0dax/Lista-de-tarefas


  ## Autor

  * **Yan "K0da" Carlos** 

  Por favor, siga o github e junte-se a nós!
