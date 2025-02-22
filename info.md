# Инструкция для работы с Git + инструкция для работы с Markdown

## инструкция по git

* git --version - показывает текущею версию git
* git init - инициализация локального репозитория
* git status - получить информацию от git о его текущем состоянии
* git add info.md - добавляет отслеживание файла info.md
* git add . - добавляет отслеживание всех файлов в диретории
* git commit -m "Коментарий" - фиксация состояния изменений
* git log - вывод на экран истории всех коммитов с их хеш-кодом
* git log --graph - визуализация всех веток в виде древа
* git checkout - переход от одного комита к другому
* git checkout master - переход к актуальному состоянию файла
* git diff - увидеть разницу между актуальным файлом и последним комитом
* git branch <имя ветки> - создает новую ветку/черновик
* git branch -d <имя ветки> - удаление ветки
* git merge <имя ветки> - делает слияние ветки с текущей
* git clone <url-адрес реепозитория> - клонирование внешнего репозитория на локальный ПК
* git pull - выкачивает данные из удаленного репозитория и делает слияние (merge) с локальным репозиторием
* git push - отправляет свою версию репозитория во внешний

# Инструкция для работы с Markdown

## Работа с заголовками
Чтобы выделить текст в заголовок, необходимо перед началом заголовка постовить знак (#), заголовки могут быть разных размеров. Например:
# Заголовок 1
## Заголовок 2
### Заголовок 3
#### Заголовок 4
##### Заголовок 5
###### Заголовок 6

## Акцепты или выделение текста

Чтобы выделить текст курсивом необходимо обромить его звездочкам (*) или знаком нижнего подчеркивания (_). Например, *вот так* или _вот так_.

Чтобы выделить текст полужирным, необходимо обрамить его двойными звездочками (**) или двойным знаком нижнего подчеркивания (__). Например, **вот так** или __вот так__.

Альтернативные способы выделения текста жирным или курсивом для того, чтобы мы могли совмещать оба этих способа. Например, _текст может быть выделен курсивом и при этом быть **жирным**_.

## Списки

Чтобы добавить ненумерованные списки, небходимо пунты выделить звездочкой (*) или знаком (+).
* Элемент 1
* Элемент 2
+ Элемент 3
+ Элемент 4

Чтобы добавить нумерованные списки, необходимо просто пронумеровать . Например, вот так:
1. Первый пункт
2. Второй пункт 

## Цитаты

Чтобы выделить цитату, необходимо впереди начала цитаты постовить знак(>) или использовать знак на каждой строчке, где начинается начало цитаты. Можно совмещать с другими элементами. Напимер:
> Цитата 1

>Цитата 2

> Цитата в цитате
>> Цитата в цитате

> ## Цитата с совмещение других элементов
> - Добовление списков
> 1. Списки пронумерованные
> 2. С *использованием* **акцептов**

## Работа с изображениями

Чтобы вставить изображение в текст, достаточно написать следующее:
![Привет, это печеньки!](mini_magick20221215-162-3rxh0d.png)

## Ссылки
Чтобы вставить ссылку, достаточно написать например следующие: Ссылка на сайт [GeekBrains](https://gb.ru/)
Ссылки можно совмещать с другими элементами: _**[GeekBrains](https://gb.ru/)**_

## Работа с таблицами

Несколько примеров создания таблицы
| |**Столбец А**|**Столбец Б**|
|----|----|----|
|*Строка 1*|*Ячейка 1А*|*Ячейка 2А*|
|_**Строка 2**_|_**Ячейка 1Б**_|_**Ячейка 2Б**_|

***
git 
>|Столбец 0|Столбец 1|Столбец 2|Столбец 3|
>|----|----|----|----|
>|Строка A|Ячейка A1|Ячейка A2|Ячейка A3|
>|Строка B|Ячейка B1|Ячейка B2|Ячейка B3|
>|Строка C|Ячейка C1|Ячейка C2|Ячейка C3|

# pull request
* команда для предложения изменений 
* запрос на вливание изменений в репозиторий
> В больших компаниях один ответственный за проект создает аккаунт. Другие пользователи дают
команду pull request. Предлагать изменения на GitHub нужно в отдельной ветке. Сначала
пользователь копирует репозиторий на свой компьютер, делает fork репозитория, затем
клонирует версию на своём ПК, создаёт ветку с предлагаемыми изменениями, отправляет
изменения командой push в свой аккаунт на GitHub и даёт команду pull request. 

## Как сделать pull request
1. Делаем **fork** (ответвление) репозитория
2. Делаем git clone **своей** версии репозитория
3. Создаем новую ветку и в НЕЕ вносим свои изменения
4. Фиксируем изменения (делаем коммиты)
5. Отправляем свою версию в свой GitHub
6. На сайте GitHub нажимаем кнопку **pull request**