# cursosjson

Fake REST API for college activity, powered by [json-server](https://github.com/typicode/json-server).

## Resources

| Endpoint | Description |
|---|---|
| `/cursos` | Available courses |
| `/alunos` | Students enrolled in courses |
| `/professores` | Professors and their disciplines |
| `/disciplinas` | Disciplines linked to courses |
| `/empresa` | Company info |

## Getting Started

**Install dependencies:**

```bash
npm install
```

**Start the server:**

```bash
npm start
```

The API will be available at `http://localhost:3000`.

## Example Requests

```bash
# List all courses
GET http://localhost:3000/cursos

# Get a specific course
GET http://localhost:3000/cursos/1

# List all students
GET http://localhost:3000/alunos

# List students from a specific course (using relation)
GET http://localhost:3000/alunos?cursoId=1

# List all professors
GET http://localhost:3000/professores

# List disciplines of a specific course
GET http://localhost:3000/disciplinas?cursoId=1

# Get company info
GET http://localhost:3000/empresa
```

## Available HTTP Methods

json-server supports the full REST API:

- `GET` – Read resources
- `POST` – Create a new resource
- `PUT` – Replace a resource
- `PATCH` – Update part of a resource
- `DELETE` – Remove a resource
