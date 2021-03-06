﻿Act552SellerContent
===================

Объект предназначен для работы с содержанием документов типа "Акт в
формате 552-го приказа ФНС"

Свойства
--------

- **Seller** (объект :doc:`ExtendedOrganizationInfo <ExtendedOrganizationInfo>`, чтение) - исполнитель (продавец услуг)

- **Buyer** (объект :doc:`ExtendedOrganizationInfo <ExtendedOrganizationInfo>`, чтение) - заказчик (покупатель услуг)

- **Signers** (коллекция :doc:`Collection <Collection>` объектов :doc:`ExtendedSigner <ExtendedSigner>`, чтение) - подписанты

- **Grounds** (коллекция :doc:`Collection <Collection>` объектов :doc:`GroundInfo <GroundInfo>`, чтение) - основания

- **Currency** (строка, чтение/запись) - валюта (код)

- **CurrencyRate** (строка, чтение/запись) - курс валюты

- **Works** (коллекция :doc:`Collection <Collection>` объектов :doc:`Act552WorkDescription <Act552WorkDescription>`) - описание выполненных работ

- **DocumentDate** (дата, чтение/запись) - дата составления документа о передаче товара

- **DocumentNumber** (строка, чтение/запись) - номер документа о передаче товара

- **RevisionDate** (дата, чтение/запись) - дата исправления документа

- **RevisionNumber** (строка, чтение/запись) - номер исправления документа

- **DocumentCreator** (строка, чтение/запись) - составитель файла информации продавца

- **DocumentCreatorBase** (строка, чтение/запись) - основание, по которому экономический субъект является составителем файла

- **OperationType** (строка, чтение/запись) - вид операции

- **OperationTitle** (строка, чтение/запись) - заголовок содержания операции

- **GovernmentContractInfo** (строка, чтение/запись) - идентификатор государственного контракта

- **AdditionalInfo** (объект :doc:`AdditionalInfoId <AdditionalInfoId>`, чтение) - информационное поле документа

- **DocumentName** (строка, чтение/запись) - наименование первичного документа, определенное организацией

- **TransferInfo** (объект :doc:`Act552TransferInfo <Act552TransferInfo>`) - содержание факта хозяйственной жизни - сведения о передаче результатов работ (о предъявлении оказанных услуг)

Методы
------

-  :doc:`AddSigner <AddSigner-(Act552SellerContent)>` - добавляет новый элемент в коллекцию подписантов

-  :doc:`AddGround <AddGround-(Act552SellerContent)>` - добавляет основание в список оснований

-  :doc:`AddWork <AddWork-(Act552SellerContent)>` - добавляет элемент в коллекцию описаний выполненных работ

.. toctree::
   :name: Auto
   :hidden:

    AddSigner <AddSigner-(Act552SellerContent)>
    AddGround <AddGround-(Act552SellerContent)>
    AddWork <AddWork-(Act552SellerContent)>
    Act552WorkDescription <Act552WorkDescription>
    Act552TransferInfo <Act552TransferInfo>