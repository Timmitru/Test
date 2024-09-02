Для начала мы можем просуммировать все числа в переменную sm. Так мы получим самую большую сумму, которая может собраться в данном файле. Теперь решим вопрос с тем, чтобы данная сумма делилась на 89.
Узнаем из-за чего наша сумма не делиться на 89. Для этого найдем, на сколько эта сумма «перепрыгивает» за 89. Именно на сколько она больше, чем ближайшее число, делящееся на 89, так как полученную сумму мы можем только уменьшать, потому что она в принципе изначально самая большая возможная. Для этого найдём остаток от деления суммы на 89 и занесём результат в переменную lе.

Теперь наша задача сводится к тому, чтобы убрать наш «остаток от деления на 89», и постараться сделать уменьшение ранее найденной суммы минимальным

1 Часть. Проверим, сколько нужно убрать элементов из начала нашей цепочки, чтобы сумма убранных элементов содержала в себе тот самый остаток, который нам необходимо вычесть из суммы нашей последовательности.


Как только мы это найдём, в переменной sm1 будет сумма элементов, которые можно убрать из начала, чтобы сумма основной цепочки делилась на 89. В переменной k1 будет количество этих элементов.


2 Часть. Всё как в первой части, только теперь убираем элементы из конца основной цепочки.


3 Часть. Нам нужно убрать элементы, у которых сумма будет как можно меньше, ведь в основной цепочке сумма должна быть, как можно больше! После двух частей мы сохраним наименьшую сумму убранных элементов в переменную mn.

Мы можем убирать элементы и из начала, и с конца одновременно. Берём сначала один элемент из начала, а остальные с конца. Как только в сумме убранных элементов накопился необходимый остаток, проверяем, может этот результат и будет претендовать на ответ? Т.е. сравниваем сумму убранных элементов с переменной mn.

Если сумма больше, чем переменная mn, то она нас не интересует. Тогда берём два элемента из начала, а остальные с конца и продолжаем.

Если сумма убранных элементов меньше (и там есть нужная сумма остатка), то это значение перезаписывается в mn.

Затем, мы продолжаем третью часть до тех пор, пока сумма элементов, которые мы берём с начала, не превысит переменную mn. Ведь, если эта сумма превысит переменную mn, то мы точно не получим сумму убранных элементов меньшую, чем уже имеющийся результат.

4 часть. Делаем аналогично 3 части, только начало и конец меняем местами.

Итог 

Во всех частях учитываем, что, если сумма убранных элементов равна значению переменной mn, мы должны выбрать тот вариант, где количество убранных элементов, как можно больше, ведь нам нужна основная цепочка с наименьшим количеством элементов.

После того, как у нас выберется самый лучший вариант, мы должны от общего числа элементов отнять количество убранных элементов. Это и будет нашим ответом.
