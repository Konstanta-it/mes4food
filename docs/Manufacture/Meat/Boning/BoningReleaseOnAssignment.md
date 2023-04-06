# Выпуск продуктов обвалки по производственному заданию

Для выпуска по заданию необходимо создать производственное задание, как это описано в разделе ["Создание производственного задания"](./ProductionAssignment.md).

- В подсистеме **"Производство"** открываем **"Меню учетных точек"**:

![](BoningReleaseOnAssignment.assets/1.png)

- Указываем дату смены, смену и учетную точку, на которой производится выпуск продуктов обвалки. Нажимаем на кнопку **"Выпуск с обвалки по заданию"**:

![](BoningReleaseOnAssignment.assets/2.png)

- Открывается список производственных заданий на указанную смену.

Для выполнения необходимо выбрать задание в статусе "Не начато" либо "В процессе". При необходимости можно отфильтровать задания в списке по статусу, выбрав нужный в строке "Состояние" в шапке АРМа.

Выбираем в списке  строку задания, по которому планируется выпуск продуктов обвалки/разделки, нажимаем кнопку "Приступить":

![](BoningReleaseOnAssignment.assets/3.png)

- В верхнем левом углу находится информация о номенклатуре выпуска, указанной в задании.

Справа указаны рабочий центр и склад-получатель по умолчанию. Если на складе-получателе используются складские ячейки, необходимо выбрать ячейку из списка.

С помощью калькулятора тары указываем тару, в которой производится взвешивание выходного изделия.

Получаем с весов вес брутто, вес нетто рассчитается автоматически, нажимаем на кнопку **"Подтвердить"**:

![](BoningReleaseOnAssignment.assets/4.png)

- После подтверждения выпуска печатается этикетка партии сырья:

![](BoningReleaseOnAssignment.assets/5.png)

- Если выпущено меньшее количество продукта, чем указано в задании, состояние задания останется **"В процессе"**. 

Если веса недостаточно, для завершения задания, можно завершить его вручную:

![](BoningReleaseOnAssignment.assets/6.png)

- В списке заданий завершенное задание будет выделено зеленым цветом, его состояние изменится на **"Выполнено"**:

![](BoningReleaseOnAssignment.assets/7.png)

- Если взвешено ровно запланированное или большее количество выходного изделия, статус задания изменится автоматически:

![](BoningReleaseOnAssignment.assets/8.png)

- По результатам выпуска продуктов по заданию в окне рабочего места мастера смены отображается фактический выпуск продукта и процент отклонения от плана выпуска:

![](BoningReleaseOnAssignment.assets/9.png)