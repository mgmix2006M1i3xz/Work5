Домашнее задание к работе номер 4
Условие Задачи
Создать программу вычисления указанной величины. Результат проверить при заданных исходных значениях.
<img width="816" height="113" alt="image" src="https://github.com/user-attachments/assets/4d4f4a53-0eaa-4987-8e0c-f0df1a0d51bb" />

1. Алгоритм и блок-схема.
   Алгоритм:
1. Начало
2. Объявить переменные:
x — первое исходное значение;
y — второе исходное значение;
z — третье исходное значение;
3. term1 — первое слагаемое;
4. numerator — числитель;
5. denominator — знаменатель;
6. term2 — второе слагаемое;
7. w — результат вычисления.
8. Присвоить значения:
x = -2.235e-2;
y = 2.23;
z = 15.221.
9. Вычислить term1 = ∛(x⁶ + ln²y).
10. Вычислить numerator = e^|x−y| · |x−y|^(x+y).
11. Вычислить denominator = arctg(x) + arctg(z).
12. Вычислить term2 = numerator / denominator.
13. Вычислить w = term1 + term2.
14. Вывести значения x, y, z, w.
15. Конец.
    <img width="402" height="750" alt="image" src="https://github.com/user-attachments/assets/a4b694f9-de2d-4bbf-9144-197cf6cb0451" />

2. Реализация программы
#include <stdio.h> 
#include <math.h> 
#include<locale.h>

   int tast4() {
    double x = -2.235e-2;
    double y = 2.23;
    double z = 15.221;

    double term1 = pow(pow(x, 6) + pow(log(y), 2), 1.0 / 3.0);

    double numerator = exp(fabs(x - y)) * pow(fabs(x - y), x + y);

    double denominator = atan(x) + atan(z);

    double term2 = numerator / denominator;

    double w = term1 + term2;

    printf("Исходные данные:\n");
    printf("x = %.5f\n", x);
    printf("y = %.2f\n", y);
    printf("z = %.3f\n", z);
    printf("Вычисленное значение w = %.3f\n", w);

    return 0;
}
3. Результаты работы программы
Исходные данные:
x = -0.02235
y = 2.23
z = 15.221
Вычисленное значение w = 0.750
4. Информация о разработчике
Митин Михаил Александрович, бТИИ-261
