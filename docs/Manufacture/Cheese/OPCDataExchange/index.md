# Общая информация

Если на предприятии около различных устройств (на танках сырого молока при закачке из машин, на участке сепарации у выхода сливок и т.п.), установлены датчики, то передачу данных с этих датчиков в систему можно выполнить без участия человека (или с минимальным его участием).



Для этого разворачивается сервер, куда передается информация со всех подключенных датчиков. MES-система периодически обращается к этому серверу, запрашивая и получая данные для дальнейшей обработки.



Такая интеграция упрощает процесс [приемки молока](MilkReceivingQuality.md), выпуска сливок/обрата/схожих продукций [через киоски](AcceptanceAndTransfer.md), а также процесс выпуска/перемещения продукции в [рабочем месте мастера смены](ShiftMaster.md).