Задача 1 (X_L5_T1)

Създайте рекурсивна функция за изчисляване на първите n числа на Фибоначи, и тяхното съхранение в списък. Реализацията трябва да съхранява вече изчислените стойности, така че когато рекурсивно извикване е с аргумент, който вече е изчислен, стойността да се взима директно, а да не се изчислява. Програмата да получава параметри от командния ред начално и крайно число позиция в редицата и да разпечатва списък с числата от редицата на Фибоначи, от началният до крайният индекс включително.

Примерен вход: 4 20  
Примерен изход: [2, 3, 5, 8, 13, 21, 34, 55, 89, 144, 233, 377, 610, 987, 1597, 2584, 4181]

Задача 2 (X_L5_T2)

Създайте рекурсивна функция, която при зададено число и степен, връща числото, повдигнато на степента. Програмата да получава параметри от командния ред число и степен и да изпечатва резултатът от повдигането на числото на съответната степен.

Примерен вход: 2 10  
Примерен изход: 1024

Задача 3 (X_L5_T3)

Напишете рекурсивна функция за двоично търсене в нареден списък. Програмата да получава параметър от командния ред число за търсене. Резултатът е един от следните два:  

**not found** - ако стойността не се намира в списъка  
**found at X** - ако първото срещане на търсената стойност в списъка е на позиция X

Списъкът за търсене да е статично описан в кода и да е следният: [30, 40, 50, 52, 56, 62, 70, 91, 100, 131, 132, 166, 170, 195, 202, 205, 212, 248, 249, 256, 263, 272, 288, 289, 290, 296, 332, 345, 352, 364, 380, 390, 407, 412, 429, 430, 438, 444, 486, 493, 497, 499, 510, 513, 514, 519, 521, 521, 535, 546, 552, 554, 556, 570, 584, 638, 640, 655, 655, 657, 692, 692, 711, 713, 731, 739, 740, 842, 858, 885, 887, 888, 893, 898, 900, 903, 908, 909, 959, 988]

Примерен вход: 88999999  
Примерен изход: not found

Примерен вход: 30  
Примерен изход: found at 0

Задача 4 (X_L5_T4)

Напишете рекурсивна функция, която връща дали даден символен низ е палиндром (дали низът и обърнатият символен низ са същите). Програмата да получава параметър от командния ред низ, за който да извърши проверката. Резултатът трябва да е True или False в завимиост от това дали входът е палиндром.

Примерен вход: level  
Примерен изход: True

Примерен вход: banana  
Примерен изход: False
