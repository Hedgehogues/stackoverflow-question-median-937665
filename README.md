# [stackoverflow-question-937665](https://ru.stackoverflow.com/questions/937665/%D0%9F%D0%BE%D1%81%D1%87%D0%B8%D1%82%D0%B0%D1%82%D1%8C-%D0%BC%D0%B5%D0%B4%D0%B8%D0%B0%D0%BD%D1%83-%D1%81%D0%BF%D0%B8%D1%81%D0%BA%D0%B0-%D0%BF%D0%BE-%D1%83%D0%BD%D0%B8%D0%BA%D0%B0%D0%BB%D1%8C%D0%BD%D1%8B%D0%BC-%D0%B7%D0%BD%D0%B0%D1%87%D0%B5%D0%BD%D0%B8%D1%8F%D0%BC)
## Посчитать медиану списка по уникальным значениям

Есть исходный DF:

    com	x1
    1	5
    1	4
    1	3
    1	2
    1	4
    2	5
    2	6
    2	8
    2	3

Нужно посчитать дельту x1, а потом от всех дельт всех медиану для каждой позиции из com - в примере только две.

то есть на выходе нужно получить нечто такое:

    com	x1	delta	median
    1	5		-1
    1	4	-1	-1
    1	3	-1	-1
    1	2	-1	-1
    1	4	2	-1
    2	5		1
    2	6	1	1
    2	8	2	1
    2	3	-5	1

Пробовал через циклы, но опять же занимает очень много времени и выдает ошибку отсюда https://ru.stackoverflow.com/questions/937352/Ошибка-в-python-pandas-a-value-is-trying-to-be-set-on-a-copy-of-a-slice-from-a
