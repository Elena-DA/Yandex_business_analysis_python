# Анализ бизнес-показателей приложения Procrastinate Pro+.

Вы — маркетинговый аналитик развлекательного приложения Procrastinate Pro+. Несмотря на огромные вложения в рекламу, последние несколько месяцев компания терпит убытки. Ваша задача — разобраться в причинах и помочь компании выйти в плюс.
    
Есть данные о пользователях, привлечённых с 1 мая по 27 октября 2019 года:
    
- лог сервера с данными об их посещениях,
- выгрузка их покупок за этот период,
- рекламные расходы.

---
    
**Описание данных**

В вашем распоряжении три датасета. Файл `visits_info_short.csv` хранит лог сервера с информацией о посещениях сайта, `orders_info_short.csv` — информацию о заказах, а `costs_info_short.csv` — информацию о расходах на рекламу.
    
Структура `visits_info_short.csv`:
    
- `User Id` — уникальный идентификатор пользователя,
- `Region` — страна пользователя,
- `Device` — тип устройства пользователя,
- `Channel` — идентификатор источника перехода,
- `Session Start` — дата и время начала сессии,
- `Session End` — дата и время окончания сессии.
    
Структура `orders_info_short.csv`:
    
- `User Id` — уникальный идентификатор пользователя,
- `Event Dt` — дата и время покупки,
- `Revenue` — сумма заказа.
    
Структура `costs_info_short.csv`:
    
- `dt` — дата проведения рекламной кампании,
- `Channel` — идентификатор рекламного источника,
- `costs` — расходы на эту кампанию.

---
    
**Цели исследования**

1. Изучить данные о пользователях приложения Procrastinate Pro+, привлечённых с 1 мая по 27 октября 2019 года.
2. Посмотреть, откуда приходят пользователи и какими устройствами они пользуются
3. Посчитать, сколько стоит привлечение пользователей из различных рекламных каналов.
4. Посчитать, сколько денег приносит каждый клиент.
5. Исследовать когда расходы на привлечение клиента окупаются.
6. Исследовать, какие факторы мешают привлечению клиентов.
    
---
    
***Ход исследования***
    
Данные о пользователях приложения Procrastinate Pro+ получим из трех разных датасетов. О качестве датасетов информации нет. Перед тем как приступать к целям исследования, нам необходимо изучить данные.
    
Проверим данные на предмет ошибок и оценим их влияние на результаты исследования. В процессе преодобработки данных попробуем исправить все ошибки, которые могут привести к искажению конечного результата. Далее мы выберем подходящие типы визуализации, интерпретируем графики и приступим к анализу бизнес-показателей. Напишем выводы и рекомендации на основе проведенного исследования маркетологам.
    
Таким образом, мое исследование пройдет в шесть этапов:
- изучение предоставленных данных
- предобработка данных
- исследовательский анализ данных
- исследование бизнес-показателей
- оценка окупаемости рекламы
- написание общих выводов и рекомендаций для маркетологов на основе исследования
