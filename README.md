# Анализ результатов A/B теста для турагенства.

### Описание проекта    
Оценка статистической значимости результатов A/B теста. 


### Какой кейс решаем?    
Компания планирует запустить новую акцию, чтобы продать как можно больше туров. Команда разработала два варианта посадочной страницы официального сайта компании и провела A/B-тестирование.
Необходимо оценить эффективность обоих вариантов посадочной страницы сразу по двум критериям: конверсии покупки и среднему чеку. На основе проведенного анализа решим: какой из вариантов дизайна более предпочтительный.


### Краткая информация о данных
Предоставлены 294478 записей транзакций клиентов. Среди данных:

* user_id - идентификатор пользователя, зашедшего на сайт;
* data — дата посещения сайта;
* group — группа теста (контрольная — А или тестовая — B);
* purchase — признак покупки: совершил ли пользователь покупку тура (1 — да, 0 — нет);
* price — цена купленного тура (если покупка не состоялась, цена равна 0).

### Этапы работы над проектом  
1. Загрузка и подготовка данных
2. Оценка кумулятивных метрик
3. Статистические тесты
4. Довирительные интервалы
5. Машинное обучение
6. Тест на нормальность и оценка среднего чека
7. Выводы

### Результаты:  
* Был проведен первичный анализ данных, удалены общие для групп клиенты.
* Для оценки метрик во времени были построены кумулятивные значения конверсии и среднего чека - данные стабильны во времени.
* Статестический z-тест и построение доверительных интервалов показали, что разницы в конверсии между группами нет.
* T-тест и доверительные интервалы для среднего чека показали, что средний чек в группе B однозначно больше.
* Был сделан вывод, что вариант B более эффективный.
