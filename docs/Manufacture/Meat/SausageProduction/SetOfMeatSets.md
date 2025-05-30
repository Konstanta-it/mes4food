# Набор комплектов мясного сырья

Для выпуска комплекта мясного сырья необходимо создать производственное задание, как это описано в разделе ["Создание производственного задания на наборку сырья"](./CreateTaskForASet.md).

- В подсистеме **"Производство"** открываем **"Меню учетных точек"**:

![](SetOfMeatSets.assets/1.png)

- Указываем дату смены, смену и рабочий участок, на котором будет выполняться стандартизация сырья.

- Нажимаем на кнопку **"Комплектация мясного сырья"**:

![](SetOfMeatSets.assets/2.png)

- В списке заданий выбираем строку производственного задания, по которому будет осуществляться наборка по рецептуре и нажимаем на кнопку **"Наборка"**.

![](SetOfMeatSets.assets/3.png)

- Открылось окно наборки: слева находится информация о партии производимого полуфабриката и рецептура для наборки с указанием планового веса ингредиентов.

В таблице рецептуры указан плановый вес, который необходимо набрать.

- Сканируем штрихкод тары, в которой будет взвешиваться полуфабрикат, или выбираем номер тары из списка. Вес тары указывается автоматически:

![](SetOfMeatSets.assets/4.png)

- Сканируем штрихкод номенклатуры материала, который планируем мариновать, или выбираем партию материала вручную. При необходимости можно выбрать несколько партий используемого материала. Для этого после взвешивания первой партии необходимо повторно открыть форму подбора и выбрать вторую партию, далее произвести ее взвешивание. При этом на форме подбора партии будет видно, какие партии и в каком количестве (колонка "Набрано") были использованы в данной наборке.

- Получаем вес брутто с весов или вводим вручную, вес нетто рассчитается автоматически. При включенном автовзвешивании имеется возможность последовательно взвешивать материалы, не нажимая каждый раз кнопку на форме. При этом могут быть подключены одновременно несколько весов.

- Когда вес по рецептуре набран полностью, в ячейке "Всего" набранное количество выделяется зеленым цветом. 

- По завершении наборки ингредиентов нажимаем на кнопку **"Завершить"**:

![](SetOfMeatSets.assets/5.png)

Набранные материалы смешиваются на оборудовании или вручную, полученный полуфабрикат также необходимо взвесить.

- Выбираем строку задания, по которому выполнено смешивание ингредиентов, нажимаем на кнопку **"Приступить"**:

![](SetOfMeatSets.assets/6.png)

- Номенклатура сырья для комплектации уже выбрана в АРМ.

- Склад-получатель указывается автоматически, при необходимости его можно изменить, выбрав из списка.

- Сканируем штрихкод тары, в которой будет взвешиваться полуфабрикат, или выбираем номер тары из списка.

- Получаем вес брутто с весов, вес нетто рассчитается автоматически.

- По завершении взвешивания сырья для комплектации нажимаем кнопку **"Завершить"**:

![](SetOfMeatSets.assets/7.png)

- Выполненное задание в  АРМ выделяется зеленым цветом, состояние задания переходит в статус **"Выполнено"**:

![](SetOfMeatSets.assets/8.png)