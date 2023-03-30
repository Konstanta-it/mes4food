**Установка цен и параметров расчетов цен по поставщикам**
==========================================================

Расчет стоимости поступающего молока происходит на основании следующей
установленной информации в системе.


**Коэффициенты стоимости жира и белка в молоке**

-   Коэффициенты жира и белка в расчете стоимости сырья заполняются в "Настройки параметров учета":  
![](ustanovka_tsen_i_parametrov_raschetov_tsen.assets/drex_ustanovka_tsen_i_parametrov_raschetov_tsen.png)  
-   На вкладке "Баланс жира и белка" заполнить соответствующие поля и нажать "Записать и закрыть":  
![](ustanovka_tsen_i_parametrov_raschetov_tsen.assets/drex_ustanovka_tsen_i_parametrov_raschetov_tsen_2.png)


**Справочник "Виды цен"**


Для каждого поставщика нужно создать вид цены, который в дальнейшем
    будет определять стоимость его молока базовой жирности. 
    
-    Открыть справочник "Виды цен" и перейти к созданию нового элемента:   
![](ustanovka_tsen_i_parametrov_raschetov_tsen.assets/drex_ustanovka_tsen_i_parametrov_raschetov_tsen_3.png)  
-   В поле "Наименование" указать, к какому поставщику относится
    создаваемый вид цены. В поле "Валюта" - валюта, в которой будут идти
    расчеты с этим поставщиком:  
![](ustanovka_tsen_i_parametrov_raschetov_tsen.assets/drex_ustanovka_tsen_i_parametrov_raschetov_tsen_4.png)  
-    "Способ задания" указать "Ручной ввод" и нажать "Записать и
    закрыть":  
![](ustanovka_tsen_i_parametrov_raschetov_tsen.assets/drex_ustanovka_tsen_i_parametrov_raschetov_tsen_5.png)


**Установка стоимости молока базисной жирности**

Для каждого поставщика задать стоимость его молока базовой жирности.

-   Открыть документы "История изменеия цен" и перейти к
    созданию нового:   
![](ustanovka_tsen_i_parametrov_raschetov_tsen.assets/drex_ustanovka_tsen_i_parametrov_raschetov_tsen_6.png)  
-   В таблице перечислить цены всех поставщиков, которые будут заданы
    далее, и нажать "Перейти к установке цен":  
![](ustanovka_tsen_i_parametrov_raschetov_tsen.assets/drex_ustanovka_tsen_i_parametrov_raschetov_tsen_7.png)  
-   В таблицу добавить номенклатуру молочного сырья:  
![](ustanovka_tsen_i_parametrov_raschetov_tsen.assets/drex_ustanovka_tsen_i_parametrov_raschetov_tsen_8.png)  
-   Заполнить столбцы "Новая цена" под каждым поставщиком
    соответствующей стоимостью:  
![](ustanovka_tsen_i_parametrov_raschetov_tsen.assets/drex_ustanovka_tsen_i_parametrov_raschetov_tsen_9.png)  
-   Нажать "Провести и закрыть".


**Соглашения с поставщиками.**

Для каждого поставщика задать индивидуальные условия, по которым будет считаться стоимость молока.

-   Открыть справочник "Соглашения об условиях продаж" и перейти к созданию его нового элемента:  
![](ustanovka_tsen_i_parametrov_raschetov_tsen.assets//drex_ustanovka_tsen_i_parametrov_raschetov_tsen_10.png)  
-   Заполнить информацию на вкладке "Основное": поставщик, для которого
    создается это соглашение, нашу организацию и установить статус
    "Действует":  
![](ustanovka_tsen_i_parametrov_raschetov_tsen.assets/drex_ustanovka_tsen_i_parametrov_raschetov_tsen_11.png)  
-   На вкладке "Ценовые условия" указать валюту, в которой ведутся
    расчеты, и выбрать вид цены, соответствующий поставщику:  
![](ustanovka_tsen_i_parametrov_raschetov_tsen.assets/drex_ustanovka_tsen_i_parametrov_raschetov_tsen_12.png)   
-   На вкладке "Условия поставки" указать, каким образом учитывать
    отклонения фактических значенений от заявленных поставщиком при
    приемке:  
![](ustanovka_tsen_i_parametrov_raschetov_tsen.assets/drex_ustanovka_tsen_i_parametrov_raschetov_tsen_13.png)  
-    Также, здесь можно задать индивидуальные условия расчета стоимости
    сырья. Для этого отметить данный пункт галочкой:  
![](ustanovka_tsen_i_parametrov_raschetov_tsen.assets/drex_ustanovka_tsen_i_parametrov_raschetov_tsen_14.png)  
-   Выбрать способ расчета стоимости сырья:
    -   стандартный - по жиру и белку, т.е. при расчете стоимости молока
    будет учитываться содержание и белка, и жира в молоке
    -   только по жиру - в этом случае содержание белка в молоке
    игнорируется:  
    ![](ustanovka_tsen_i_parametrov_raschetov_tsen.assets/drex_ustanovka_tsen_i_parametrov_raschetov_tsen_15.png)       
-   Указать базу расчета стоимости сырья:
    -   по физическому весу - тогда стоимость будет считаться как  
    ```
    вес принятого молока * стоимость молока базовой жирности этого поставщика *
    коэффициент сорта * коэффициент, учитывающий содержание жира (или жира и белка, в зависимости от указанного выше условия), коэффициенты жира и белка, заданные в параметрах учета, и нормативы содержания их в молоке базовой жирности
    ```
    -   по зачетному весу - тогда стоимость будет считаться как  
    ```
    стоимость молока базовой жирности поставщика * зачетный вес, который считается как физический вес * коэффициент сорта * коэффициент, учитывающий содержание жира (или жира и белка, в зависимости от указанного выше условия), коэффициенты жира и белка, заданные в параметрах учета, и нормативы содержания их в молоке
    базовой жирности
    ```
    ![](ustanovka_tsen_i_parametrov_raschetov_tsen.assets/drex_ustanovka_tsen_i_parametrov_raschetov_tsen_16.png)  
-   Для жира (или и жира, и белка) и зачетного веса (если была выбрана
    такая база расчета) задать точность округления при расчетах:  
![](ustanovka_tsen_i_parametrov_raschetov_tsen.assets/drex_ustanovka_tsen_i_parametrov_raschetov_tsen_17.png)  
-   Если установлена база расчета по зачетному весу, то можно указать, по какому принципу будет округляться этот вес:
    - В пользу предприятия - всегда в бОльшую сторону;
    
    - В пользу поставщика - всегда в меньшую сторону;
    
    - По математическим правилам
    
      ![image-20201211144105319](ustanovka_tsen_i_parametrov_raschetov_tsen.assets/image-20201211144105319.png)
-   В таблице ниже можно задать индивидуальные коэффициенты каждого
    сорта (либо же оставить таблицу пустой, тогда будут использованы
    общие коэффициенты):  
![](ustanovka_tsen_i_parametrov_raschetov_tsen.assets/drex_ustanovka_tsen_i_parametrov_raschetov_tsen_18.png)  
-   Нажать "Записать и закрыть". Повторить пункты для каждого
    поставщика.