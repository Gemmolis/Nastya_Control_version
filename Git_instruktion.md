# Инструкция по работе с Git-ом

> **git init**  - создание пустого репозитория в выбранной папке.

> **git add <Имя файла>** - Добавляет файл к следующему commit

> **git add .**  - добавляет все файлы к следующему commit
> **git commit -m "some comments"** - добавляет комментарий к изменению

Зеленая полоска слева сигнализирует, что информация не сохранена в Git

> **git commit -am "some comments"** - заменяет две команды **git add** и **git commit**  Срабатывает только если ранее уже были использованы обе команды по отдельности.

>**git log**  вывод на экран истории всех коммитов с их хеш-кодами

>**git log graph**  выводит ветки в графическом виде

>**git log oneline** выводит commit в сжатом виде

> **git diff** показывает что добавилось с момента последнего commit

> **git checkout <код коммита> (достаточно первых 5 цифр)** переносит на ту стадии при которой создан commit, то же самое для веток

> **git checkout master** - возвращает на текущие изменения то же самое для веток, вместо master возможно main

>**git branch <название ветки>** создает ветку с указанным именем

>**git branch** позволяет просмотреть список всех имеющихся веток в нашем репозитории

>**git checkout <имя ветки>** переключает на указанную ветку

>**git checkout -b <имя ветки>** создает ветку и сразу нанее переключает

>**git merge <имя ветки>** соединяет названную ветку с текущей

>**git branch -d <название ветки>** удаляет ненужную ветку проверяя на наличие merge, если проверка не требуется то ставим -D


## Как связать локальный репозиторий и GitHub

1. Создать аккаунт на GitHub
2. Создать локальный репозиторий
3. Подружить локальный и удаленный репозиторий. Github  при создании нового репозитория подскажет как 
    > это можно сделать так **git clone <ссылка на репозиторий в GetHub>** 

    >**cd ..** - позволяет перейти из текущего каталога в каталог на уровень выше

   >**git cd <название подчиненного каталога>**  - позволяет перейти из корневого каталога в текущий
4. Отправить (push) локальный репозиторий в удаленный (на Github), при этом , возможно, нужно будет авторизоваться на удаленном репозитории. 
   > это можно сделать так **git push** 
5. Провести изменение с другого ПК
6. Выкачать (pull) актуальное состояние из удаленного репозитория.