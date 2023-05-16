# Movie Rental Shop

## Description

API with Django Rest Framework in order to manage users, movies and purchases, including authentication and route permissions for different types of users.

## Endpoints

| HTTP Method | Description    | Endpoint                             | User Types          | Authentication Required |
| ----------- | -------------- | ------------------------------------ | ------------------- | ----------------------- |
| POST        | Register movie | `/api/movies/`                       | Employees           | Authenticated           |
| GET         | List movies    | `/api/movies/`                       | Users and Employees | No Authentication       |
| GET         | List movie     | `/api/movies/<int:movie_id>/`        | Users and Employees | No Authentication       |
| DELETE      | Delete movie   | `/api/movies/<int:movie_id>/`        | Employees           | Authenticated           |
| POST        | Create order   | `/api/movies/<int:movie_id>/orders/` | Users and Employees | Authenticated           |
| PATCH       | Update movie   | `/api/movies/<int:movie_id>/orders/` | Users and Employees | No Authentication       |
| POST        | Register user  | `/api/users/`                        | Users and Employees | No Authentication       |
| GET         | List users     | `/api/users/`                        | Employees           | Authenticated           |
| POST        | Login          | `/api/users/login/`                  | Users and Employees | No Authentication       |
| GET         | List user      | `/api/users/<int:user_id>/`          | Users and Employees | Authenticated           |
| PATCH       | Update user    | `/api/users/<int:user_id>/`          | Users and Employees | Authenticated           |

## Run the tests for each task

Example:

- Task 1

```shell
pytest --testdox -vvs tests/tarefas/tarefa_1/
```

- Task 2

```shell
pytest --testdox -vvs tests/tarefas/tarefa_2/
```

- Task 3

```shell
pytest --testdox -vvs tests/tarefas/tarefa_3/
```

- Task 4

```shell
pytest --testdox -vvs tests/tarefas/tarefa_4/
```
