# VK MOBILE PHONES DUMPER
<a href="https://python.org"><img src="https://img.shields.io/badge/python-3-green.svg" /></a>
### Программа, создающая дамп номеров телефонов всех подписчиков группы в ВКонтакте (обновленная версия)

# Как это работает?
* Программа сканирует каждого подписчика заданной вами группы на наличие указанного в открытом доступе мобильного телефона в.
* Программа проверяет номер телефона через фильтр, который можно настроить в ```settings.py```.
* Если номер телефона подходит, то программа записывает его в базу данных ```MySQL```.

# Установка
## Установка Python
1. Скачайте интерпретатор Python 3 с <a href="https://python.org">официального сайта</a>.
2. Начните установку
3. При установке нажмите на кнопку "Customize installation" и убедитесь, что стоит галочка на пункте "pip".
4. Откройте командную строку cmd и пропишите ```pip3 install -r requirements.txt```, если получаете ошибку, то попробуйте ```pip install  -r requirements.txt```
## Установка Open Server
1. Скачайте Open Server Basic с <a href="https://ospanel.io/">официального сайта</a> (если скорость скачивания слишком медленная, попробуйте скачать  <a href="https://soft.mydiv.net/win/files-OpenServer.html">отсюда</a>).
2. Запустите установачный файл и следуйте инструкциям.
# Подготовка
## Open Server и PHP My Admin
1. Перейдите в директорию, куда вы установили Open Server.
2. Запустите от имени администратора ```Open Server x64.exe``` или ```Open Server x32.exe``` в зависимости от вашей архитектуры.
3. Перейдите в трей и нажмите правой кнопкой мыши на красный флажок.
4. Нажмите "Запустить".
5. Перейдите во вкладку "Дополнительно" и выберите пункт "PhpMyAdmin".
6. Войдите под в PHP My Admin (стандартный логин: ```root```, стандартный пароль: пустой])
7. Выберите русский язык.
8. Выберите "Создать БД" в левой панели.
9. Укажите имя базы данных как "vk_dumper" и кодировку "utf8_general_ci".
10. Нажмите "Создать".
## Настройка VK MOBILE PHONES DUMPER
1. Перейдите в директорию, куда вы установили VK MOBILE PHONES DUMPER.
2. Откройте ```settings.py``` любым текстовым редактором.
3. Задайте значение переменной ```access_token``` (строка 10). Получить ВК access token можно <a href="https://vkhost.github.io/">здесь</a>.
4. По желанию настойте остальные переменные и настройки фильтра.
### Теперь все готово для работы программы.
# Использование
### Используя данную программу вы безоговорочно соглашаетесь не использовать ее в незаконных целях или целях заработка.
```python dumper.py [group_id] [params]```
## Параметры запуска программы:
```
-h. --help  :  показать помощь и выйти
-v, --view  :  просматривать логи во время дампа
```
## Примеры:
```
python dumper.py 1 -v
python dumper.py 2293
python dumper.py 44 -v
```









