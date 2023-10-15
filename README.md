# todolist

Iniciar a aplicação via debug e após iniciar será possível realizar as seguintes ações via API:
- Criar um usuario;
- Adicionar uma tarefa ao usuario;
- Buscar a tarefa do usuario via login cadastrado anteriormente.

  Exemplo:
  1 - POST: http://localhost:8080/users/ <br>
  { <br>
    "name": "kleiton gomes", <br>
    "username": "abacate", <br>
    "password": "123456" <br>
  } <br>
<br>
  2 - POST: http://localhost:8080/tasks/ <br>
  { <br>
    "description": "Tarefa teste", <br>
    "title": "Gravacao de aula", <br>
    "priority": "BAIXA", <br>
    "startAt": "2023-10-20T12:30:00", <br>
    "endAt": "2023-10-21T15:35:00", <br>
    "idUser": "f0d072cc-6221-43b9-a800-724e0f43a063" <br>
} <br>
<br>
3 - GET: http://localhost:8080/tasks/ <br>
BASIC AUTH: <br>
abacate <br>
123456 <br>
 
