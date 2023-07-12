# Основные правила Markdown

![HD-wallpaper-ghibli-a·-github-topics-a·-github-cute-ghibli](https://github.com/MelikovGraf/GIT/assets/98654937/6cf897c3-7e6b-48b3-9220-128cf8b2c893)

Заголовки и горизонтальные линии
Заголовки H1–H6 выделяются в Markdown с помощью знаков решетки (диез/шарп). Можно просто поставить нужное количество решеток в начале строки, чтобы указать уровень. Или заключить строку с двух сторон по аналогии с HTML-тегами, кому как удобно.

# Это H1

## Это H2 ##

### Это H3

#### Это H4 ####

##### Это H5 #####

###### Это H6

Другой вариант: написать текст первого заголовка, затем нажать Enter и на следующей строке указать любое количество знаков «равно». Аналогичным образом можно выделить H2, только использовать уже нужно дефисы. Заголовки других уровней таким методом оформить нельзя.

# Выделения текста
Форматирование курсивом и жирным точно есть во всех инструментах, где другие функции Markdown могут быть ограничены. Синтаксис выделения текста и расставления акцентов:

__Жирный__

**Тоже жирный**

*Курсив*

_Тоже курсив_

~~Зачеркнутый~~ (~~)

Можно легко комбинировать эти способы выделения.

Списки и отступы
Чтобы оформить строку в элемент маркированного списка, в начале нужно поставить плюс, минус или звездочку. Звездочка не приведет к курсивному выделению, потому что отделяется от слова пробелом.

- Пункт 1

- Пункт 2

- Пункт 3

или

+ Пункт 1

+ Пункт 2

+ Пункт 3

или

* Пункт 1

* Пункт 2

* Пункт 3


Если необходимо создать нумерованный список, используйте в начале строки цифру с точкой. Удобно, что нумерация автоматическая: можно вставить любые цифры, и ошибки не будет.

1. Пункт 1

2. Пункт 2

3. Пункт 3

или

1. Пункт 1

1. Пункт 2

1. Пункт 3

или даже

9. Пункт 1

5. Пункт 2

1. Пункт 3

Маркдаун-разметка также позволяет оформлять многоуровневые списки. Уровень обозначается не количеством спецсимволов, как в случае с заголовками, а за счет отступов. Проще не считать пробелы, а каждый новый подпункт выделять табуляцией.

- Пункт 1

        - Подпункт A

                - Подподпункт a

- Пункт 2

        + Подпункт A

                * Подподпункт a

---

1. Пункт 1

        + Подпункт A

                - Подподпункт a

2. Пункт 2

        1. Подпункт 2.1.

                1. Подподпункт 2.1.1

3. Пункт 3

Если пункт списка включает несколько строк или абзацев, нужно соблюдать всё те же отступы, чтобы было красиво оформлено. Ключевые мысли в списках также можно выделять другой разметкой, например, жирным. Примеры:

* __Тезис №1__

    Раскрываем тезис.

* __Тезис №2__

    Раскрываем тезис.

---

* __Тезис №1__ Раскрываем тезис.

* __Тезис №2__ Раскрываем тезис.

Ссылки и картинки
Чтобы поставить гиперссылку без анкора, нужно взять URL в угловые скобки. С e-mail – аналогично.

Если вставлять с анкором, то тогда текст ссылки заключается в квадратные скобки, а адрес страницы – в круглые. Рядом с URL можно прописать тайтл, его объявляют в кавычках (он тоже остается внутри круглых скобок).

Это [Наша ссылка](https://mysite.ru "Ваш сайт") с тайтлом.

[ссылка](https://mysite.ru) без заголовка.

<https://mysite.ru/&gt; – а это безанкорная ссылка.


Цитаты и вставки кода
Если безанкорные ссылки оформляются двумя угловыми скобками, то для цитаты нужна только одна такая скобка. Все очень просто:

> Привет! Это цитата

> Это тоже цитата

> Это еще одна цитата

Это ее продолжение (показываем отступом)

> Это тоже

Будет

>

> Одна целая цитата

Кстати, о коде. Вставлять его можно как внутрь строк, так и отдельными блоками. Для соответствующей разметки используют грависы или обратные тики. Инлайн-код выделяют одиночными символами, а блоки – тройными. При оформлении целого блока можно указать язык программирования, чтобы подсветить соответствующий синтаксис. Примеры:

Просто инлайн-код: `print("Hello, World!")`

Код на Python:

```python

x = int(input())

if x > 0:

    print(x)

else:

    print(-x)

```

Код на JavaScript:

```javascript

let greeting1 = 'Father!';

console.log(greeting1);

let greeting2 = 'Mother!';

console.log(greeting2);

```


Таблицы и чек-боксы
Если поддерживается расширенная версия Markdown, можно вставлять таблицы. Для этого используются всего два символа: вертикальная черта и дефис. Дефисы работают примерно так же, как в случае с горизонтальной линией: отделяют заголовки от других строк, при этом количество символов значения не имеет. Вертикальная черта служит границей между столбцами.

Пример – таблица меток для блоков кода, об этом было в предыдущем разделе:

| Язык | Метка |

| -----|------|

| Java Script | javascript |

| C++ |cpp|

| HTML|html|

|Markdown|md|

|JSON|json|

|Python|python|

|SQL|sql|
