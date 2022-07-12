# note-service-nodejs

# Тестовое задание для Back-end программиста

**Необходимо разработать бэкенд для сервиса заметок используя микросервисную архитектуру.**

Структура сервисов:

- Сервис пользователей
    - Авторизация + регистрация (JWT)
    - После регистрации отправлять пользователю приветственное письмо.
    - CRUD пользователей
- Сервис записей
    - Авторизация (JWT)
    - CRUD записей
- Сервис рассылки E-mail уведомлений
    - Сервис должен обрабатывать сообщения в порядке очереди ( 1 сообщение за 1 секунду), для этого стоит использовать брокеры (RabbitMQ, *Kafka и т.д.)

Требования к сервисам:

- Необходимо поместить каждый сервис в отдельный докер контейнер (Dockerfile).
- Каждый сервис должен содержать отдельный Http сервер.
- Каждый сервис должен работать со своей базой данных.
- Уметь горизонтально масштабироваться (одновременно может быть запущено 1 + n копий сервиса).

Плюсом будет:

- Подключение автоматизированной документации (Swagger / AsyncApi).

<aside>
✅ Можно использовать:

</aside>

- Fastify / Express для Http сервера
- NodeJS
- Базы данных MySQL, *PostgreSQL
- ORM-фреймворки (TypeORM / *Sequelize)
- Месседж брокеры RabbitMQ, *Kafka или др.

***** - предпочтительнее использовать

<aside>
❌ Нельзя использовать:

</aside>

- NestJS

**Результат тестового задания необходимо отправить в наш whatsapp ответным сообщением. В результате должно быть указано:**

1. Ссылка на репозиторий в [https://github.com/](https://github.com/) .
2. С какими проблемами столкнулись во время выполнения тестового задания.

C уважением, Welbex
