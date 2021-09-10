# 🎨 Majestic Docker Сontainer


Данное окружение полностью настроено и готово к работе с [**Majestic Framework**](https://github.com/majestic-studio/Majestic-Framework), его отдельными [компонентами](https://github.com/majestic-studio), либо другими проектами написанными на [**PHP**](https://php.ornetg/).



### ✨ **MDC** включает в себя следующие компоненты:

- **Окружение**
  - [PHP](https://php.ornetg/)
  - [Enable JIT](https://wiki.php.net/rfc/jit)
- **Сервер**:
  - [Nginx](https://hub.docker.com/_/nginx)
  - [Apache](https://hub.docker.com/_/httpd)

- **Базы данных**:
  - [MariaDB](https://hub.docker.com/_/mariadb)
  - [MySQL](https://hub.docker.com/_/mysql)
  - [Postgres](https://hub.docker.com/_/postgres)
  - [Redis](https://hub.docker.com/_/redis)

- **Управление базами данных**:
  - [PHPMyAdmin](https://hub.docker.com/_/phpmyadmin)

  Всё настроено и готово к работе с первых секунд!


Структура папок и файлов:
- **Docker**
  - **Addons**: основыые настройки окружения контейнеров
  - **DataBase**: содержимое базы данных MySQL, MariaDB и так далее.
- **Logs**: папка содержит вседоступные логи приложения
  - **Nginx**: логи веб-сервера Nginx
  - **Apache**: логи веб-сервера Apache


## Настройки
Все настройки вынесены в общий с Majestic файл `.env`
- db_username
  - Содержит имя базы данных
- db_password
  - Содержит пароль базы данных
- db_driver
  - Содержит драйвер (тип) базы данных, будь то MySQL или MariaDB

## Запуск контейнера
Для начала необходимо установить все внешние зависимости, сделать это можно командой 
```shell script
docker-compose build
```
Данная команда установит все необходимые образы для запуска необходимых контейнеров.


После чего мы можем запустить сам Docker
```shell script
docker-compose up -d
```


*Этот README был создан с ❤️*
