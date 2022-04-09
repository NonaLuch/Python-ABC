# ЗАДАЧА

В крупном онлайн-магазине, который реализует товары «всё для праздников». Вам необходимо провести ABC-анализ и выявить наиболее важные товары на основе объемов продаж и популярности. Эта информация составит план закупок на весь следующий год.

#### Задача анализа разделить товары на группы по принципу:

- А — наиболее ценные, 20% — ассортимента (номенклатура); 80% — продаж
- В — промежуточные, 30% — ассортимента; 15% — продаж
- С — наименее ценные, 50% — ассортимента; 5% — продаж

# Этапы выполнения

1. Сохраним все данные из таблицы products из PostgreSQL в дата-фрейм products и подготовим данные к анализу.
2. Посчитаем, какой доход принес каждый продукт и сколько единиц каждого продукта было продано.
3. Найдем нарастающий итог по процентам.
4. Пометим товары метками 'A', 'B', 'C' в зависимости от нарастающего итога.
5. Найдем нарастающий итог по количеству товарных единиц и пометим товары метками 'A', 'B', 'C', отмечая тем самым популярность товара.
6. Объединим группы и проанализируем.
7. Выгрузим данные по товарам с меткой по ABC-анализу для отдела закупок.


