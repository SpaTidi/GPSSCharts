Доступные блоки:

GENERATE a,b,c,d,e,f
a,b,c,d,e,f - воспринимаются как единая строка
TERMINATE a
a - необязательный параметр
ADVANCE a,b
a,b - воспринимаются как единая строка
QUEUE a,b
a - название очереди
b - мест в очереди
DEPART a,b
a - название очереди
b - мест в очереди
SEIZE a
a - название устройства
RELEASE a
a - название устройства
ENTER a,b
a - название накопителя
b - единиц памяти
LEAVE a,b
a - название накопителя
b - единиц памяти
TRANSFER a,b,c
a - Вероятность или BOTH
b - блок с вероятностью перехода 1-a (если BOTH то транзакт, который проверяется первым)
c - блок с вероятностью перехода a (если BOTH то транзакт, который проверяется в случае если в b перейти не удалось)
MARK a
a - записать в этот параметр текущее значение таймера абсолютного времени
PRIORITY a
a - значение нового приоритета для транзакта
ASSIGN a*,b
a - номер параметра, который будет меняется
* - знак изменения(добавить(+),вычесть(-) и т.д.)
b - величина для модификации
SELECT x a,b,c,d,e,f
x - операция
a - номер параметра активного транзакта, в который запишется номер объекта удовлетворяющий условию
b - минимальный номер объекта, для которого проверяется условие
c - максимальный номер объекта, для которого проверяется условие
d - велечина для сравнения
e - СЧА типа объекта для режима отношения и выбора максимального или минимального
f - следующий блок
TEST x a,b,c
x - операция
a - переменная 1
b - переменная 2
с - Имя блока, для перехода если условие не выполняется
SPLIT a,b,c
a - число копий транзакта
b - метка блока, куда направляются копии
c - параметр, в котором запоминаются номера копий транзактов
MATCH a
a - имя блока, с которым нужно синхронизировать движение транзактов
ASSEBMLE a
a - счетчик, указывающий сколько членов одного семейства должны быть объединены
GATHER a
a - число транзактов, принадлежащих к одному семейству, которое нужно накопить
SAVEVALUE a,b
a - номер ячейки
b - присваеваемое значение
