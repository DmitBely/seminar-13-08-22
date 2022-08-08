# Инструкция по работе с Git

## Что  такое Git?
Git - одна из систем контроля версий позволяющая организовать версионность как локально так и на удаленном сервере. Самая популярная платформа реализующая Git это [GitHub](https://github.com)


## Подготовка репозитория
Для создания в папке репозитория необходимо открыть эту папку в терминале и написать команду *git init*, после чего в этой папке создастся скрытая папка .git

## Создание коммитов

### Просмотр состояния репозитория
Для просмотра состояния репозитория используется команда *git status*. В терминале с открытой папкой-репозиторием необходимо написать команду *git status*. В результате можно увидеть следующие выводы:
1. On branch *** nothing to commit - это ознаает нет активных изменений
2. Untracked file - это означает, что имеются файлы неотслеживаемые системой контроля версий
...

### Добавление файла к коммиту
Для того чтобы добавить файл к сохранению, необходимо использовать команду *git add*. В терминале с откртой папкой-репозиторием необходимо написать *git add <название файла>*, и этот файл добавится к сохранению.

### Создание фиксации
Для создания фиксации используется команда *git commit*. Для этого в терминале с папкой-репозиторием необходимо написать команду *git commit -m "сообщение к комиту". Написание сообщения обязательно.

## Журнал изменений
Для просмотра истории изменений используется комманда *git log*. Для этого в терминале с папкой-репозиторием необходимо написать *git log*, и вы увидите список всех коммитов в этой ветке с описанием имени, электронной почты, сообщением к коммиту и номер коммита.

## Перемещение между коммитами
Для перемещения между коммитами используется комманда *git checkout*. Для этого в терминале с папкой-репозиторием необходимо написать *git checkout <номер комита>. Номер комита берётся из журнала изменений ветки.

## Ветки в git

## Слияние веток и решение конфликтов

## Удаление веток

