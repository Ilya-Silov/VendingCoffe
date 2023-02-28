# VendingCoffe
## Discription
В качестве предметной области выбраны аппараты по разливу горячих напитков 
программа подразумевает наличия общей базы данных(бд) на сервере и локальной бд на каждом аппарате
P.S или только аппараты

## TO DO
DB аппарата должна включать:
- продажи
- список товаров

Доп:
- 1 напиток = 1 заказ
- синхронизация локальной бд с серверной (при наличии серверной)
- группировка товаров

Продумать:
- теги для товаров(отдельная таблица много ко многим в которую записываются теги)  
  P.S скорее всего хранятся только локально на аппарате, но настраиваются из админ панели

## Etities
### Local
- Sale
    - datetime
    - product
- Product
  - name
  - description
  - compound
  - priceID
  - GroupID
- Price
  - priceID
  - price
  - datestart
- Category
  - CategoryID
  - name
  - parentCategory

(таблица с составляющими для напитков)
