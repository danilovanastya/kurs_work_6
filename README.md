# Cервис управления рассылками, администрирования и получения статистики 

## Краткое описание
Наш сервис для рассылки, с использованием:  
База данных - Postgresql

## Приложения
* Блог
* Клиент
* Сообщение для рассылки
* Рассылка
* Пользователь

_Для запуска проекта необходимо клонировать репозиторий и создать и активировать виртуальное окружение:_ 
```
python3 -m venv venv

source venv/bin/activate
```
_Установить зависимости:_
```
pip install -r requirements.txt
```
_Для работы с переменными окружениями необходимо создать файл .env и заполнить его согласно файлу .env.sample_
```
Не забывайте создать базу данных в pgAdmin с вашим названием, у которой есть Пользователь и Имя из .env
```
_Выполнить миграции:_
```
python3 manage.py migrate
```
_Для заполнения БД запустить команду:_

```
python3 manage.py fill
```

_Для создания администратора запустить команду:_

```
python3 manage.py csu
```

_Для запуска redis_:

```
redis-cli
```

_Для запуска приложения:_

```
python3 manage.py runserver
```
