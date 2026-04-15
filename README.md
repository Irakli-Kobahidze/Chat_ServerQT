# Chat_ServerQT

Chat_ServerQT - Сервер чата
Многопоточный чат-сервер с клиент-серверной архитектурой, поддержкой приватных и публичных сообщений, админ-панелью и графическим интерфейсом для мониторинга. Ссылка на клиент:
https://github.com/Irakli-Kobahidze/Chat__ClientQT

Ключевые возможности:

Регистрация и аутентификация пользователей (хеширование паролей по алгоритму SHA-1)

Приватные и публичные сообщения

Админка с управлением пользователями (бан, разблокировка, удаление)

Графический интерфейс для мониторинга (Qt6) — онлайн-пользователи, статистика, логи

Хранение данных в MySQL (пользователи, сообщения)

Поддержка неблокирующего ввода-вывода (poll)

Технологии:

Язык — C++17. Сеть — сокеты POSIX (TCP/IP), опрос. База данных — MySQL, MySQL Connector/C++. Графический интерфейс — Qt6. Сборка — CMake, qmake. Хеширование — SHA-1 (собственная реализация). Платформа — Linux.

Установка и запуск


Установка зависимостей (Ubuntu/Debian)
sudo apt update sudo apt install build-essential cmake qt6-base-dev libmysqlcppconn-dev mysql-server Настройка базы данных: CREATE DATABASE bd; CREATE USER 'dbeaver'@'localhost' IDENTIFIED BY 'dbeaver123'; GRANT ALL PRIVILEGES ON bd.* TO 'dbeaver'@'localhost'; FLUSH PRIVILEGES;

Сборка: скопируйте директорию в QT: https://github.com/Irakli-Kobahidze/Chat_ServerQT Запустите.
