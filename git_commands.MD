## Основные команды для работы с Git  
1. `git version` – проверить версии Git  
2. `git init` – создать Git-репозиторий в папке 
    - `rm -rf .git` – разгитить папку (удалить подпапку .git)
3. `git status` – проверить состояние репозитория
    - `git status --ignored` – проверить состояние репозитория и показать игнорируемые файлы
4. `git add` – подготовить файлы к сохранению (untracked -> staged)
    - `git add --all` – подготовить все файлы к сохранению
    - `git add .` – подготовить всю папку к сохранению
5. `git restore --staged <файл>` – выполнить unstage изменений (staged -> untracked)
    - `git restore --staged .` – выполнить unstage изменений всех файлов в папке
    - `git restore <файл>` – откатить изменения, которые не попали ни в staging, ни в коммит (modified)
6. `git commit -m 'описание коммита'` – сделать коммит
    - `git commit --amend --no-edit` – изменить последний коммит без исправления сообщения
    - `git commit --amend -m 'новое описание коммита'` – изменить последний коммит и исправить сообщение
7. `git reset --hard <хэш коммита>` – откатить изменения к нужному коммиту
8. `git diff` – сравнить последнюю закоммиченную версию файла с той, что находится в состоянии modified
    - `git diff --staged` – показать изменения в staged-файлах относительно последних закоммиченных версий
    - `git diff <хэш коммита 1> <хэш коммита 2>` – сравнить изменения в двух коммитах
    - `git diff <название ветки 1> <название ветки 2>` – сравнить изменения в двух ветках
    - `git diff ~` – суффикс навигации ~N, где N — это число. Он отсчитывает от заданного коммита N коммитов назад во времени (нумерация начинается с нуля)
9. `git log` – посмотреть историю коммитов
    - `git log --oneline` – посмотреть сокращенную историю коммитов
10. `git remote add` – привязать удалённый репозиторий к локальному
    - `git remote -v` – проверить связь репозиториев
11. `git push -u origin main/master` – отправить изменения на удаленный репозиторий в первый раз
    - `git push` – отправить изменения на удаленный репозиторий
12. `git clone <адрес клонируемого репозитория>` – клонировать удаленный репозиторий на локальный компьютер и связать локальный репозиторий с удалённым
13. `git branch` – посмотреть ветки проекта и проверить, в какой ветке находишься
    - `git branch <название ветки>` – создать новую ветку
    - `git branch -D <название ветки>` – удалить ветку
    - `git branch -d <название ветки>` – удалить ветку только если она была полностью объединена с другой
    - `git branch -a` – показать все известные ветки, как локальные, так и удалённые
14. `git checkout <название ветки>` – переключиться на другую ветку
    - `git checkout -b <название ветки>` – создать ветку и сразу переключиться на неё
15. `git merge <название ветки>` – объединить ветки
16. `git pull` – подтянуть изменения из удалённого репозитория