# metall
Блок 1: Таблица с складскими остатками
    Требования:
        * подключение разных пользователей
        * каждый видит свою таблицу
        * данные таблицы могут изменятся извне
        * сквозной номер позиции для всей системы: номер лота
        * веб фронтенд
        * возможность удобно заносить данные и менять их
        * у каждого пользователя до 100 записией в таблице
        * стуктура доступа: тер подразделение -> супервайзер -> кладовщик
        * при вводе данных срабатывает триггер и обновляются или пересчитываются данных в других ячейках этой таблицы
        * администраторский доступ: возможность массового добавления-удаления, фильтр по параметрам поиска
Блок 2: Интернет магазин
    Требования:
        * синхронизация с таблицей из Блока 1
        * после завершения редактирования (утверждения) строки таблицы - публикуется новый товар в ИМ
        * в случае удаления строки или пометки удаленная, товар из ИМ снимается с публикации
        * синхронизация через сквозной номер позиции: номер лота
        * расчет цены на сайте через формулу на основании цены из таблицы складских остатков
        * корзина: оплата онлайн и выставление счет на безналичную оплату
        * корзина: оформление заказа
        * резервирование товара после оформления заказа: поставить пометку в таблицу Блока 1 о резервировании лота
        * добавить +- 3000 товаров в магазин с ценой "под заказ", структура категорий и типов есть
        * отправка web hook для интеграции при разных событиях в ИМ: добавление товара, оформление заказа, покупка и тд
        * интеграция с 1С: получение информации об оплаченном счете

Блок 3: Ретробонусы
        * отдельный сервис или внутри ИМ
        * формула скидки или ретробонусов от объемов
        * учет реферальных клиентов
  
