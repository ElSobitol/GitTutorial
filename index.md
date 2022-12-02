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
# Туториал по языку разметки MarkDown

## Как добавить заголовки

**Абзацы создаются при помощи пустой строки. Если вокруг текста
сверху и снизу есть пустые строки, то текст превращается в абзац.**

**Чтобы сделать перенос строки вместо абзаца,
нужно поставить два пробела в конце предыдущей строки.**

**Заголовки отмечаются диезом # в начале строки, от одного до шести. Например:**

## Как добавить таблицы

В чистом Маркдауне нет синтаксиса для таблиц, а в GFM
есть.
First Header | Second Header
------------- | -------------
Content Cell | Content Cell
Content Cell | Content Cell

Можно управлять выравниванием столбцов при помощи
двоеточия.
| Left-Aligned | Center Aligned | Right Aligned |
|:------------- |:---------------:| -------------:|
| col 3 is | some wordy text | **$1600** |
| col 2 is | centered | $12 |
| zebra stripes | are neat | ~~$1~~ |

## Использование HTML внутри Markdown

У лукоморья дуб зеленый...
Mожно смешивать Markdown и HTML. Если на какие-то
элементы нужно поставить классы или атрибуты, смело
используем HTML:
> Выделять слова можно при помощи * и _ . Например, это
<em class="a1">italic</em> и это тоже <i
class="a1">italic</i>. А вот так уже <b>strong</b>, и
так тоже <strong>strong</strong>.
Можно и наоборот, внутри HTML-тегов использовать
Маркдаун.
<section class="someclass">

### Пример Маркдауна внутри HTML

Выделять слова можно при помощи `*` и `_` . Например,
это _italic_ и это тоже *italic*. А вот так уже
__strong__, и так тоже **strong**.
</section>

## Цитаты

Dont worry be happy tuuuuu rutuuu tutu rututu tutu dont worry
## Цитаты

Цитаты оформляются как в емейлах, с помощью символа `>`.

> This is a blockquote with two paragraphs. Lorem ipsum
dolor sit amet,
> consectetuer adipiscing elit. Aliquam hendrerit mi
posuere lectus.
> Vestibulum enim wisi, viverra nec, fringilla in,
laoreet vitae, risus.
>
> Donec sit amet nisl. Aliquam semper ipsum sit amet
velit. Suspendisse
> id sem consectetuer libero luctus adipiscing.

Или более ленивым способом, когда знак `>` ставится
перед каждым элементом цитаты, будь то абзац, заголовок
или пустая строка:

> This is a blockquote with two paragraphs. Lorem ipsum
dolor sit amet,
consectetuer adipiscing elit. Aliquam hendrerit mi
posuere lectus.
Vestibulum enim wisi, viverra nec, fringilla in, laoreet
vitae, risus.
>
> Donec sit amet nisl. Aliquam semper ipsum sit amet
velit. Suspendisse
id sem consectetuer libero luctus adipiscing.
В цитаты можно помещать всё что угодно, в том числе
вложенные цитаты:
> ## This is a header.
>
> 1. This is the first list item.
> 2. This is the second list item.
>
> > Вложенная цитата.
>
> Here's some example code:
>
> return shell_exec("echo $input |
$markdown_script");
