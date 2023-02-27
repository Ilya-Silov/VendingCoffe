# VendingCoffe
## Discription
В качестве предметной области выбраны аппараты по разливу горячих напитков 
программа подразумевает наличия общей базы данных(бд) на сервере и локальной бд на каждом аппарате  
P.S или только аппараты

Реализовать:
- просмотр доступных товаров
- просмотр раширеной информации о заказе
- 1 напиток = 1 заказ
- синхронизация локальной бд с серверной (при наличии серверной)
- группировка товаров

Продумать:
- теги для товаров(отдельная таблица много ко многим в которую записываются теги)  
  P.S скорее всего хранятся только локально на аппарате, но настраиваются из админ панели

## Etities

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

