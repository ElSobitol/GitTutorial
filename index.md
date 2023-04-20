# Туториал по работе с Git

## Начало работы

Для начала работы, необходимо инициализировать сам Git

Для его инициализации введите команду 

```
  git init
```

## Добавление файла

Для добавления файла в Git необходимо воспользоваться командой 

```
git add название файла
```
# Работа с удаленным реппозиторием
#

Для работы с remote reppo в идеале нужен SSH-key
## Создание SSH-key
1. GitHub - settings - SSH and GPG keys - add ssh-key
2. На ПК: `VSC - add folder (.ssh-key-main)`
3. переходим в эту папку
4. Запускаем ssh-keygen -o
5. после адреса папки прописываем: .\id.rsa
6. заходим в папку - открываем файл id.pub - копируем
7. GitHub: вставляем данные в поле 2
8. Активируем ключ: `eval "$(ssh-agent -s)"`
`ssh-add /c/Users/Alina/Desktop/.ssh-main/id.rsa`
9. Проверка: `ssh-add -1 -E sha256`
10. `git push -u origin main`

#
## Создаем реппозиторий на GitHub:
1. profile - your reppo - new
2. VSC: называем основную папку main: `git branch -M main`
3. Проверить все уд. соединения: `git remote -v`
4. проверить все remote rep:
`git remote add origin`
5. `git push -u origin main` потом можно git push
#
## Remote work with Fork
1. Заходим в чужой реппозиторий - делаем себе копию (FORK)
2. Создается копия оригинала - заходим в него - копируем ssh
3. VSC: создаем папку проекта - подвязываем ключ:

`eval "$(ssh-agent -s)"`

`ssh-add /c/Users/Alina/Desktop/.ssh-main/id.rsa`

4. git clone (указываем адрес SSH нашей копии!)
5. Работаем с файлами: создаем новую ветку

git switch -c nb
touch readme.md
6. коммитим
7. push (SSH-addres) + название новой ветки (nb)
8. GitHub: compare - ... - create request (появится в pull-request)

## Work without Fork
#
1. Заходим в origin реппозитория - копируем адрес
2. VSC: открываем новый терминал (выполняем привязку реппозитория как отдельного пользователя)

`git remote -v`

`git remote add Edy888 (addres)` удаленно добавили пользователя на аккаунт

`git remote -v`

## Из инструкции (no fork)
#
1. VSC: `git clone`
2. создаем внутри папки новую ветку
3. коммитим
4. связываем: `git remote add upstream https: ..... username`
5. Получить последние изменения: `git fetch upstream`
6. Обновить ветку новыми изменениями из основной ветки: `git rebase upstream/mean`
7. Загрузить ветку в удаленный реппозиторий: `git push -u origin nb`
8. GIT: создать pull-request на основе моей ветки
9. теперь владелец видит мою ветку и сможет принять изменения при желании.