# Исследование объявлений о продаже квартир

По представленным данным сервиса Яндекc Недвижимость (архив объявлений о продаже квартир в Санкт-Петербурге и соседних населённых пунктах за несколько лет), необходимо выявить параметры, которые влияют на цену недвижимости. Это позволит построить автоматизированную систему: она отследит аномалии и мошенническую деятельность. 

По каждой квартире на продажу доступны два вида данных. Первые вписаны пользователем, вторые получены автоматически на основе картографических данных.

В таблице находится 22 столбца, 23 699 строк.

Для исследования использовалась библиотека Pandas.

В ходе исследования была проведена предобработка данных. В учебных целях предобработка производилась особо тщательно (с заменой экстремальных значений с помощью функций). Были созданы дополнительные столбцы в исходной таблице (цена квадратного метра, день недели, месяц и год публикации объявления, категория этажа, соотношение жилой и общей площади и отношение площади кухни к общей), проведён исследовательский анализ данных.

**Выводы:**
* Самый значимый фактор, влияющий на стоимость объектов недвижимости - это их площадь. Цена квадратного метра влияет на общую цену объекта недвижимости несколько меньше - и это не удивительно с учётом многих других факторов.

* Значимое влияние на стоимость квартиры в целом и на стоимость квадратного метра оказывает то, на каком этаже находится квартира: первый и последний существенно "сбавляют" цену.

* Удалённость от центра в некоторой степени влияет на стоимость квартир: объекты в центре в среднем почти в два раза дороже, чем в среднем по выборке. При этом они обладают и другими положительными характеристиками, прежде всего, большей площадью, а также большей высотой потолков, большим количеством комнат.

* Рынок недвижимости чутко реагирует на общую ситуацию в экономике, поэтому кризис служит предиктором снижения стоимости объектов. Необходимо заметить при этом, что цена квадратного метра восстанавливается быстрее, чем общая стоимость объектов (видимо, покупатели начинают предпочитать квартиры меньшей площади).

* На стоимость как объектов целиком, так и квадратного метра в некоторой степени влияет сезонность. Обобщая данные, можно говорить о том, что в период высокой деловой активности осенью цены несколько выше, чем весной и, особенно, в декабре. Кроме того, более дорогие объекты начинают продавать по вторникам и средам, а по субботам размещают, по всей видимости, больше объявлений о продаже загородных домов. 

* Влияние различных факторов на стоимость квартир в самом центре Санкт-Петербурга чуть менее выражено, чем в среднем по выборке, площадь остаётся определяющим предиктором цены квартиры. Интересной особенностью является то, что в 2018-2019 годах, когда в целом в Петербурге наметился рост цен на недвижимость, в центре продолжалось снижение средней цены объекта.
