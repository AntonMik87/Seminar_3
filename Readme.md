# Инструкция по работе с Git и по работе с ветками

## Что такое git?
---
Git это - одна из реализаций распределенных систем контроля версий. Что позволяет иметь версионность как в локальном репозитории. Так и в удаленном репозитории (общее для всех). Git является на данный момент самой популярной системой контроля версий.
## Подготовка репозитория
--- 
Для создания репозитория используется команда *git init*. В терминале в папке с будущим репозиторием достаточно написать *git init*, и эта папка станет репозиторием.

## Создание коммитов
---
Для создания commit в Markdown необходимо создать файл в папке с проектом и присвоить ему "разрешение" понятное для программы. Например, файл - Readme.md
Когда файл создан, мы можем вносить в него данные с клавиатуры. Это будет наш рабочий каталог. Чтобы сохранить данные, в начеле необходимо добавить содержимое нашего рабочего каталога в так называемый индекс - это черновик коммита, для этого используется команда *git add*. Только файлы из индекса попадут в коммит. После добавления в индекс мы можем создать коммит. Выполнив команду *git commit*


## Просмотр состояния репозитория
---
Для того чтобы просмотреть состояние репозитория в git, существует команда *git status*. Она отображает состояние рабочего каталога и радела проиндексированных файлов. С ее помощью можно проверить индексацию изменений и увидеть файлы, которые не отслеживаются Git.

## Добавление файла в коммит
---
Для добавления файла в текущей коммит используется команда *git add*. Для этого достаточно в терминале с папкой текущего репозитория написать *git add <название файла>*

### Сохранение коммита
---
Для сохранения коммита используется команда *git commit*. Для этого в терминале с папкой репозитория необходимо написать команду *git commit -m "<сообщение к коммиту>"*. Сообщение к коммиту писать ***Обязательно***

## Журнал изменений
---
Для просмотра истории коммитов, то есть истории наших изменений используется команда *git log*. Для этого необходимо в терминале с папкой-репозиторием написать *git log*


## git log Перемещение между коммитами
---
Для того чтобы перемещаться между коммитами необходимо использовать *git checkout*. Для этого в терминале с папкой репозитория необходимо написать *git checkout <номер коммита>* Номер коммита берется из истории. После такого "перемещения" мы попадаем в состояние *Detached head*. Для возвращения в обычное состояние используется команда *git checkout master*.

## Ветки в Git
___
Ветка - это последовательность коммитов, представляют собой указатель на снимок изменений. Если нужно добавить новую возможность или исправить что-то, создаем новую ветку, в которой будут размещаться эти изменения. Для того чтобы создать ветку используется команда *git branch <название ветки.>* Для переключения между ветками пользуемся командой *git checkout <название ветки>

## Слияние веток и решение кофликтов
___
Слияние веток в Git делается для объединения ответвлений-черновиков с головным файлом и производится по средством команды *git merge <название ветки.>* Так же не редко при объединении возникают конфликты, которые необходимо разрешить. Git может предложить ряд вариантов разрешения конфликта:

1. **Accept Current Cuhange** (принять текущую версию)
2. **Accept Incoming Change** (принять входящую версию)
3. **Accept Both Changes** (принять обе версии)
4. Или же решить конфликт вручную.

## Удаление веток
---
Когда мы завершили работу с веткой и слили ее с основной, эту ветку можно будет удалить без потери истории. Для этого необходимо в терминале воспользоваться командой *git branch -d <название ветки>. После этого ветка будет удалена, в чем можно будет убедиться с помощью команды *git branch*.
