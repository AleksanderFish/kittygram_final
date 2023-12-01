# Kittygram

![Build Status](https://github.com/AleksanderFish/kittygram_final/actions/workflows/main.yml/badge.svg
)

## Описание
Kittygram - это веб-приложение, предназначенное для создания и управления профилями "котиков". Это проект для любителей котов, позволяющий делиться фотографиями и историями своих питомцев. Он позволяет добавлять фотографии, имя, год рождения, навыки котов на сайт.

## Стек Технологий
- Django
- Docker
- GitHub Actions


## Настройка и Развертывание
### Как запустить проект:

Клонировать репозиторий и перейти в него в командной строке:

```
git clone https://github.com/yandex-praktikum/kittygram_backend.git
```

```
cd kittygram_backend
```

Cоздать и активировать виртуальное окружение:

```
python3 -m venv env
```

* Если у вас Linux/macOS

    ```
    source env/bin/activate
    ```

* Если у вас windows

    ```
    source env/scripts/activate
    ```

```
python3 -m pip install --upgrade pip
```

Установить зависимости из файла requirements.txt:

```
pip install -r requirements.txt
```

Выполнить миграции:

```
python3 manage.py migrate
```

Запустить проект:

```
python3 manage.py runserver
```


### Настройка Переменных Окружения
Создайте файл `.env` в корневой директории и заполните необходимые переменные:

DB_NAME=example
DB_USER=user
DB_PASSWORD=password

### Запуск с Docker

docker-compose up -d


## Тестирование
Для запуска тестов выполните:

pytest


## CI/CD с GitHub Actions
В файле `kittygram_workflow.yml` описаны шаги для непрерывной интеграции и развертывания приложения.

## Автор
Александр Фиш

