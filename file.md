# Git tutorial

## Восстановление изменений

*Восстановить в рабочей директории указанный файл на момент указанного коммита (и добавить это изменение в индекс)*

```
git reset index.html для удаления из индекса, но сохранения изменений в файле

git checkout 5589877 index.html 

```

## Кто написал строку

*Показать строки 5-8 указанного файла и коммиты, в которых строки были добавлены*

```
git blame README.md --date=short -L 5,8 
```

## Клонирование репозитория

*Клонировать удаленный репозиторий в одноименную директорию*

```
git clone https://github.com/cyberspacedk/Git-commands.git    
```

*Клонировать удаленный репозиторий в директорию «FolderName»*

```
git clone https://github.com/cyberspacedk/Git-commands.git FolderName 
```


*Клонировать репозиторий в текущую директорию*

```
git clone https://github.com:nicothin/web-design.git .  
```