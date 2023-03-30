# Датчики

Каждый физический датчик (на количество выпущенных сливок, на количество молока, принятого в каждый танк и т.п.) в системе должен соответствовать одному элементу справочника "Датчики". Элемент содержит информацию о том, как обрабатывать данные, получаемые с датчика.

## Вкладка Общее

- Открыть справочник "**Датчики**":

![image-1](../../../Cheese/OPCDataExchange/SystemSetting/Sensors.assets/image-1.png)

- Перейти к созданию нового элемента. Указать "**Наименование**":

![image-2](../../../Cheese/OPCDataExchange/SystemSetting/Sensors.assets/image-2.png)

- Указать "**Вариант использования**":

    - Регламентное задание - не требует участия человека, система сама получает и обрабатывает данные с датчика;
    - По запросу - обращение к датчику происходит по запросу сотрудника - по нажатию настроенной кнопки.

![image-3](../../../Cheese/OPCDataExchange/SystemSetting/Sensors.assets/image-3.png)

- Выбрать "**Тип данных**":
    - Производство - показатели количества;
    - Показатели технологического процесса. Например, показатели "**МДЖ**" и "**МДБ**";
    - Параметры производственной среды - показатели склада (например, влажность);
 
![image-4](../../../Cheese/OPCDataExchange/SystemSetting/Sensors.assets/image-4.png)

- Выбрать "**Тип значения данных**" и "**Источник данных**":
 
![image-5](../../../Cheese/OPCDataExchange/SystemSetting/Sensors.assets/image-5.png)

- Для типа данных "**Производство**" также нужно указать "**Вид пересчета**":
 
![image-6](../../../Cheese/OPCDataExchange/SystemSetting/Sensors.assets/image-6.png)

- Если используется пересчет, указать "**Способ пересчета**" и "**Показатель плотности**":
 
![image-7](../../../Cheese/OPCDataExchange/SystemSetting/Sensors.assets/image-7.png)

- Для источников данных "**SCADA**", "**Milkoscan FT2**" или "**Milkoscan FT3**" так же нужно указать "**Способ получения значения**":
 
![image-8](../../../Cheese/OPCDataExchange/SystemSetting/Sensors.assets/image-8.png)

## Вкладка Учетные данные

На вкладке "Учетные данные" заполняются индивидуальные параметры для каждого типа данных.

- Для **"Показателей технологического процесса"** необходимо заполнить показатель анализов:

![credentials-1](../../../Cheese/OPCDataExchange/SystemSetting/Sensors.assets/credentials-1.png)

- Для **"Производства"** необходимо заполнить склады:

![credentials-2](../../../Cheese/OPCDataExchange/SystemSetting/Sensors.assets/credentials-2.png)

- Для **"Параметров производственной среды"** необходимо заполнить склад и показатель склада:

![credentials-3](../../../Cheese/OPCDataExchange/SystemSetting/Sensors.assets/credentials-3.png)

## Вкладка Подключение

### OPC

- Указать "**Тег значение**":

![image-9](../../../Cheese/OPCDataExchange/SystemSetting/Sensors.assets/image-9.png)

- Опционально можно указать "**Тег дата готовности значения**":

![image-10](../../../Cheese/OPCDataExchange/SystemSetting/Sensors.assets/image-10.png)

### SCADA

- Нажать **"Подобрать"**. Выбрать строку, соответствующую нужному датчику (сенсор, операции, места хранения).

![image-11](../../../Cheese/OPCDataExchange/SystemSetting/Sensors.assets/image-11.png)

- Нажать на кнопку **"Выбрать"**

![image-12](../../../Cheese/OPCDataExchange/SystemSetting/Sensors.assets/image-12.png)

- Значения идентификаторов заполнятся автоматически:

![image-13](../../../Cheese/OPCDataExchange/SystemSetting/Sensors.assets/image-13.png)

### Milkoscan FT2/FT3

??? Info "Чтобы указать Milkoscan как "**Источник данных**" на вкладке Общее, необходимо в качестве "**Типа данных**" выбрать "**Показатели технологического процесса**""

- Выбрать "**Показатель анализов**":

![image-15](../../../Cheese/OPCDataExchange/SystemSetting/Sensors.assets/image-15.png)

## Запись и проверка подключения

- Когда все поля заполнены, нужно нажать кнопку "**Записать**". После записи появляется возможность проверить датчик, нажав на кнопку "**Проверить подключение**":

![image-16](../../../Cheese/OPCDataExchange/SystemSetting/../../../Cheese/OPCDataExchange/SystemSetting/Sensors.assets/image-16.png)

## Настройки датчика для записи в регистр "Данные к обработке"

- Для передачи данных в регистр "**Данные к обработке**" и дальнейшего использования в обработке "**Рабочее место мастера смены**" нужно:
    -  Заполнить поле "**Оборудование**"
    -  Указать "**Вариант использования**" - "Регламентное задание"
    -  Указать "**Тип данных**" - "Производство" или "Параметры производственной среды"
    -  Указать "**Тип значения данных**" - "Число"

![image-17](../../../Cheese/OPCDataExchange/SystemSetting/../../../Cheese/OPCDataExchange/SystemSetting/Sensors.assets/image-17.png)