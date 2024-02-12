#Тестовое задание QA Близнов Даниил

##Общие вопросы:
1. По вашему - кто такой QA инженер?
QA инженер - это специалист, осуществляющее проверку программного продукта с целью обеспечения качества. Иными словами QA это звено между разработчиком и пользователем, отвечающее за качество конечного продукта.
2. Что такое тестирование?
Тестирование – это процесс, включающий в себя все элементы жизненного цикла, как статические, так и динамические, касающиеся планирования, подготовки и оценки программного продукта с целью определить их соответствие описанным требованиям, показать, подходят ли они для заявленных целей и определения дефектов.
3. Зачем вообще проводить проверку ПО?
Проверка ПО необходима для того, чтобы обнаружить баги на более раннем этапе и снизить затраты на их исправление. И основное, это удобство и корректная работа для конечного пользователя, для повышения доверия к компании.
##Логическая задача:
5 пиратов собираются разделить 100 золотых монет. Порядок пиратов определен – известно кто 1й 2й и так далее. По традиции пираты делят деньги следующим образом. 1й пират предлагает вариант деления денег. Все голосуют за или против этого варианта. Если голосов против более половины пирата убивают и следующий делит по тем же правилам. Когда дело касается денег каждый пират отлично умеют считать и поддержит предложенный вариант если он для него выгоднее чем альтернатива. Как 1му пирату получить максимально возможное количество денег и остаться в живых.

Ответ: Если начать решать задачу от большего к меньшему, то можно поделить эти 100 монет между первыми тремя пиратами, из расчёта 34 монеты получит первый, а 2-й и 3-й получат по 33 монеты. Такой ответ удовлетворяет обоим условиям задачи. 
Если же решать задачу с «конца», т.е. рассчитав, что 4-й и 5-й пират выкинут за борт первых трех. Тогда 100 монет заберет 4-й, а 5-й ничего не получит (такой расклад его не устроит).
Если же пираты останутся втроем, то 3-й пират может оставить себе 99 монет и отдать одну монету 5-му пирату, но такое условие не устроит 4-ого. 
Если же они убьют только первого пирата, соответственно 4 оставшихся могут поделить монеты так, что 2-й получит 99 монет, 4-й 1 монету, а 3-й и 5-й ничегог нее получат. Их голосов не хватит для перевеса. И, с условием, что первый пират уцелеет, то наиболее выгодно ему распределить монеты так: 98 – себе, 3-му и 5-му по одной монете, 2-му и четвертому ноль. Исходя из условий выше, это удовлетворит большинство пиратов.
##Задачи на тестирование:
1. Как протестировать сломанный тостер?
Нужно написать тест-кейс.
Тест-кейс #1: Проверка исправности сломанного тостера.
_Шаги:_
•	Вставить тостер в розетку
•	Вставить ломтики хлеба в камеры с прорезями 
•	Опустить пружину, загружающую хлеб в тостер
_Ожидаемый результат:_ Пружина не сработает. Хлеб не нагреется.
2. В приложении к тестовому заданию вы найдете 2 скриншота - реальное приложение (приложение №1) и макет (приложение №2). Найдите ошибки при реализации. Опционально - дайте рекомендации по улучшению.
Ответ: 
1. Надпись в верней части экрана о готовности карты в приложении не отражает действительный статус карты, как в макете.
2. В макете указано крайнее число для того, чтобы забрать карту, а в приложении указана дата готовности карты, но не указаны сроки хранения.
3. В приложении в отличии от макета вся информация не уместилась на экране, в т.ч. полный адрес и напоминание о том, что нужно взять паспорт. 
4. Надписи на нижних кнопках в макете и приложении отличаются. 

3.
 | № | Тестовые данные                          | Ожидаемый результат                                                                            | Фактический результат                                             |
|---|------------------------------------------|------------------------------------------------------------------------------------------------|-------------------------------------------------------------------|
| 1 |                   1+1+1                  |                                             3 (три)                                            |                              2 (два)                              |
| 2 |             3 разделить на 0             |                                  Деление на ноль не определено                                 |                   Деление на ноль не определено                   |
| 3 |   Девять целых девять десятых плюс 0,1   |                                           10 (десять)                                          |                     Данная операция не найдена                    |
| 4 |   Пятнадцать умножить на двадцать пять   |                                   375 (триста семьдесят пять)                                  |                    375 (триста семьдесят пять)                    |
| 5 | Одна целая две десятых разделить на семь |                 0,17142 (ноль целых семнадцать тысяч сто сорок две стотысячных)                |  0,17142 (ноль целых семнадцать тысяч сто сорок два стотысячных)  |
| 6 |              Минус один + 1              |                                            0 (ноль)                                            |                          -1 (минус один)                          |
| 7 |       Триста четыренадцать минус 14      |                                      Некорректный ввод (?)                                     |                   286 (двести восемьдесят шесть)                  |
| 8 |            пи умножить на 100            | 314,15926 (триста четырнадцать целых сто пятьдесят девять тысячных двадцать шесть стотысячных) | 314,159 (триста четырнадцать целых сто пятьдесят девять тысячных) |