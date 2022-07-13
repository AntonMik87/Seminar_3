# Инструкция по работе с Git и по работе с ветками

## Что такое git?
---
Git это - одна из реализаций распределенных систем контроля версий. Что позволяет иметь версионность как в локальном репозитории. Так и в удаленном репозитории (общее для всех). Git является на данный момент самой популярной системой контроля версий.

## Подготовка репозитория
--- 
Для создания репозитория используется команда *git init*. В терминале в папке с будущим репозиторием достаточно написать *git init*, и эта папка станет репозиторием.

## Создание коммитов

### просмотр состояния репозитория
текст про гит статус

### Добавление файла в коммит
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

## Гит ветки добавить инфу
___
Ветка - это последовательность коммитов, представляют собой указатель на снимок изменений. Если нужно добавить новую возможность или исправить что-то, создаем новую ветку, в которой будут размещаться эти изменения. Для того чтобы создать ветку используется команда *git branch <название ветки.>* Для переключения между ветками пользуемся командой *git checkout <название ветки>

## Слияние веток и решение кофликтов

## Удаление веток

