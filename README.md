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

## Local

### Etities
- Sale
  - id
  - datetime
  - product
- Product
  - id
  - name
  - description
  - compound
  - price_id
  - group_id
- Price
  - id
  - price
  - datestart
- Category
  - id
  - name
  - parent_category_id
- Constituence (trigger на добавление в таблицу с покупками на удаление из кол-ва)
  - id
  - const_name
  - amount
- Compound (подумать как считать кол-во разных типов составляющих)
  - product_id
  - constituence_id
  - amount_of_constituence

## Server
### Entities
