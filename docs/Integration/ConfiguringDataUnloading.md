# Настройка выгрузки данных

Все объекты выгрузки находятся в подсистеме **"Обмен данными ИБ"** - **"Выгрузка"**.

[![1][1]][1]

## Заполнение настроек выгрузки

1. **Активные получатели**

    В регистре хранится список баз в которые происходит выгрузка данных.

    Если получатель создан, но не указан в регистре ***Активные получатели***, то данные в эту базу выгружаться не будут.

    В справочнике **"Внешние базы"** хранится информация о базах получателях и виде транспорта, с помощью которого данные выгружаются в базу приемник.

    Виды транспорта:

    - ***Встроенный*** – это обмен через http-сервис. Для него необходимо указать параметры подключения к базе приемнику: сервер, порт, имя публикации, пользователь и пароль для подключения к базе приемнику.
    - ***Datareon*** – обмен с использованием шины данных Datareon. Для использования необходимо встроить подсистему Datareon.

    [![2][2]][2]

2. **Правила выгрузки**

    Справочник **"Правила выгрузки"** содержит информацию о получателях, типах передаваемых пакетов, способах отбора, дате начала обмена.

    *Тип пакета* – это тип выгружаемых данных.

    Способов отбора может быть два:

    - Все объекты;
    - По условию - условия выгрузки прописываются в конфигураторе. На форму могут быть выведены какие-то дополнительные отборы. Например, список видов номенклатуры для выгрузки или список подразделений, по которым выгружаются документы и т.д..

    [![3][3]][3]

## Выгрузка данных

1. При записи объекта, для которого настроено правило выгрузки, он попадает в **"Объекты к выгрузке"**. В данном регистре хранится информация об объектах ИБ, дате,  виде транспорта. Также можно добавлять объекты по кнопке **"Добавить"**.

1. Затем нужно обработать *"Объекты к выгрузке"* в соответствии с правилами выгрузки либо кнопкой **"Добавить в очередь"** из формы списка, либо с помощью регламентного задания **"Обмен данными ИБ: Маршрутизация исходящих пакетов"**.

    [![4][4]][4]
    [![5][5]][5]

1. Обработанные объекты попадают в регистр **"Очередь исходящих пакетов"**. Если объект не удовлетворяет условиям ни одного из правил, то он удаляется из **"Объектов к выгрузке"** и не попадает в **"Очередь исходящих пакетов"**.

    В регистре **"Очередь исходящих пакетов"** хранится информация о получателях, УИДах пакетов данных, Объектах ИБ, Типах пакетов, Правилах, Приоритетах, датах и хешах объектов ИБ.

    - Тип пакета – тип данных ИБ;
    - Получатель – база, в которую будут отправлены данные. При этом, если для данного *Типа пакета* существуют правила для нескольких приемников, то в **Очереди исходящих пакетов** будет столько строк для данного Объекта ИБ, сколько активных получателей указано в правилах выгрузки;
    - Пакет данных УИД – УИД пакета данных, который представляет собой строку в формате json, содержит в себе все данные для выгрузки по Объекту ИБ;
    - Правило – правило выгрузки, по которому был обработан Объект ИБ и сформирован пакет данных для выгрузки.

    [![6][6]][6]

2. Далее объекты из **"Очереди исходящих пакетов"** базы источника передаются в **"Очередь входящих пакетов"** базы приемника. Это осуществляется либо по кнопке **"Отправить"** из формы списка **Очереди исходящих пакетов**, либо с помощью регламентного задания **"Обмен данными ИБ: Отправка исходящих пакетов"**.

    [![7][7]][7]

    Если выгрузка произошла корректно, то строка из **"Очереди исходящих пакетов"** исчезнет. В противном случае – отобразится информация об ошибке. Информация о всех выгруженных пакетах хранится в **"Журнале исходящих пакетов"**, в том числе текст ошибки.

    [![8][8]][8]

[1]: ConfiguringDataUnloading.assets/1.png
[2]: ConfiguringDataUnloading.assets/1.gif
[3]: ConfiguringDataUnloading.assets/2.gif
[4]: ConfiguringDataUnloading.assets/3.gif
[5]: ConfiguringDataUnloading.assets/2.png
[6]: ConfiguringDataUnloading.assets/3.png
[7]: ConfiguringDataUnloading.assets/5.gif
[8]: ConfiguringDataUnloading.assets/4.png
