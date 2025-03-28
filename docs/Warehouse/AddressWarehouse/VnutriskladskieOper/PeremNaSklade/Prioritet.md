# Формирование приоритетов размещения/перемещения в ячейки

Правила и приоритеты размещения номенклатуры задаются только для складов с адресной системой хранения.

### Настройка склада

Использование адресной системы хранения включается в справочнике **"Склады"** в подсистеме **"Нормативно-справочная информация"**.

![](Prioritet.assets/image.png)

На этой вкладке также задаются приоритеты размещения номеклатуры по ячейкам склада. Например, на скриншоте:

- 1 приоритет: *свободные ячейки* - значит, при размещении всегда будет в первую очередь подбираться свободная ячейка;
- 2 приоритет: *монотоварные по серии* - если не найдена свободная ячейка, будет подбираться ячейка, где уже лежит номенклатура той же серии;
- 3 приоритет: *монотоварные* - если не найдена монотоварная по серии ячейка, будет подбираться ячейка, где уже лежит такая номенклатура любой серии;
- 4 приоритет: *политоварные* - если не найдены другие подходящие ячейки, будет подбираться любая ячейка, независимо от номенклатуры и серии, которая там лежит.

Порядок и выбор приоритетов можно задавать самостоятельно по кнопкам **"Добавить"** и **"Вверх"**/**"Вниз"**.

### Настройка ячейки

Чтобы ограничения работали, для складских ячеек также должен быть задан типоразмер и правило, по которому в ячейку размещается номенклатура. Для этого нужно перейти в справочник **"Складские ячейки"**, выбрать ячейку склада и перейти к полю **"Типоразмер"**:

![](Prioritet.assets/image-1.png)

При создании типоразмера указывается правило, по которому в ячейку размещается номенклатура (например, ячейка может быть только монотоварной по серии), и ограничения по габаритам (например, не больше 500 кг, тогда при размещении в ячейку нельзя будет поместить паллету весом 600 кг).

![](Prioritet.assets/image-2.png)
![](Prioritet.assets/image-3.png)

Аналогично типоразмер ячеек можно задать на этапе [генерации топологии склада](../../../../CommonInformation/WarehouseTopologyGeneration.md):

![](Prioritet.assets/image-4.png)

### Формирование приоритетов размещения

Приоритеты размещений задаются для операций перемещения из ячейки приемки в ячейки хранения (размещение) и для перемещения между ячейками хранения. Обработка находится в подсистеме **"Склад и доставка"** - **"Формирование приоритетов размещения"**:

![](Prioritet.assets/image-5.png)

Для настройки приоритетов нужно выбрать склад и вид отображения: по ячейкам или по номенклатурам. 

![](Prioritet.assets/image-6.png)

Если выбран вид *"Ячейки"*, то в левую таблицу выводятся вся топология склада и правила размещения, заданные для этих ячеек. В правую таблицу подтягиваются уже заданные номенклатуры, которые могут помещаться в ячейку, и приоритеты их размещения:

![](Prioritet.assets/image-7.png)

Для добавления списка номенклатур, которые могут помещаться в ячейку, нужно выбрать ячейку и нажать **"Подобрать"**. Затем через форму подбора номенклатур заполнить список:

![](Prioritet.assets/image-8.png)

После подбора номенклатур система сразу предложит установить приоритет:

![](Prioritet.assets/image-9.png)

После нажатия кнопки **"ОК"** номенклатура с соответствующим приоритетом будет перенесена в таблицу справа. Приоритет можно редактировать вручную.

![](Prioritet.assets/image-10.png)

Если выбран вид отображения *"Номенклатура"*, то по кнопке **"Заполнить по регистру"** левая таблица будет заполнена уже сохраненными значениями. В правой таблице отображается ячейка, в которую может размещаться номенклатура, и приоритет размещения.

![](Prioritet.assets/image-11.png)

Для добавления новых записей можно воспользоваться кнопками **"Подобрать"** и **"Назначить приоритет"**.