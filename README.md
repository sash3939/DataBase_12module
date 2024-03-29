# Домашнее задание к занятию «Базы данных»

---
### Легенда

Заказчик передал вам [файл в формате Excel](https://github.com/netology-code/sdb-homeworks/blob/main/resources/hw-12-1.xlsx), в котором сформирован отчёт. 

На основе этого отчёта нужно выполнить следующие задания.

### Задание 1

Опишите не менее семи таблиц, из которых состоит база данных:

- какие данные хранятся в этих таблицах;
- какой тип данных у столбцов в этих таблицах, если данные хранятся в PostgreSQL.

Приведите решение к следующему виду:

Сотрудники (

- идентификатор, первичный ключ, serial,
- фамилия varchar(50),
- ...
- идентификатор структурного подразделения, внешний ключ, integer).

### Решение 1
[Tables](https://github.com/sash3939/DataBase_12module/assets/156709540/769f8000-f9cd-4f30-8675-6b262b088bf1)

serial: integer auto_increment
varchar(n): строка переменной длины с максимальной длиной n
numeric: числовой тип данных с фиксированной точностью и масштабом
date: тип для хранения даты
text: строка переменной длины, предназначенная для хранения больших объемов текста


## Дополнительные задания (со звёздочкой*)
Эти задания дополнительные, то есть не обязательные к выполнению, и никак не повлияют на получение вами зачёта по этому домашнему заданию. Вы можете их выполнить, если хотите глубже шире разобраться в материале.


### Задание 2*

Перечислите, какие, на ваш взгляд, в этой денормализованной таблице встречаются функциональные зависимости и какие правила вывода нужно применить, чтобы нормализовать данные.


В таблицах оставить только те идентификаторы, с помощью которых можно избежать дублирования данных о подразделениях, филиалах и проектах и др.
Добавить вспомогательные таблицы для связи между сотрудниками и их назначенными задачами, а также между задачами и сотрудниками
