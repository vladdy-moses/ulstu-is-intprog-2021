# Лабораторная работа №4 - Flexbox (CSS)

## Цель работы

Освоение flexbox в CSS.

## Ход выполнения работы

1. Прочитать справочный материал по flexbox.
2. Реализовать flex-контейнер хотя бы в одном из документов html-документов, выполненных ранее.
3. Заполнить [google-форму](https://docs.google.com/forms/d/e/1FAIpQLSduygNgeE3AQSSN5rLsllKs5wUyBsBrNJ17Rb-a7pqxBYv3sg/viewform?usp=sf_link).

## Понимание flexbox

Flexbox - технология, созданная для упрощения создания макетов html-документов.
Она позволяет гибко настроить ширину, высоту и позицию блоков, что при использовании свойств позиционирования и отступов сделать ранее было либо сложно, либо невозможно.

Для понимния flexbox и возможностей этой технологии ознакомьтесь со статьёй в MDN: <https://developer.mozilla.org/ru/docs/Learn/CSS/CSS_layout/Flexbox>.
Там разбираются основные примеры использования flexbox.

Также для демонстрации работы flexbox можно пользоваться онлайн-сервисами: <http://cssworld.ru/flex/>, <https://flexbox.help/>, <https://basicweb.ru/css/flexbox_generator.php>, <https://flexbox.malven.co/> или любыми другими.

## Добавление flexbox к себе на web-страницы

После понимания того, что есть flexbox и как он может помочь, необходимо найти в своих html-документах место, где использование flex-контейнера было бы полезным, и реализовать там стилизацию блоков при помощи flex-свойств в CSS.

Например, можно при помощи flexbox реализовать отображение карточек на странице со списком, чтобы любое количество карточек растягивалось на всю ширину строки: обычно при размещении строчных элементов они располагаются слева направо сверху вниз, и на последней строке справа остаётся пустое место.
При помощи flexbox можно настроить, чтобы карточки на последней строке растягивались по ширине на одинавую ширину.

Можно основной макет сайта сделать при помощи flex: шапка фиксированной высоты, потом основной контент сайта с `flex-grow`, потом подвал фиксированной высоты.
Основной контент сайта сам может являться контейнером, где в одной строке будет боковое меню фиксированной ширины на всю высоту контента, а затем основной контент также с `flex-grow`.
Также можно боковое меню сделать слева на всю высоту сайта.
В этом случае сначала будет идти контейнер с одной строкой, где слева боковое меню, а далее - контейнер с шапкой, контентом и подвалом.

В случае полного отсутствия идей можно реализовать вёрстку колонок (классы `row` и `col*`) самостоятельно при помощи своих классов и flexbox.

## Сдача лабораторной работы

Необходимо продемонстрировать преподавателю html-разметку с flex-контейнером и css-стилями с настройкой контейнера и дочерних элементов.

В случае дистанционной сдачи работы, заполните [google-форму](https://docs.google.com/forms/d/e/1FAIpQLSduygNgeE3AQSSN5rLsllKs5wUyBsBrNJ17Rb-a7pqxBYv3sg/viewform?usp=sf_link) и напишите в личные сообщения Telegramm преподавателю ФИО, группу и номер работы.
