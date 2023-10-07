# Навигатор
-[Обзор демаскирующих сигналов БПЛА](#Обзор-демаскирующих-сигналов-БПЛА)

-[Обзор способов обнаружения БПЛА](#Обзор-способов-обнаружения-БПЛА)

-[Оптико-электронные средства обнаружения](#Оптико-электронные-средства-обнаружения)
 
-[Акустические средства обнаружения](#Акустические-средства-обнаружения)

-[Славная таблица со славным сравнением способов обнаружения](#Славная-таблица-со-славным-сравнением-способов-обнаружения)

-[Детальное рассмотрение методов обнаружения](#Детальное-рассмотрение-методов-обнаружения) 
 
-[Литература и статьи](#Литература-и-статьи) 
 
  
# Обзор демаскирующих сигналов БПЛА  
- сигналы радиолокационной станции (РЛС), отраженные от корпуса и агрегатов БВС, в том числе проявление в отраженном сигнале эффекта доплера
- команды и ответные сигналы канала управления между пультом управления и БВС, а также между БВС и спутником-ретранслятором системы навигации
- каналы обмена информацией (канал управления, передачи телеметрии и видеоинформации)
- сигналы системы автоматической посадки
- собственное электростатическое поле за счет трения БВС о воздух 
- отражение в оптическом диапазоне 
- инфракрасное излучение (тепловое поле двигателя)
- акустическое поле винта и двигателя (может отсутствовать при планировании) 

# Обзор способов обнаружения БПЛА
## Применение РЛС в качестве средства обнаружения
Эффективность применения зависит от множества факторов таких как: размер БПЛА, высота полета, рельеф местности, наличие сильно отражающий объектов вокруг РЛС. К недостаткам РЛС можно отнести ослабление радиоизлучения высокого частотного диапазона дождем, туманом или иными осадками. частицы воды рассеивают и поглощают часть электромагнитной энергии, излучаемой РЛС, что приводит к уменьшению дальности обнаружения объектов. использование же низкочастотных РЛС (ниже дециметрового диапазона) не позволяет обнаружить настолько малые цели. Так же стоит заметить, что большинство БПЛА в настоящее время производят полет по заранее загруженной программе без вмешательства оператора. Следовательно, РЛС не поймает никаких сигналов взаимодействия оператора с БПЛА в силу их отсутствия. Использование пластиковых и композитных материалов в конструкции БПЛА так же понижают излучаемые им сигналы.

Применение радиолокационных систем, позволяет повысить дальность обнаружения БПЛА до единиц километров, при этом качество их работы не зависит от времени суток и погодных условий, что выгодно их отличает от акустических и оптических средств. Помимо выявления, радиолокаторы позволяют определить направление и дальность до приближающегося дрона, однако неспособны определить тип обнаруженного объекта и как следствие, подвержены ложным срабатываниям.

## Радиочастотное обнаружение
По характерным радиосигналам БПЛА могут быть обнаружены радиотехническими средствами обнаружения (РТСО) путем приема и анализа сигналов. Причем для этого установка должна обладать базой с характерными радиосигналами БПЛА, чтобы в дальнейшем оперируя ими детектить угрозы.

Важным преимуществом является то, что РТСО позволяет выделять идентифицировать БПЛА среди естественных объектов. Тем не менее есть и недостатки: РТСО могут с хорошей точностью определить общее направление БПЛА, а вот высота и дальность цели определяется с существенными погрешностями. Кроме того БПЛА полностью в автономном режиме РТСО не обнаруживает. В случае, если с БПЛА ведется обмен данными, то в результате такого обмена возникает высокоинтенсивное излучение, которое является основным демаскирующим признаком.

### Итог для РЛС и РТСО
В целом можно сделать вывод, что данные методы подходят для обнаружения БПЛА на расстояниях порядка километров при этом с приемлемой точностью

Однако использование таких методов не позволяет узнать тип БПЛА, его высоту и скорость. Также важную роль играет рельеф местности, на которой проиходит детектирование

## Оптико-электронные средства обнаружения
Сразу стоит отметить, что данные способы обнаружения существенно зависят от погодных условий. В ночное время, например, необходимо наличие подсветки для точной идентификации БПЛА. Если охватывать широкий диапазон местности для обзора, то дальность обнаружения будет в среднем от 150м до 600м. Поэтому для увеличения дальности обнаружения зоны обзора уменьшаются, что приводит к увеличению времени поиска. Однако в комбинации с РЛС возможно эффективное использование, РЛС будет находить направление БПЛА, а уже с помощью оптический средств можно будет выйти на наблюдение самого объекта. Для обнаружения БПЛА возмодно применение оптико-электронных устройств, работающих в ближнем ИК-диапазоне.

### ИК-видеокамера с подсветкой
Принцип работы заключается в считывании отраженного от объекта ИК-излучения, формируемого подсветкой. Работают в ближнем ИК-диапазоне (0,78-3 мкм). Недостаток заключается в том, что в случае неблагоприятных погодных условий (осадки, задымленность и т.п) ИК-излучение рассеивается и поглощается

### Тепловизоры
Не требуют подсветки. Тепловизор принимает волны, исходящие от объектов различной температуры, что приводит к формированию теплового изображения на матрице. Тепло от БПЛА в основном выделяется от силовой установки, а также точками торможения на несущих краях крыльев, пропеллеров и винтов. Материалы с высокой теплопроводимостью (серебро, алюминий) могут стать причиной появления дополнительных зон с повышенным температурным контрастом с окружающей средой, что может изменить изображение БПЛА на матрице тепловизора в результате чего алгоритм разпознавания может некорректно отработать.

### Лидары
Метод лазерной детекции в основе которого положена технология получения и обработки информации об удаленных объектах с помощью активных оптических систем (лидаров), использующих явления поглощения и рассеивания света в оптически прозрачных средах. Лидар представляет собой дальномер оптического диапазона. Не рекомендован как основное средство обнаружения.

#### Итог для оптико-электронных средств
Малая дистанция обнаружения и зависимость от погодных условий является существенных недостатком данных методов. Тем не менее они позволяют определить и тип, и скорость БПЛА. 

## Акустические средства обнаружения
В полете БПЛА генерирует звуковые волны, источниками которых являются двигательные установки и лопасти воздушных винтов. Частота генерируемого звука кратна частоте выхлопа горячих газов, количеству и частоте вращения лопастей воздушного винта. Интенсивность звука зависит от скорости обтекания лопастей

К достоинства данного метода можно отнести следующее:
- Обеспечивает автоматическое обнаружение низкоскоростных маловысотных БПЛА в любых погодных условиях
- Являются пассивными средствани обнаружения. В силу этого сохраняют работоспособность даже при радиоэлектронных помехах
- Имеют малые габариты и низкое энергопотребление

При этом из недостатков можно выделить следующее:
- Низкая точность определения местоположения БПЛА
- Среди рассмотренных методов данный имеет самую низкую дальность обнаружения малых БПЛА, особенно если они используют электродвигатель

### Итог для акустических методов
Как по мне, то это идеальный метод обнаружения в плохих погодных условиях. Также стоит выделить размеры и потребление акустических средств. Тем не менее непригодность в обнаружении малых БПЛА и низкая точность в определении местоположения БПЛА делают данные методы очень ненадежными, если использовать их в качестве основных

# Славная таблица со славным сравнением способов обнаружения
![image](https://github.com/DeSauzzz/Drone_detectio/assets/145459536/52fce36f-1e3b-487b-852a-bd8919a9b2b3) 

# Детальное рассмотрение методов обнаружения
## Рассмотрение РЛС как средства обнаружения
Физической основой радиолокации является рассеяние радиоволн объектами, отличающимися своими электрическими характеристиками от соответствующих характеристик окружающей среды при их облучении. Интенсивность вторичного поля зависит от степени отличия электрических характеристик объекта и среды, а также от формы объекта и его размеров. Результирующее электромагнитное поле состоит из поля отражения, распространяющегося в сторону первичного излучения и от теневого поля, распространяющегося за объект т.е в ту же сторону, что и первичное излучение.

С помощью приемной антенны и приемного устройства (Прм) можно принять часть рассеянного сигнала, преобразовать и усилить его для последующего обнаружения. Таким образом, простейшая РЛС может состоять из передатчика (Прд), формирующего и генерирующего радиосигналы, передающей антенны, излучающей эти радиосигналы, приемной антенны, принимающей отраженные сигналы, радиоприемника, усиливающего и преобразующего сигналы и, наконец, выходного устройства (ВУ), обнаруживающего отраженные сигналы.

Амлитуда (мощность) принимаемого сигнала мала, а сам сигнал имеет случайный характер. Малая мощность сигнала объясняется большим расстоянием до цели и поглощением энергии сигнала при его распространении. Также на интенсивность отраженного сигнала существенно влияют размеры целей. Случайный характер сигнала является следствием флуктуации отраженного сигнала за счет случайного перемещения элементов цели сложной формы при отражении радиоволн. Результатом данных факторов является то, что принимаемый сигнал по виду и интенсивности похож на шумы и помехи. Исходя из этого можно заключить, что основной задачей РЛС является обнаружение полезного радиосигнала, т.е. вынесения решения о присутствии полезного сигнала в поступающей на вход приемного тракта смеси полезного сигнала с помехами. Для этого используется специальное устройство - обнаружитель, в котором пытаются использовать алгоритм оптимального обнаружения.

На рисунке ниже представлен способ работы простейшей РЛС:
![image](https://github.com/DeSauzzz/Drone_detectio/assets/145459536/2975d5ab-37be-4fde-92b3-a70420fe2c8b)

Передатчик формирует мощные высокочастотные колебания. В зависимости от того, какая антенна используется в РЛС, может быть реализован в модельном варианте и встроен в активную ФАР (фазированную антенную решетку), либо в виде модулятора и однокаскадного или многокаскадного генератора радиочастоты для пассивной ФАР. Приемник обеспечивает прием, обработку и выделение информации из принятого сигнала. Короткие зондирующие импульсы через антенну излучаются в 
пространство. При наличии на пути распространения радиоволн объекта часть электромагнитной энергии отражается обратно в сторону РЛС. Отраженный сигнал через антенну поступает в приемник, усиливается и поступает в выходное устройство для индикации и (или) обработки (обнаружитель, измерители).

Построение РЛС на базе современных технологий обработки информации заключается в следующем:
- в использовании в качестве антенн фазированной антенной решетки 
(ФАР), работающей на передачу и прием сигналов
- в качестве генератора пусковых импульсов синтезатора частоты используется синхронизатор, регламентирующий во времени порядок работы и взаимодействия основных блоков РЛС
- в качестве выходного устройства используется цифровой процессор

Абстрактная схема такой РЛС представлена ниже:
![image](https://github.com/DeSauzzz/Drone_detectio/assets/145459536/cd96bd63-b8a1-47bf-8606-bed0cadaf98b)


### Виды радиолокации
- Пассивная радиолокация исследует собственное излучение (тепловое, электромагнитное и т.п.), которое генерирует цели (ракеты, самолеты, космические объекты).
- Активная с активным ответом осуществляется в случае, если объект оборудован собственным передатчиком и взаимодействие с ним происходит по алгоритму "запрос - ответ".
- Активная с пассивным ответом предполагает исследование вторичного (отраженного) радиосигнала. Радиолокационная станция в этом случае состоит из передатчика и приемника.
- Полуактивная радиолокация - это частный случай активной, в случае когда приемник отраженного излучения расположен вне РЛС (например, является конструктивным элементом самонаводящейся ракеты).

### Классификация по характеру размещения
По характеру размещения частей аппаратуры в пространстве различают однопозиционные, двухпозиционные (бистатические) и многопозиционные РЛС. Последние два типа РЛС отличаются тем, что их аппаратура разнесена в пространстве, и эти РЛС могут функционировать как самостоятельно, так и совместно (разнесенная радиолокация). Благодаря пространственному разнесению элементов в таких системах достигаются большие информативность и помехозащищенность, однако сама система усложняется.

Однопозиционные радиолокационные системы (ОПРЛС) отличаются тем, что вся аппаратура располагается на одной позиции. В ОПРЛС реализуется активный или пассивный вид радиолокации.

Бистатические радиолокационные системы (БиРЛС) представляют собой РЛС, в которых передающая и приемная части расположены в различных точках пространства. Такие БиРЛС основаны на  активном виде радиолокации.

### Факторы, влияющие на характеристики и эффективность работы РЛС
Эффективность работы РЛС можно оценить по следующим факторам:
- Максимальная дальность действия
- точность измерения расстояния до цели и ее азимута
- возможность различения нескольких целей
- возможность обнаружения отраженного от цели сигнала при наличии помех от местных предметов, мешающих сигналов и в условиях применения противником средств радиоэлектронного подавления (РЭП)
- боевая и эксплуатационная готовность, надежность и ремонтопригодность радиолокационного оборудования
Рассмотрим основные факторы, влияющие на эффективность РЛС чуть более детально.

#### Несущая частота радиопередатчика
Более высокие частоты увеличивают разрешающую способность при обнаружении целей, позволяют обнаруживать цели меньшего размера и использовать антенны меньшего размера. В то же время, с увеличением частоты
увеличивается затухание сигнала, а значит и максимальная дальность действия радиолокационной системы.

#### Импульсная мощность
дальность действия РЛС увеличивается при увеличении мощности в импульсе. Простой расчет показывает, что при удвоении мощности в импульсе дальность действия увеличивается на 25%. В то же время, это приводит к тому, что для увеличения дальности приходится использовать оборудование большего размера и большей мощности. 

#### Физические размеры антенны
точность и дальность действия РЛС зависит от коэффициента усиления и эффективной площади антенны, которые, в свою очередь, зависят от физических размеров антенны. Иногда стационарные антенны РЛС бывают очень большими. Например, антенны загоризонтных РЛС декаметрового диапазона имеют длину более километра. Параболические полноповоротные антенны диаметром и более 70 м тоже не являются чем-то необычным. Однако бывают ситуации, когда практический размер антенны ограничен. Например — в авиации.

#### Форма импульса
Импульсы, излучаемые радиолокационными станциями, должны иметь короткие фронты, чтобы обеспечить лучшую точность определения дальности до цели. В то же время, для обеспечения хорошей формы импульсов требуется более широкая полоса пропускания, а значит более сложное, дорогое и энергоемкое оборудование.

#### Длительность импульса
Чем больше длительность (ширина) импульса, тем больше дальность действия РЛС, потому что в каждом импульсе можно передать больше энергии. В то же время, короткие импульсы обеспечивают меньшую минимальную дальность действия и более высокую точность определения расстояния до цели.

#### Частота повторения импульсов
Временной интервал между соседними излученными импульсами определяет частоту повторения импульсов. Чем выше частота повторения импульсов, тем меньше максимальная дальность действия РЛС и тем лучше точность измерения дальности и разрешение по азимуту. Между двумя импульсами должно пройти достаточно времени, чтобы отраженный сигнал мог вернуться к цели и не был заблокирован следующим передаваемым импульсом.

#### Ширина диаграммы направленности антенны
Более узкий луч обеспечивает большую угловую точность и большую дальность действия РЛС. В то же время, сужение диаграммы направленности антенны приводит к уменьшения числа оборотов антенны, что, в свою очередь, приводит к увеличению времени обнаружения цели.

#### Чувствительность и шумовые характеристики приемного тракта РЛС
Чувствительность приемного тракта РЛС определяется шумом приемника. Более чувствительные приемники обеспечивают большую дальность действия. Однако для увеличения чувствительности требуется более сложное и дорогое оборудование.

#### Размеры цели
Размер цели, видимый радиолокатору, называется эффективной площадью рассеяния цели. Обычно эта величина не связана с физическими размерами цели. Она зависит от геометрии цели, а также от того, насколько хорошо материал цели поглощает электромагнитную энергию радиоволн и превращает их в тепловую энергию.

#### Математическое обоснование 
Мощность отраженного от цели сигнала $P_{r}$ на приемной антенне определяется по формуле:

$$ P_{r} = {P_{t}G_{t}A_{r}F^4\sigma \over (4\pi^2)R_{t}^2R_{r}^2} $$

где
$G_{t}$ - коэффициент усиления передающей антенны
$P_{t}$ - мощность излученного сигнала
$\sigma$ - эффективная площадь рассеивания цели
$F$ - коэффициент потерь при распространении сигнала. В вакууме и без помех этот коэффициент равен 1
$R_{t}$ - расстояние от передающей антенны до цели
$R_{r}$ - расстояние от цели до приемной антенны
$A_{r}$ - эффективная площадь антенны

Эффективная площадь приемной антенны можно выразить как
$A_{r} = {G_{r}\lambda^2 \over 4\pi}$

где $\lambda$ - длина волны передаваемого сигнала, $G_{r}$ - коэффициент усиления приемной антенны. Поскольку $f = {c \over \lambda}$ то:

$A_{r} = {G_{r}c^2 \over 4\pi*f^2}$

Опуская ряд вычислений получим итоговую формулу для определения максимальной дальности действия РЛС:

$R = \sqrt[4]{(P_{t}G^2c^2\sigma \over (4\pi)^3f^2P_{r})}$

### Общий итог для РЛС
Исходя из всего вышесказанного можно определить какими преимуществами и недостатками обладает РЛС как средство обнаружения БПЛА.
#### Примущества
- _Дальность обнаружения БПЛА измеряется в единицах километров_- из математических расчетов выше и анализа факторов, влияющих на эффективность работы РЛС можно заключить: дальность действия РЛС можно увеличить путем добавления более мощных компонентов. Так, например, комплекс "Бук-М3" способен засекать цели на расстоянии не менее 120км.
- _Способность определять расстояние до цели_ - путем математических расчетов можно не только обнаружить цель, но и определить расстояние до нее по разнице времени между испущенным импульсом и полученным.
- _Наименьшая подверженность погодным условиям_ - безусловно, осадки и прочие атмосферные явления снижают эффективность РЛС. Однако при этом сигнал отраженный от цели все еще будет доходить до цели и поступать в отраженном виде на приемник. Пусть и на меньшем расстоянии.
- _Многовариативность_ - поскольку существует несколько видов радиолокации, то исходя из них можно спроектировать РЛС, работающую на каждом из этих видов. Это существенно увеличивает количество доступных вариаций РЛС.

#### Недостатки
- _Громоздкость_ - в случаях увеличения дальности действия установки РЛС приобретают коллосальные размеры. Например загоризонтные РЛС обладают антенной, у которой радиус превышает километр
- _Невозможность определить тип цели_ - обнаружения цели и расстояние до нее полезная информация, но РЛС не способны дать понимание того, какая именно цель летит в вашу сторону, поскольку по полученному радиосигналу невозможно определить вид цели.
- _Композитные материалы в БПЛА_ - композитные материалы снижают отражательную способность тела, что ведет к невидимости этого тела для РЛС на расстояниях, при которых, согласно расчетам, РЛС должна действовать.
- _Возможность подавления_ - средства РЭБ способны понизить эффективность РЛС путем излучения мощных сигналов, которые создают помехи
- _Влияние рельефа местности_ - отражаясь от поверхности радиосигналы теряют свою энергию, поэтому в условиях, где много естественных преград, сигнал либо полностью рассеивается так и не дойдя до цели, либо дойдя до цели не создает достаточного вторичного излучения, которое смог бы зафиксировать приемник.

## Рассмотрение оптико-электронных средств обнаружения
### ИК-камеры
Это устройство, которое способно считывать инфракрасное излучение, не видное глазу человека. Принцип работы заключается в следующем: объекты излучают в инфракрасном диапазоне, а камера фиксирует это излучение и траслирует его на дисплей. Так как БПЛА тоже излучают в ИК-диапазоне, то ИК-камеры могут быть одним из средств их обнаружения.
#### Преимущества ИК-камер
- _Возможность использования в ночное время суток_ - поскольку тепловая карта тела не зависит от того, днем она сделана или ночью.
- _Компактность_ - сами по себе ИК-камеры обладают небольшими размерами, следовательно, они могут использоваться как портативное средство обнаружения.
- _Возможность обнаружения низколетящих БПЛА в рельефной местности_ - в случае, когда радиоволны не смогут дать ответа на вопрос о наличии цели в, например, горной местности, можно использовать ИК-камеры, которые с легкостью зафиксируют тепловую сигнатуру и определять цель. 
#### Недостатки ИК-камер
- _Зависимость от погодных условий_ - в тумане, дожде и прочих атмосферных явлениях ИК-излучение ослабляется в результате рассеивания и поглощения.
- _Невозможность определить тип цели_ - по полученной тепловой карте не предоставляется возможным определить тип БПЛА, который был зафиксирован.
- _Малая дальность действия_ - так как получить изображение можно только при непосредственном оптическом контакте с обнаруженной целью.
- _Плохая фиксация объектов с низкой температурой_ - для производства беспилотников могут быть использованы материалы, которые плохо излучают в ИК-диапазоне, что не позволит точно зафиксировать цель на камере.
### Лидары
Лидар - это технология измерения расстояний с помощью светового луча. Принцип действия схож с РЛС, различие в том, что вместо радиоволн испускается свет. Это, например, дает преимущество при малых размерах цели, поскольку радиоволны зависят от этих размеров, а свет - нет. Лидар посылает световую волну (как правило, в инфракрасном диапазоне), она отражается от объекта и возвращается. Анализируя время или отраженный сигнал можно рассчитать расстояние до объекта. Различают импульсный и фазовый методы измерения дальности. При импульсном методе к объекту посылается импульс, параллельно которому устройство запускает внутренний счетчик. Когда отраженный луч возвращается, он останавливает работу счетчика. После этого микропроцессор с использованием времени счетчика по формуле рассчитывает расстояние до объекта. В таком случае математическое обоснование данного метода таково:
$L = {ct \over 2}$
где $с$ - скорость света; $t$ - разница во времени между испущенным импульсом и принятым.
При фазовом методе излучение модулируется по синусоидальному закону, а отраженный луч смещается по фазе. На основе разницы в фазе и определяется расстояние.
$L = {c\phi \over 2f\pi}$
где $f$ - частота модуляции; $\phi$ - фазовый сдвиг; $c$ - скорость света.

Лидар можно использовать не только для замера расстояния до цели, но и для построения 3D-карт. В случае замера расстояния используется единичные импульсы, а при построении карт отправляют пучки импульсов.
#### Преимущества
- _Возможность обнаружения малых целей_ - как и было оговорено, свет не зависит от размеров цели, поэтому отправленный импульс будет зафиксирован в отраженном виде приемником.
- _Меньшее рассеяние в атмосфере_ - свет незначительно рассеивается в атмосфере. Теряется примерно 1,3% интенсивности на 1км.
- _Возможность получения детального изображения цели_ - использование многочисленных пучков света после их фиксации в отраженном виде на приемнике позволяет увидеть тепловую карту цели, исходя из которой можно определить размер цели.
- _Возможность узнать точное расстояние до цели_ - испуская единичный импульс можно определить расстояние до цели.
- _Можно использовать в ночное время суток_ - в силу того, что испускается свет для обнаружения цели, то для нас не важно день сейчас или ночь

#### Недостатки
- _Невозможность опрелелить тип цель_ - на основе полученного теплового изображения можно определить тип цели только косвенно, опираясь на внешний вид цели, согласно изображению.
- _Генерация большого объема материла_ - системы LIDAR генерируют большие объемы материалов, из-за чего требуют больших вычислительных ресурсов для их обработки.
- _Влиялие погодных условий_ - сильные дожди или снег способны снизить эффективную работу систем LIDAR

### Общий итог для оптико-электронных средств
Данные средства являются компактными, благодаря этому они могут использоваться не только на одной точке, но и могут быть перевезены без особых проблем на другую точку. Благодаря системам LIDAR и ИК-камерам можно получить примерное изображение цели, по которому можно косвенно понять тип цели и используемое вооружение. Свет меньше рассеивается в атмосфере, что несколько понижает влияние погодных условий на эффективность работы. Тем не менее ИК-камеры и лидары имеют меньший обзор по сравнению с системами РЛС. В случае лидаров это обусловлено тем, что испускаются единичные импульсы для определения расстояния до цели в определенном направлении.


# Литература и статьи
https://www.astrosoft.ru/articles/radar/obnaruzhenie-dronov-s-pomoshchyu-rls-s-mimo-i-ofdm/ - Обнаружение дронов с помощью РЛС с MIMO и OFDM

https://www.secuteck.ru/articles/aktualnost-vybora-metodov-obnaruzheniya-malyh-bespilotnyh-vozdushnyh-sudov-grazhdanskogo-klassa - вот тут нормас так способы обнаружения расписаны
