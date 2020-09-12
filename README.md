# Construction company database

## Задание №19: БД Строительной компании.

Таблицы:	
Сотрудники (Код сотрудника, ФИО, Возраст, Пол, Адрес, Телефон, Паспортные данные, Код должности)[10 записей].
Должности (Код должности, Наименование должности, Оклад, Обязанности, Требования)[5 записей].
Виды работ (Код вида, Наименование, Описание, Цена работы, Код материала 1, Код материала 2, Код материала 3)[5 записей].
Материалы (Код материала, Наименование, Упаковка, Описание, Цена) [5 записей].
Бригады (Код бригады, Код сотрудника 1, Код сотрудника 2, Код сотрудника 3) [5 записей].
Заказчики (Код заказчика, ФИО, Адрес, Телефон, Паспортные данные)[5 записей].
Заказы (Код заказчика, Код вида работ, Код бригады, Стоимость, Дата начала, Дата окончания, Отметка о завершении, Об оплате, Код сотрудника) [10 записей].

Запросы:	
Отдел кадров (Связывает таблицы "Сотрудники" и "Должности" по полю "Код должности").
Список работ (Связывает таблицы "Виды работ" и "Материалы" по полям "Код материала", "Код материала 1", "Код материала 2" и "Код материала 3").
Список бригад (Связывает таблицы "Бригады" и "Сотрудники" по полям "Код сотрудника", "Код сотрудника 1", "Код сотрудника 2" и "Код сотрудника 3").
Список заказов (Связывает таблицы "Заказы", "Виды работ", "Бригады" и "Сотрудники" по полям "Код вида", "Код бригады" и "Код сотрудника").

Фильтры:	
Фильтры для отображения сотрудников отдельных должностей (На основе запроса "Отдел кадров").
Фильтры для отображения отдельных видов работ (На основе запроса "Список работ").
Фильтры заказов на конкретные работы (На основе запроса "Список заказов").
Фильтры для отображения заказов отдельных заказчиков (На основе запроса "Список заказов").
Фильтры на заказы, выполняемые отдельными бригадами (На основе запроса "Список заказов").
Фильтры для завершённых и не завершённых заказов (На основе запроса "Список заказов").
Фильтры для оплаченных и неоплаченных заказов (На основе запроса "Список заказов").
