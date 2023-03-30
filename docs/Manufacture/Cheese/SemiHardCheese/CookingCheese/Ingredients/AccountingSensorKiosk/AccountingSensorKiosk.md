# Учет расхода сыроделом через сенсорный киоск

Сыродел указывает, сколько какого ингредиента он положил в котел для
конкретной варки сыра.

 

 

-   Открыть "Меню учетных точек":
    ![](AccountingSensorKiosk.assets/drex_uchet_raskhoda_syrodelom_cherez_sensornyj_kiosk_custom.png)
-   Указать текущую дату и смену, если они еще не указаны:
    ![](AccountingSensorKiosk.assets/drex_uchet_raskhoda_syrodelom_cherez_sensornyj_kiosk_custom_2.png)
-   Указать учетную точку, отвечающую за участок, где варится сыр:
    ![](AccountingSensorKiosk.assets/drex_uchet_raskhoda_syrodelom_cherez_sensornyj_kiosk_custom_3.png)
-   Нажать кнопку, соответствующую указанию ингредиентов. Откроется
    задание на текущую смену. Выбрать первую варку и нажать
    "Ингредиенты":
    ![](AccountingSensorKiosk.assets/drex_uchet_raskhoda_syrodelom_cherez_sensornyj_kiosk_custom_4.png)
-   По умолчанию таблица заполняется ингредиентами по основной спецификации выбранного сыра. При этом возможны два сценария расчета норм ингредиентов (способ [настраивается в соответствующей кнопке учетной точки](../../../../CommonInformation/Handbooks/ButtonOfAccountPoint/WorkWithTasks/WorkWithTasks.md)).



## Расчет нормы ингредиентов от объема выпуска

- В случае расчета от объема выпуска при открытии уже будут видны нормы ингредиентов. При этом, если было указано [начало варки](../AccountingTimeBeginEndTSD/AccountingTimeBeginEndTSD.md), то будет указано и плановое время внесения каждого ингредиента:

  ![image-20200803155628011](AccountingSensorKiosk.assets/image-20200803155628011.png)

-   Далее возможно ручное указание ингредиентов, в случае если до этого не было их [наборки](../../SetIngredients/SetIngredients.md), или сканирование набранных пакетов, по которому заполняется время соответствующих ингредиентов. 

### Ручной ввод
-   Если какого-то ингредиента нет в списке, добавить его:
    ![](AccountingSensorKiosk.assets/drex_uchet_raskhoda_syrodelom_cherez_sensornyj_kiosk_custom_6.png)
             
    ![](AccountingSensorKiosk.assets/drex_uchet_raskhoda_syrodelom_cherez_sensornyj_kiosk_custom_7.png)
-   Выбрать первый использованный ингредиент, указать его партию:
    ![image-20200803155732540](AccountingSensorKiosk.assets/image-20200803155732540.png)
    ![](AccountingSensorKiosk.assets/drex_uchet_raskhoda_syrodelom_cherez_sensornyj_kiosk_custom_9.png)
-   Указать количество ингредиента и нажать "Подтвердить":
    ![](AccountingSensorKiosk.assets/drex_uchet_raskhoda_syrodelom_cherez_sensornyj_kiosk_custom_10.png)

- Если указание количества основного материала происходит в литрах (если это [настроено в соответствующей кнопке учетной точки](../../../../CommonInformation/Handbooks/ButtonOfAccountPoint/WorkWithTasks/WorkWithTasks.md)), то при подтверждении будет сделан пересчет в кг (если лаборантами был внесен показатель плотности):

  ![image-20200803160248232](AccountingSensorKiosk.assets/image-20200803160248232.png)

- Аналогично заполнить остальные. Нажать кнопку сохранения:
  ![image-20200803160429989](AccountingSensorKiosk.assets/image-20200803160429989.png)

### Сканирование
-   Когда придет время внесения первого пакета, в открытой форме отсканировать QR-код, напротив ингредиентов, которые были засыпаны в пакет, проставится текущее время. Далее пакет высыпается в котел.
    
    ![image-20201214104017317](AccountingSensorKiosk.assets/image-20201214104017317.png)
    
-   Так сканируются остальные пакеты. После каждого можно сохранять данные по кнопке:
    ![image-20200803160429989](AccountingSensorKiosk.assets/image-20200803160429989.png)

## Расчет нормы ингредиентов от объема смеси

- В случае расчета от объема смеси при открытии нормы ингредиентов будут пустыми. При этом, если было указано [начало варки](../AccountingTimeBeginEndTSD/AccountingTimeBeginEndTSD.md), то будет указано и плановое время внесения каждого ингредиента:

  ![image-20200803160932154](AccountingSensorKiosk.assets/image-20200803160932154.png)

- При указании количества смеси происходит расчет и остальных норм:

  ![image-20200803161050063](AccountingSensorKiosk.assets/image-20200803161050063.png)

- Остальное заполнение делается аналогично предыдущему разделу.