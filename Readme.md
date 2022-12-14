# Инструкция для работы с Git и удалёнными репозиториями

## Что такое Git?
Git - это одна из реализаций распределённых систем контроля версий, имеющая как и локальные, так и удалённые репозитории. Является самой популярной реализацией систем контроля версий в мире.
## Подготовка репозитория
Для создание репозитория необходимо выполнить команду *git init*  в папке с репозиторием и у Вас создаться репозиторий (появится скрытая папка .git)

## Создание коммитов
Чтобы добавить коммит, необходимо прописать команду "git commit -m "Сообщение". Например так: *git commit -m "Добавил команду коммита"*
Также при работе над одним файлом можно использовать команду git commit -am "Сообщение". Эат команда позволяет объединить сразу две команды -add(добавление) и -m(сообщение коммита). Упрощает работу
### Git add
Для добавления измений в коммит используется команда *git add*. Чтобы использовать команду *git add* напишите *git add <имя файла>*

### Просмотр состояния репозитория
Для того, чтобы посмотреть состояние репозитория используется команда *git status*. Для этого необходимо в папке с репозиторием написать *git status*, и Вы увидите были ли измения в файлах, или их не было.

### Создание коммитов
Для того, чтобы создать коммит(сохранение) необходимо выполнить команду *git commit*. Выполняется она так: *git commit -m "<сообщение к коммиту>*. Все файлы для коммита должны быть ***ДОБАВЛЕНЫ*** и сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО***.

## Перемещение между сохранениями
Для того, чтобы перемещаться между коммитами, используется команда *git checkout*. Используется она в папке с пепозиторием следующим образом: *git checkout <номер коммита>*

## Журнал изменений
Для того, чтобы посмтреть все сделанные изменения в репозитории, используется команда *git log*. Для этого достаточно выполнить команду *git log* в папке с репозиторием

## Ветки в Git
Чтобы делегировать работу над файлом нескольким сотрудникам, необходимо для кадого сощдать ветку, в которой он будет работать и назвать соответсвующим действием. Например нам нужно написать полноценную инструкцию по работе с изображениями в GIT, для этого используем комманду git branch images(images - это краткое обозначение того, что мы хотим увидеть в ветке, над которой будет работать другой сотрудник)

Для создания ветки с мгновенным переходом на неё, необходимо использовать команду git checkout -b(от сокращения branch) new name branch

Для перемещения между ветками, необходимо использовать команду git checkout *name_branch*

### Создание ветки
Для создание еще одной ветки, необходимо прописать следующую команду git branch *new_name_branch*
Для того, чтобы создать ветку, используется команда *git branch*. Делается это следующим образом в папке с репозиторием: *git branch <название новой ветки>*

## Слияние веток

Для того чтобы дабавить ветку в текущую ветку используется команда *git merge <name branch>*

## Удаление веток
Для удаления ветки ввести команду "git branch -d 'name branch'"
## Списки
Чтобы добавить ненумерованные списки, необходимо пункты начинать прописывать со знаком (* ). Например:
* Пункт 1
* Пункт 2
* Пункт 3

Чтобы добавить нумерованный список в текст, необходимо прописывать нумерацию с точкой. Например:
1. Первый пункт
2. Второй пункт
3. Третий пункт

## Работа с текстом
Чтобы выделить текст курсивом, необходимо обрамить текст знаком (*) или (_). Например, *вот так* или _вот так_

Чтобы выделить текст жирным, необходимо обрамить текст знаками (**) или (__). Например, **вот так** или __вот так__

## Как работать с изображениями
Чтобы добавить изображение в текстовый файл формата Markdown, необходимо сделать следующее:
![Инструкция по GIT](КомандыGIT.jpg)

