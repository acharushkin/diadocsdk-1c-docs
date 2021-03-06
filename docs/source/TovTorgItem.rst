﻿TovTorgItem
===========

Сведения о товаре торг-12 в формате 551-го приказа

Свойства объекта
----------------


- **Product** (строка, чтение/запись) - наименование товара

- **Feature** (строка, чтение/запись) - характеристика товара

- **Sort** (строка, чтение/запись) - сорт товара

- **VendorCode** (строка, чтение/запись) - артикул товара

- **ProductCode** (строка, чтение/запись) - код товара

- **UnitName** (строка, чтение/запись) - наименование единицы измерения товара

- **Unit** (строка, чтение/запись) - единицы измерения товара (код)

- **PackageType** (строка, чтение/запись) - вид упаковки товара

- **QuantityInPack** (число, чтение/запись) - количество мест в 1 упаковке

- **Quantity** (число, чтение/запись) - количество единиц товара

- **Gross** (число с плавающей точкой/строка, чтение/запись) - масса брутто

- **Net** (число с плавающей точкой/строка, чтение/запись) - масса нетто, количество передано (отпущено)

- **ItemToRelease** (число, чтение/запись) - Количество надлежит отпустить

- **Price** (число с плавающей точкой/строка, чтение/запись) - цена за единицу товара

- **SubtotalWithVatExcluded** (число с плавающей точкой/строка, чтение/запись) - сумма без учета налога

- **TaxRate** (строка, чтение/запись) - ставка налога

- **Vat** (число с плавающей точкой/строка, чтение/запись) - сумма налога

- **Subtotal** (число с плавающей точкой/строка, чтение/запись) - сумма всего

- **ItemAccountDebit** (строка, чтение/запись) - Корреспондирующие счета: дебет

- **ItemAccountCredit** (строка, чтение/запись) - Корреспондирующие счета: кредит

- **StructedAdditionalInfos** (коллекция :doc:`Colection <Collection>` объектов :doc:`StructedAdditionalInfo <StructedAdditionalInfo>`) - Информационное поле документа

Свойство **TaxRate** принимает одно из следующих значений:

-  "10/110" - ставка налога 10/110 (дробь)
-  "18/118" - ставка налога 18/118 (дробь)
-  "без НДС" - без НДС
-  "0" - ставка налога 0%
-  "10" - ставка налога 10%
-  "18" - ставка налога 18%
-  "ИсчНалАг" - НДС исчисляется налоговым агентом

Числа рекомендуется записывать строкой в виде XML представления типа decimal (см. http://www.w3.org/TR/xmlschema-2/#decimal)
В 1С такое представление можно получить с помощью функции глобального контекста XMLСтрока (XMLString)

Методы объекта
--------------

-  :doc:`AddStructedAdditionalInfo <AddStructedAdditionalInfo-(TovTorgItem)>` - добавляет новый элемент в список дополнительных сведений информационного поля документа


.. toctree::
   :name: Auto
   :hidden:

   AddStructedAdditionalInfo <AddStructedAdditionalInfo-(TovTorgItem)>