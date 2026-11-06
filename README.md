\# Лабораторная работа №6. Система контроля версий



\*\*Студент:\*\* 4515 Курилкин И.А.

\*\*Цель работы:\*\* изучение базовых возможностей системы управления версиями, опыт работы с Git API, локальным и удалённым репозиторием.



\## Ход работы



\### 1. Fork репозитория

Создана копия репозитория https://github.com/Kurtyanik/LR6/ в личное хранилище.



!\[Fork](screenshots/01\_fork.png)



\### 2. Установка и настройка Git

Git установлен, указаны имя пользователя и email.



!\[Git version](screenshots/02\_version.png)

!\[Git config](screenshots/03\_config.png)



\### 3. Клонирование репозитория

!\[Clone](screenshots/04\_clone.png)



\### 4. Добавление файла через GitHub и git pull

Файл `from\_github.txt` создан через интерфейс GitHub и подтянут в локальный репозиторий.



!\[Git pull](screenshots/06\_pull.png)



\### 5. История веток и последние изменения

!\[История веток](screenshots/07\_log.png)

!\[git show и git diff](screenshots/08\_show\_diff.png)



\### 6. Слияние в master и разрешение конфликта

!\[Конфликт](screenshots/09\_conflict.png)

!\[Файл с маркерами](screenshots/10\_markers.png)

!\[Слияние завершено](screenshots/11\_merge.png)



\### 7. Удаление побочной ветки

!\[Удаление ветки](screenshots/12\_delete\_branc23:02 06.11.2026h.png)



\### 8. Коммиты с комментариями

!\[Коммиты](screenshots/13\_commits.png)



\### 9. Откат коммита

!\[Revert](screenshots/14\_revert.png)



\### 10. Ветка для отчёта

!\[Ветка report](screenshots/15\_report\_branch.png)



\## Лог команд



```bash

git --version

git config --global user.name "4515 Курилкин И.А."

git config --global user.email "kurilkin2007@gmail.com"

git clone https://github.com/BruhManyMan/LR6.git

cd LR6

git status

git pull

git log --oneline

git checkout -b feature

git add conflict.txt

git commit -m "Add conflict.txt in feature branch"

git checkout master

git add conflict.txt

git commit -m "Add conflict.txt in master branch"

git log master --oneline

git log feature --oneline

git log --all --graph --oneline --decorate

git show

git diff master feature

git merge feature

git add conflict.txt

git commit -m "Merge feature into master, resolve conflict"

git branch -d feature

git add file1.txt

git commit -m "Add file1.txt with first line"

git commit -am "Update file1.txt: add second line"

git add notes.txt

git commit -m "Add notes.txt"

git revert HEAD

git checkout -b report

```



\## История операций



f4ac504 2026-11-06 4515 Курилкин И.А. Добавлены ссылки к скриншотам
ad183cc 2026-11-06 4515 Курилкин И.А. Добавление отчёта и скриншотов
5955ada 2026-11-06 4515 Курилкин И.А. Revert "Изменение файла"
12d43e4 2026-11-06 4515 Курилкин И.А. Изменение файла
94668f7 2026-11-06 4515 Курилкин И.А. Добавление первого файла
7a89c76 2026-11-06 4515 Курилкин И.А. Merge feature into master
6e21452 2026-11-06 4515 Курилкин И.А. Изменение файла в ветке feature
d19326d 2026-11-06 4515 Курилкин И.А. Изменение файла в ветке master
7643ce0 2026-11-06 BruhManyMan Add github-file.txt
921f53b 2020-11-21 Kurtyanik Обновление информации
c08a654 2020-11-21 Kurtyanik Файл создан пустым
3c6e913 2020-11-21 Kurtyanik Initial commit

