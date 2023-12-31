Задача 1 (X_L6_T1)

Напишете програма, реализираща базов клас SchoolMember,  и производни класове Teacher и Student, като всеки от тях има атрибути име и възраст.

Обекти от класа Teacher освен това съхраняват информация за заплатата си и списък от курсовете, които преподават. Конструктурът на Teacher трябва да приема низ за име, години и заплата.

Да сe реализират следните методи:

getSalary(), който връща заплатата.

addCourse(), който приема два параметъра - сигнатура и име на курс и ги добавя в речник с ключ сигнатурата и стойност името на курса

getCourses(), който разпечатва всички курсове, по един на ред, първо сигнатурата, после интервал, после името.


Пример:

teacher = Teacher("Ivan", 40, 2500)

print(teacher.getSalary())

teacher.addCourse("MTH", "Math")

teacher.addCourse("PHY", "Physics")

teacher.addCourse("CHM", "Chemistry")

teacher.getCourses()


Изход:

2500

MTH Math

PHY Physics

CHM Chemistry

Обекти от класа Student съхраняват информация за курсовете, които са записали, годината, в която е записан всеки всеки курс и списък с оценки за всеки курс. Контсруктурът на Student приема име и възраст.

Да сe реализират следните методи:

attentCourse(), който приема сигнатура на курс и година и го добавя в речник с ключ сигнатурата и стойност друг речник, който съдържа ключове grades и year, и стойностите им са съответно списък с оценки и година на записване на курса.

addGrade(), който получава като параметри сигнатура и оценка и добавя оценката в съответния списък в речниковата стойност grades на курса с тази сигнатура. Методът извършва това само ако вече съществува курс с това име в речникът с курсове. В противен случай не прави нищо.

getCourses(), който разпечатва всички курсове, по един на ред, първо сигнатурата, после стойността като речник.

getAvgGrade(), който приема за входен параметър сигнатура на курс и връща средното аритметично за всичко оценки, съхранени в списъка с оценки.


Пример:

student = Student("Ivan", 18)

student.attendCourse("MTH", 2023)

student.attendCourse("PHY", 2023)

student.addGrade("MTH",5)

student.addGrade("MTH",2)

student.addGrade("MTH",5)

student.addGrade("PHY",6)

student.addGrade("CHEM",5)

student.getCourses()

print(student.getAvgGrade("MTH"))


Изход:

MTH {'grades': [5, 2, 5], 'year': 2023}

PHY {'grades': [6], 'year': 2023}

4.0


Задача 2 (X_L6_T2)

Траекторията на тяло, изстреляно под ъгъл А спрямо земната повърхност с начална скорост V се описва от следните две уравнения:

x = V * cos(А) * t
y = V * sin(A) * t − 1/2 * g * t^2

където t е времето в секунди, а g е земното притегляне.

Реализирайте клас Projectile, моделиращ снаряд, изстрелян във въздуха. Снарядът има маса, х и у координати. Реализирайте следните методи: 

конструктор с маса на снаряда и х координата (у е нула)

move(), който придвижва снаряда на време t и променя х и у

shoot() с параметри ъгъл и начална скорост, който вика move през 0.1 секунди, докато у-координата не стане 0. 

Нека програмата прави инстанция на такъв клас, като приема от потребителя ъгъл и начална скорост и след това извиква shoot. Текущите координати да се разпечатват във вид, удобен за внасяне в електронна таблица и изчертаването им.
