# Настройки учета в системе

Перед стартом работы в MES-системе следует задать настройки, которые будут влиять на дальнейшее прохождение учета всего
производства.

Эти настройки находятся в панели **"Настройка параметров учета"**:

![](SettingOfAccounting.assets/image.png)

## Вкладка "Основное"

- Основной график работы предприятия - указывается, по какому графику работает предприятие. Есть встроенный - общепринятый график работы на территории РФ;
- Контролировать остатки по производственным заданиям - включает/отключает контроль остатков по производственным заданиям. Нельзя выполнить сверх нормы по заданию (выпустить больше, чем указано), нельзя недовыполнить;
- Использовать штрих-коды складов для подтверждения перемещений - включает/отключает при перемещении продукции на определенный склад необходимость не только просканировать, ЧТО перемещаем, но еще и КУДА. Т.е. для склада будет задан свой штрих-код, учет перемещения на него требует сканирования данного штрих-кода;
- Вести учет по сменам - включает/отключает учет производства в несколько смен. Например, две смены - с 00:00 до 08:00 и с 08:00 до 24:00. Если отключен, то по умолчанию ведется учет по суточной смене: с 00:00 до 23:59;
- Вести учет по таре и местоположения тары - включает/отключает учет по тарам/контейнерам и т.п;
- Отключить использование стандартной формы ресурсных спецификаций - для работы с ресурсной спецификацией всегда будет открываться расширенная форма;
- Формировать итоговые документы за смену - включает/отключает формирование и видимость документа "Акт переработки" - сборный документ по всем выпускам и расходам за смену на рабочем центре с учетом жира и белка в продукции и сырье;
- Блокировать сырье на карантине - включает использование регистра "История карантина" и документов работы с карантином, запрещает использование сырья, помещенного на карантин. Подробнее в разделе "[Карантин](../../Quarantine/Quarantine.md)";
- Формат времени нормы хранения - ведет учет по норме хранения продукции на разных участках производства в часах или в минутах;
- Склад пересчета - склад, на который отправляются тары в случае инвентаризации, когда данные системы не сходятся с введенными пользователем данными о наличии тары на том или ином складе;
- Единица измерения веса; 
- Префикс штрихкодов узла РИБ - используется в случае распределенной базы для определения узла. 

![](SettingOfAccounting.assets/image-1.png)

## Вкладка "Себестоимость"

- Использовать расчет сырьевой себестоимости - включает возможность расчета в системе материально-сырьевой себестоимости;
- Использовать новый механизм расчета - для расчета себестоимости будет использован улучшенный алгоритм вычисления (рекомендуемая опция);
- Округлять значения до минимально допустимых - если не включена, при расчете будут игнорироваться значения меньше грамма или копейки; если включена, то значения будут округлены до минимально допустимых; 
- Вид цен себестоимость - вид цен, который используется для расчета материально-сырьевой себестоимости;
- Вид цен себестоимость при зацикливании - специальный вид цен, который используется для расчета себестоимости с том случае, если произошло зацикливание: ситуация, когда материал разузловался до производства из самого себя, например, упакованная продукция производилась из неупакованной, которая производилась из упакованной (переупаковка);
- Максимальная глубина разузлования - максимальное количество ступеней в цепочке разулования конечного продукта;
- Минимальный коэффициент разузлования - аналогично "округлять значения до минимально допустимых", используется для старого механизма расчета себестоимости.

![](SettingOfAccounting.assets/image-2.png)