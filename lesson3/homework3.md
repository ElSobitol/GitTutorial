# Инструкция о командах GIT 
+ git log — вызывать список действий и сохранений
+ git init — создать репозиторий в папке на локальной машине
+ git add — отслеживать добавленные файлы
+ git commit + комментарий — сохранить текущее состояние
+ git diff — показать разницу между версиями
+ git chechout — переключиться между разными версиями
+ git config --global user.name "test user" — устанавливает имя пользователя
+ git config --global user.email "test@test.com" - устанавливает почту пользователя
+ git add fil* - добавляет только определенные файлы
+ git log -p - выводит лог с историей
+ git show `commit id` - выводит историю конкретной записи
+ git commit --amend -m "test comment" - перезаписыват предыдущую запись
+ git checkout -b `branch_name` - создает новую ветку и переключается на нее
+ git branch -d `branch_name` - удаляет локально ветку
+ git push --delete origin `branch_name` - удаляет remote ветку
+ git merge `branch_name` - объединяет с предоставленной веточкой
+ git fetch --all - подтягивает remote веточки
+ git config --global --edit - открывает редактор глобальной конфигурации
+ git log --author=`pattern` - находит записи конкретного автора
+ git reset HEAD~`number` - откатывает без удаления изменений к номеру записи от настоящего