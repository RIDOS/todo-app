# RESFull Golang

## Введение
Данный проект был выполнен в учебных целях. Проект был сформирован @zhashkevych/todo-app.

## Начало работы

Подтянуть контейнер с базой данных **Postgres**: 
```bash
docker pull postgres 
```

Запустить контейнер:
```bash
docker run --name=todo-db -e POSTGRES_PASSWORD='qwerty' -p 5436:5432 -d --rm postgres
```

Подтянуть миграции в папке `./schema`.

Запустить проект:
```bash
go cmd/main.go
```