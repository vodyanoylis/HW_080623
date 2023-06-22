# Конспект по Git
***
## Что это такое и с чем его едят
***
*Git* - это консольная утилита, для отслеживания и ведения истории изменения файлов в вашем проекте. 

С помощью Git-a можно откатить проект до более старой версии, сравнивать, анализировать или сливать свои изменения в репозиторий.

*Репозиторием* называют хранилище вашего кода и историю его изменений. Все репозитории хранятся в определенных папках на жестком диске.

Каждая точка сохранения проекта носит название *коммит* (commit). У каждого commit-a есть hash (уникальный id) и комментарий. Из таких commit-ов собирается ветка. Ветка - это история изменений. У каждой ветки есть свое название. Репозиторий может содержать в себе несколько веток, которые создаются из других веток или вливаются в них.
***
## Команды
***
### Работа с локальным репозиторием
***
**Создание локального репозитория:**
- git init

**Добавление файла:**
- git add "filename"

**Сохранение изменений в репозитории:**
- git commit -m "message"

**Посмотреть список веток:**
- git branch

**Создать новую ветку:**
- git branch branch_name

**Переключиться между ветками:**
- git checkout branch_name

**Узнать статус текущего состояния файлов в папке:**
- git status

**Посмотреть список коммитов:**
- git log
    - --graph _позволяет визуализировать ветки_

**Слить ветку в текущую:**
- git merge branch_name

**Посмотреть различия файлов:**
- git diff

**Удалить ветку:**
- git branch -d branch_name

***
### Работа с удалённым репозиторием
***
**Клонирование удалённого репозитория:**
- git clone "adress"

**Соединение с удалённым репозиторием:**
- git remote add name https://github.com/username/repo-name.git

**Выгрузка в удалённый репозиторий:**
- git push -u name branch_name

**Сохранение изменений из удалённого репозитория:**
- git fetch

**Загрузить историю из удалённого репозитория и объединить с локальной:**
- git pull