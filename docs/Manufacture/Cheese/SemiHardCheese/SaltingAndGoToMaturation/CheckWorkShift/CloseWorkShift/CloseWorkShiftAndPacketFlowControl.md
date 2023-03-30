# Закрытие смен и контроль расхода пакетов


Контроль всех введенных в систему данных за рабочую смену осуществляется
мастером смены через "Рабочее место мастера смены"

 

 

-   Открыть "Рабочее место мастера смены":  
    ![](CloseWorkShiftAndPacketFlowControl.assets/drex_zakrytie_smen_i_kontrol_raskhoda_paketov_custom.png)
    
-   Указать дату и смену:  
    ![](CloseWorkShiftAndPacketFlowControl.assets/drex_zakrytie_smen_i_kontrol_raskhoda_paketov_custom_2.png)
    
-   Указать участок, на котором сыр извлекается из солилки и
    упаковывается в пакеты:  

    ![](CloseWorkShiftAndPacketFlowControl.assets/drex_zakrytie_smen_i_kontrol_raskhoda_paketov_custom_3.png)

-   В таблице ниже выбрать участок извлечения сыра из солилки, который
    необходимо проверить на корректность. Справа заполнится различная
    информация по данному участку. Например, на вкладке "Выпуск"
    отображается вся информация по извлеченным варкам за указанную смену:  

    ![](CloseWorkShiftAndPacketFlowControl.assets/drex_zakrytie_smen_i_kontrol_raskhoda_paketov_custom_4.png)

-   На вкладке "Остатки" -\> "Полуфабрикаты" можно видеть условные
    остатки кг сыра, получившиеся в результате разницы между входным
    количеством сыра в солилку и извлеченным. Они получаются из-за
    процесса усушки. Эти остатки необходимо "списать" со статьей
    расходов "Усушка" для дальнейшего учета в системе. Для этого
    выделить все строки, конечный остаток которых ненулевой, нажать
    "Списать усушку":  
    ![](CloseWorkShiftAndPacketFlowControl.assets/drex_zakrytie_smen_i_kontrol_raskhoda_paketov_custom_5.png)

-   На вкладке "Остатки" -\> "Материалы" можно видеть израсходованные
    пакеты (столбец "Расход"). Проверяется и контролируется
    неотрицательность остатков (столбец "Кон.остаток").
    Если при упаковке сыра по ошибке были выбраны не те пакеты (см.
    [Учет извлечения сыра](../../PoolCheeseExtractionAndPacking/AccountingPoolCheeseExtractionAndPacking.md)), здесь их можно заменить на корректные. Для этого выбрать ошибочные пакеты и нажать "Заменить материал":  
    ![image-20200818104134157](CloseWorkShiftAndPacketFlowControl.assets/image-20200818104134157.png)
    
-   Выбрать пакеты для замены:  
    ![](CloseWorkShiftAndPacketFlowControl.assets/drex_zakrytie_smen_i_kontrol_raskhoda_paketov_custom_7.png)

-   Указать количество заменяемых и подтвердить:  
    ![](CloseWorkShiftAndPacketFlowControl.assets/drex_zakrytie_smen_i_kontrol_raskhoda_paketov_custom_8.png)

-   Если в процессе упаковки сыра были выявлены бракованные пакеты, то
    здесь же можно учесть и их. Для этого выбрать пакет для учета его
    брака и нажать "Списать":  
    ![](CloseWorkShiftAndPacketFlowControl.assets/drex_zakrytie_smen_i_kontrol_raskhoda_paketov_custom_9.png)

-   Указать, что идет списание брака:  
    ![image-20200910095047754](CloseWorkShiftAndPacketFlowControl.assets/image-20200910095047754.png)

-   Указать статью затрат для брака и указать количество отбракованных
    пакетов. Подтвердить:  
    ![image-20200910095150744](CloseWorkShiftAndPacketFlowControl.assets/image-20200910095150744.png)

-   После выполнения всех вышеперечисленных действий и проверки
    корректности всех данных, смену необходимо закрыть для невозможности
    внесения в нее изменений. Для этого выбрать участок в таблице слева
    и нажать "Закрыть":  
    ![](CloseWorkShiftAndPacketFlowControl.assets/drex_zakrytie_smen_i_kontrol_raskhoda_paketov_custom_12.png)

-   При возникновении ошибок (например, отрицательных остатков - как следствие неточного или неоперативного учета) система выдаст
предупреждения. Устранить ошибки, нажать еще раз "Закрыть".
    