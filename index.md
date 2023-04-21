# Сoздание туториала по GIT

Ссылка на [Справочные материалы по Markdown](https://learn.microsoft.com/ru-ru/contribute/how-to-write-links)



1. Чтобы изменить комментарий/фиксацию/commit: **git commit --amend -m "new commit"** (при этом запись о первом коммите остается и ее можно увидеть через комманду **git reflog**)

2. **git stash** - отменяет последние изменения, но если они не зафиксированны

## Как создать локальный репозиторий

```fix
git init
```

## Как добавить файл на отслеживание:

```fix
git add .
```

## Возврат к определенной фиксации, которая будет считаться нулевой *(через git log будет прослеживаться новая ветка коммитов, а через git reflog видна абсолютно вся история фиксаций)*

```fix
git reset commit_number

git reset --soft commit_number

gir reset --hard commit_number
```

## Переключение между коммитами:

```fix
git checkout commit_number
```
*Так последующие изменения файла пойдут по ветке выбранного коммита, то есть c момента определенного/нужного коммита*

*Для возврата к главной ветке (master):*

```fix
git checkout master
```

Удалить файл:

```fix
git rm <имя файла>
```
Удалить папку:

```fix
git rm -r <имя_папки>
```

## Ошибка в имени ветки <branch> - исправляем

```fix
git branch <wrong_name>

git branch -m <wrong_name> <wright_name>
```
## Показ ветвления

```fix
git log --graph
```

# Руководство по Markdown





## Раздел 1 - Заголовки

Заголовки отмечаются диезом `#` в начале строки, от одного до шести. Например: 

# Заголовок первого уровня # 
## Заголовок h2 
### Заголовок h3 
#### Заголовок h4
##### Заголовок h5 
###### Заголовок h6 

В декоративных целях заголовки можно «закрывать» с обратной стороны.







## Раздел 2 - Списки

Для разметки неупорядоченных списков можно использовать или `*`, или `-`, или `+`:

- элемент 1
- элемент 2
- элемент ... 

Вложенные пункты создаются четырьмя пробелами перед маркером пункта: 
* элемент 1 
* элемент 2    
    * вложенный элемент 2.1    
    * вложенный элемент 2.2 
* элемент ... 

Упорядоченный список: 

1. элемент 1 
2. элемент 2    
    1. вложенный    
    2. вложенный 
3. элемент 3

4. Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse id sem consectetuer libero luctus adipiscing. 

На самом деле не важно как в коде пронумерованы пункты, главное, чтобы перед элементом списка стояла цифра (любая) с точкой. 

Можно сделать и так: 
0. элемент 1 
0. элемент 2 
0. элемент 3 
0. элемент 4 

Список с абзацами: 

* Раз абзац. Lorem ipsum dolor sit amet, consectetur adipisicing elit. 

* Два абзац. Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse id sem consectetuer libero luctus adipiscing. 

* Три абзац. Ea, quis, alias nobis porro quos laborum minus sed fuga odio dolore natus quas cum enim necessitatibus magni provident non saepe sequi?  
  
    Четыре абзац (Четыре пробела в начале или один tab).










## Раздел 3 - Исходный код

В чистом Маркдауне блоки кода отбиваются 4 пробелами в начале каждой строки. 

Но в GitHub-Flavored Markdown (сокращенно GFM) есть более удобный способ: ставим по три апострофа (на букве Ё) до и после кода. Также можно указать язык исходного кода. 

```html 
<nav class="nav nav-primary">  
    <ul>    
        <li class="tab-conversation active">      
            <a href="#" data-role="post-count" 
class="publisher-nav-color" data-nav="conversation">        
            <span class="comment-count">0 комментариев</span>
            <span class="comment-countplaceholder">Комментарии</span>
        </a>    
    </li>    
    <li class="dropdown user-menu" data-role="logout">      
        <a href="#" class="dropdown-toggle" datatoggle="dropdown">
            <span class="dropdown-toggle-wrapper">         
                 <span>            
                    Войти          
                </span>        
            </span>        
            <span class="caret"></span>      
        </a>    
    </li>  
    </ul> 
    </nav> 
    ```
```




## Раздел 4 - Таблицы


В чистом Маркдауне нет синтаксиса для таблиц, а в GFM есть. 

First Header  | Second Header
------------- | ------------
Content Cell  | Content Cell
Content Cell  | Content Cell 

Для красоты можно и по бокам линии нарисовать:

| First Header  | Second Header | 
| ------------- | ------------- | 
| Content Cell  | Content Cell  | 
| Content Cell  | Content Cell  | 

Можно управлять выравниванием столбцов при помощи двоеточия. 
| Left-Aligned  | Center Aligned  | Right Aligned | 
|:------------- |:---------------:| -------------:| 
| col 3 is      | some wordy text |     **$1600** |
| col 2 is      | centered        |         $12   |
| zebra stripes | are neat        |        ~~$1~~ |

 Внутри таблиц можно использовать ссылки, наклонный, жирный или зачеркнутый текст. Для всего остального есть обычный HTML.




 ## Раздел 5 - Создание конфликта

 dsjfh.hf.dfkhdfkjhldfkjhdfljhv

 rejghkjfhglkhklhlkerhjl

 rlghekrhglkerhjlkerj
 
 elrgherhgejrkhgkejhrgkejrhgke

 # Семинар 3

## Работа с GitHub (GH)

### Подключение удаленного репозитория(УР) к GH

1 -  копируем из GH и вставляем в терминал УР
```fix 
git branch -M main
```

2 - в УР проверка привязки
```fix
git remote -v
```

3 - если нет привязки, происходит просто переход на следующую строку, после чего копируем из GH
```fix
git remote add origin https://github.com/1techspec1/first_repository.git
```

и прописываем в терминале УР. 

*Вместо ***origin*** можно прописать никнейм пользователя, которому нужно дать доступ*

4 - копируем из GH и вставляем в терминал УР
```fix
git push -u origin main
```


# Работа с удаленным репозиторием GitHub

## Работа со сторонним проектом через GitHub *(как подключиться к работе с чужим проектом):*

1. Делаем (fork) интересующего нас репозитория
2. Делаем (git clone) для нашей версии этого репозитория
    - переключиться на скопированную папку командой **(cd <имя клонированной папки>)**
3. создаем ветку с предлагаемыми изменениями (git branch <имя_ветки>)
4. Создаем папку README.md с клонированного описанием проекта
5. Производим все изменения только в этой ветке
6. Отправляем эти изменения на свой аккаунт **(git push или git push --set-upstream origin description, если не все настроенно)**
7. В окне GH появляется возможность отправить **pull request** с моими изменениями автору проекта (владельцу репозитория, с которого сделал fork), а также появилась новая ветка
 
*После нажатия кнопки **(pull request)** написать владельцу сообщение типа - "Хотел бы поучаствовать в вашем проекте"*


Добавил этот текст для коммита