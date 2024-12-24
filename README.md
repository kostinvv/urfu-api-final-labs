# urfu-api-final-labs

## Функциональные возможности

### TODO-сервис
- cоздание задачи;
- чтение задач (все или по идентификатору);
- обновление задачи;
- удаление задачи.

Дополнительно реализовано:
- метод PATCH (частичное обновление);
- GET /items добавлена пагинация.
![Alt text](docs/Pasted%20image%2020241224194653.png)
![Alt text](docs/Pasted%20image%2020241224194730.png)
![Alt text](docs/Pasted%20image%2020241224201648.png)
![Alt text](docs/Pasted%20image%2020241224201713.png)

### Short URL-сервис
- cоздание короткой ссылки для длинного URL;
- перенаправление по короткой ссылке;
- получение информации о сокращённой ссылке;

Дополнительно реализовано: удаление ссылки.

![Alt text](docs/Pasted%20image%2020241224195126.png)
![Alt text](docs/Pasted%20image%2020241224195142.png)
![Alt text](docs/Pasted%20image%2020241224201904.png)
![Alt text](docs/Pasted%20image%2020241224201421.png)
![Alt text](docs/Pasted%20image%2020241224201447.png)

## Установка и запуск

### Запуск с использованием Docker Hub

1. Скачайте образы из Docker Hub:
    ```bash
    docker pull kostinvv/todoapp
    docker pull kostinvv/shorturl
    ```

2. Запустите контейнеры с использованием скачанных образов:
    ```bash
    docker run -p 8001:80 kostinvv/todoapp
    docker run -p 8000:80 kostinvv/shorturl
    ```

3. TODO-сервис будет доступен по адресу: [http://localhost:8001/docs](http://localhost:8000/docs)

4. Short URL-сервис будет доступен по адресу: [http://localhost:8000/docs](http://localhost:8001/docs)
