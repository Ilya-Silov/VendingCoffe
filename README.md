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


<div class="mxgraph" style="max-width:100%;border:1px solid transparent;" data-mxgraph="{&quot;highlight&quot;:&quot;#0000ff&quot;,&quot;nav&quot;:true,&quot;resize&quot;:true,&quot;toolbar&quot;:&quot;zoom layers tags lightbox&quot;,&quot;url&quot;:&quot;https://drive.google.com/uc?id=1TO40At75Du-_QEwryULpeuAFC_8_mClj&amp;export=download&quot;}"></div>
<script type="text/javascript" src="https://viewer.diagrams.net/embed2.js?&fetch=https%3A%2F%2Fdrive.google.com%2Fuc%3Fid%3D1TO40At75Du-_QEwryULpeuAFC_8_mClj%26export%3Ddownload"></script>
