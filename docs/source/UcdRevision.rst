﻿UcdRevision
===========

Объект предназначен для работы с универсальным корректировочным документом и является производным объектом от :doc:`Document <Document>`.


Свойства объекта
----------------

- **Function** (строка, чтение) - функция универсального корректировочного документа

- **Grounds** (строка, чтение) - основание документа

- **Currency** (число, чтение) - код валюты

- **TotalInc** (число, чтение) - сумма к доплате

- **TotalDec** (число, чтение) -  сумма к уменьшению

- **VatInc** (число, чтение) - сумма НДС к доплате

- **VatDec** (число, чтение) - сумма НДС к уменьшению

- **ConfirmationDate** (дата и время, чтение) - дата и время подтверждения оператора передачи документа

- **Status** (строка, чтение) - текущий статус документа в Диадоке

- **OriginalDocumentDate** (дата, чтение) - дата исходного УПД

- **OriginalDocumentNumber** (строка, чтение) - номер исходного УПД

- **AmendmentRequested** (булево, чтение) - признак, был ли запрос на уточнение

Значения свойства **Function**

- КСЧФ 
- КСЧФДИС 
- ДИС

Значения свойства **Status**

- OutboundWaitingForSenderSignature - документ исходящий, документ не отправлен, поскольку не подписан отправителем
- OutboundWaitingForInvoiceReceiptAndRecipientSignature - документ исходящий, от покупателя ожидается извещение о получении УПД/ИУПД/УКД/ИУКД, ответная подпись, либо отказ от ее формировагия
- OutboundWaitingForInvoiceReceipt - документ исходящий, ожидается извещение о получении УПД/ИУПД/УКД/ИУКД от покупателя
- OutboundWaitingForRecipientSignature - документ исходящий, ответная подпись, либо отказ от ее формирования еще не получены
- OutboundWithRecipientSignature - документ исходящий, ответная подпись получена
- OutboundRecipientSignatureRequestRejected - документ исходящий, получен отказ от формирования ответной подписи
- OutboundInvalidSenderSignature - документ исходящий, документ не отправлен, поскольку подпись отправителя не является корректной
- OutboundFinished - документ исходящий, документооборот завершен
- OutboundNotFinished - документ исходящий, извещение о получении УПД/ИУПД/УКД/ИУКД от покупателя уже есть, но документооборот еще не завершен
- InboundWaitingForRecipientSignature (документ входящий, ответная подпись, либо отказ от ее формирования еще не отправлены)
- InboundWithRecipientSignature (документ входящий, ответная подпись поставлена)
- InboundRecipientSignatureRequestRejected (документ входящий, отправлен отказ от формирования ответной подписи)
- InboundInvalidRecipientSignature (документ входящий, документооборот не завершен, поскольку подпись полуателя не является корректной)
- InboundNotFinished (документ входящий, документооборот не завершен)
- InboundFinished (документ входящий, документооборот завершен)
- UnknownDocumentStatus - неизвестный статус; может выдаваться лишь в случае, когда клиент использует устаревшую версию SDK и не может интерпретировать статус документа, переданный сервером

Методы объекта
--------------

-  :doc:`GetContent <GetContent-(UcdRevision)>` - возвращает объект титула продавца УКД
-  :doc:`GetBuyerContent <GetBuyerContent-(UcdRevision)>` - возвращает объект титула покупателя УКД
-  :doc:`SendReceiptsAsync <SendReceiptsAsync-(UcdRevision)>` - формирует и подписывает документы по регламентному документообороту УКД
-  :doc:`GetAmendmentRequestedComment <GetAmendmentRequestedComment-(UcdRevision)>` - возвращает комментарий к уведомлению об уточнении

.. toctree::
   :name: Auto
   :hidden:

   GetContent <GetContent-(UcdRevision)>
   GetBuyerContent <GetBuyerContent-(UcdRevision)>
   SendReceiptsAsync <SendReceiptsAsync-(UcdRevision)>
   GetAmendmentRequestedComment <GetAmendmentRequestedComment-(UcdRevision)>