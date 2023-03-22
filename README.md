# Инструкция по работе с **Git**

## 1. git config - *задать имя пользователя и адрес электронной почты*

```GIT
git config --global user.name "Tara Routray"
git config --global user.email "dev@tararoutray.com"
```

## 2. git init - *инициализировать репозиторий Git*

```GIT
git init
```

## 3. git add somefile.js - *Добавление отдельных файлов или всех файлов в область подготовленных файлов*

```GIT
git add somefile.js
```

## 4. git status - *Проверка статуса репозитория*

```GIT
git status
```

## 5. git commit -m - *Внесение изменений однострочным сообщением или через редактор*

```GIT
git commit -m "Your short summary about the commit"
```

## 6. git log - *Просмотр истории коммитов с изменениями*

```GIT
git log -p
```

## 7. git diff - *Просмотр изменений до коммита*

```GIT

```

## 8. git switch - *переключаться*

```GIT
git switch branch_name
```

## 9. git commit --amend -m- *Изменение последнего коммита*

```GIT
git commit --amend -m "Updated message for the previous commit" 
```

## 10. git branch new_branch_name - *Создать новую ветку можно с помощью параметра branch , указав имя ветки*

```GIT
git branch new_branch_name
```

## 11. git checkout -b new_branch_name - *Для автоматического перехода нужно добавить флаг -b и параметр checkout*

```GIT
git checkout -b new_branch_name 
```

## 12. git branch - *Можно просматривать полный список веток, используя параметр branch*

```GIT
git branch
```

## 13. git branch -d existing_branch_name - *Удалить ветку можно параметром branch с добавлением флага -d и указанием имени ветки*

```GIT
git branch -d existing_branch_name
```

## 14. git branch -D existing_branch_name - *Для принудительного удаления ветки используется флаг -D с заглавной буквой. В этом случае ветка будет удалена независимо от текущего статуса, без предупреждений*

```GIT
git branch -D existing_branch_name
```

## 15. git merge existing_branch_name - *Объединить две ветки можно параметром merge с указанием имени ветки. Команда объединит указанную ветку с основной*

```GIT
git merge existing_branch_name
```

## 16. git log --graph --oneline --decorate - *Отображение журнала фиксации в виде графика для текущей или всех веток*

```GIT
git log --graph --oneline --decorate
```

## 17. git remote -v - *Просматривать удалённые URL-адреса можно параметром remote с флагом -v . Этот параметр отображает удалённые подключения к другим репозиториям*

```GIT
git remote -v
```

## 18. git push origin main - *Отправлять изменения в удалённый репозиторий можно параметром push с указанием имени репозитория и ветки*

```GIT
git push origin main
```

## 19. git pull - *Для загрузки изменений из удалённого репозитория используется параметр pull . Он скачивает копию текущей ветки с указанного удалённого репозитория и объединяет её с локальной копией*

```GIT
git pull
```

## 20. git push - *Отправка новой ветки в удалённый репозиторий*

```GIT
git push
```
