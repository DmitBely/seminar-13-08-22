# Инструкция по работе с Git

## Что  такое Git?
Git - одна из множества систем контроля версий позволяющая организовать версионность как локально так и на удаленном сервере. Самая популярная платформа реализующая Git это [GitHub](https://github.com)


## Подготовка репозитория
Для создания в папке репозитория необходимо открыть эту папку в терминале и написать команду *git init*, после чего в этой папке создастся скрытая папка .git

## Создание коммитов

### Просмотр состояния репозитория
Для просмотра состояния репозитория используется команда *git status*. В терминале с открытой папкой-репозиторием необходимо написать команду *git status*. В результате можно увидеть следующие выводы:
1. On branch *** nothing to commit - это ознаает нет активных изменений
2. Untracked file - это означает, что имеются файлы неотслеживаемые системой контроля версий
3. Changes not staged to commit - значает, что файл не отслеживается и возможно попал в *.gitignore*

### Добавление файла к коммиту
Для того чтобы добавить файл к сохранению, необходимо использовать команду *git add*. В терминале с откртой папкой-репозиторием необходимо написать *git add <название файла>*, и этот файл добавится к сохранению.

## Журнал изменений
Для просмотра истории изменений используется комманда *git log*. Для этого в терминале с папкой-репозиторием необходимо написать *git log*, и вы увидите список всех коммитов в этой ветке с описанием имени, электронной почты, сообщением к коммиту и номер коммита.

### Создание фиксации
Для создания фиксации применяется команда *git commit*. Для этого в терминале с папкой-репозиторием необходимо написать команду *git commit -m "сообщение к комиту". Написание сообщения обязательно.



## Перемещение между коммитами
Для перемещения между коммитами используется комманда *git checkout*. Для этого в терминале с папкой-репозиторием необходимо написать *git checkout <номер комита>. Номер комита берётся из журнала изменений веток.

## .gitignore файл
В данный файл мы добавляем названия файлов и их расширений в каждой строке, во избежание их дальнейшего попадания в гит. как правило эти файлы не относятся к коду программы или не нужны в конкретном моменте программирования.

## Ветки в git
Для создания ветвления от определённой ветки используется команда *git branch*. Для этого необходимо перейти в ветку из которой планируется ветвление и написать в консоли *git branch имя создаваемой ветки*

## Преобразование вветок
Для добавления ветвления целиком, используется команда *rebase*. Для её использования нужно перейти в ветку в которую планируется перенос командой *checkout*, затем в консоли нужно прописать команду *git rebase имя_ветки_которую_переносим* 

## Слияние веток и решение конфликтов
Для слияния веток необходимо использовать команду *merge*. Для этого в терминале необходимо перейти в ветку в которую будут сливатьс изменения внесённе в другие ветки. После чего написать *git merge имя_ветки_из_которой_забираем изменения* 

## Удаление веток
Для удаления веток используется команда *branch -d имя_удаляемой_ветки*. Для того чтобы удалить ветку небходимо прописать её из комита из которой она ветвится. Удаление ветки это необратимй процесс.
