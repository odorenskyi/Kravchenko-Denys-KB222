# Лабораторна робота № 8

Тема реалізація статичних бібліотек модулів лінійних обчислювальних процесів.

Мета полягає у набутті ґрунтовних вмінь і практичних
навичок застосування теоретичних положень методології модульного
програмування, реалізації метода функціональної декомпозиції
задач, метода модульного (блочного) тестування, представлення
мовою програмування С++ даних скалярних типів, арифметичних і
логічних операцій, потокового введення й виведення інформації,
розроблення програмних модулів та засобів у кросплатформовому
середовищі Code::Blocks (GNU GCC Compiler). 

Завдання
1. Реалізувати статичну бібліотеку модулів libModulesПрізвище
C/C++, яка містить функцію розв’язування задачі 8.1.

Задача 8.1 За значеннями x, y, z обчислюється S:

#include <iostream>
#include <Math.h>
#include <Math.h>
#define _USE_MATH_DEFINES
#include <cmath>

// Змінна x, y, z не повинні бути від'ємними

unsigned long x, y, z;

using namespace std;

double my_function(double, double, double);
int main()
{
   double S, x, y, z;
    cout << "x="; cin >> x;
    cout << "y="; cin >> y;
    cout << "z="; cin >> z;
    S=my_function (x, y, z);
    cout << "S=" << S;
    return 0;
}
double my_function(double x, double y, double z){
    if (x < 0){
        std::cout << "";
    }
double s;
double radians;
radians = (z * M_PI) / 180;
s = pow(z+y+z,2)- sqrt(abs(2*M_PI*sqrt(1/2*z)/y + 4*(pow(x,3 + cos(radians)))));
return s;
}


2. Реалізувати програмне забезпечення розв’язування задачі 8.2 —
консольний застосунок. 

Задача 8.2 За послідовними запитами вводяться числа x, y, z та символи a і b.
8.2.1 Прізвище та ім’я розробника програми зі знаком охорони авторського права «©»

#include <iostream>
using namespace std;

void printAuthorInfo() {
    int x, y, z;
    char a, b;

    // Ввід чисел та символів
    cout << "Введіть числа x, y, z: ";
    cin >> x >> y >> z;

    cout << "Введіть символи a та b: ";
    cin >> a >> b;

    // Виведення прізвища та імені автора
    cout << "© Розробник програми: Кравченко Денис" << endl;
}

int main() {
    printAuthorInfo();
    return 0;
}


8.2.2 Результат логічного виразу в числовому вигляді (1/0):
A+1<b ?

#include <iostream>

using namespace std;

int main() {
    int x, y, z;
    char a, b;

    // Запитуємо користувача числа x, y, z та символи a і b
    cout << "Enter x: ";
    cin >> x;

    cout << "Enter y: ";
    cin >> y;

    cout << "Enter z: ";
    cin >> z;

    cout << "Enter a: ";
    cin >> a;

    cout << "Enter b: ";
    cin >> b;

    // Обчислюємо логічний вираз a+1<b
    bool result = (a + 1 < b);

    // Виводимо результат у числовому вигляді
    cout << "Result: " << result << endl;

    return 0;
}


8.2.3 Значення x, y, z в десятковій і шістнадцятковій системах числення; S, що обчислюється функцією s_calculation() Заголовкового файлу Modules.Прізвище.h

#include <iostream>
#include <iomanip>
#include "modulesLastname.h" // Заголовковий файл з функцією s_calculation()

using namespace std;

int main() {
    int x, y, z;
    char a, b;
    cout << "Enter x, y, z: ";
    cin >> x >> y >> z;
    cout << "x = " << x << " (hex: " << hex << x << ")" << endl;
    cout << "y = " << y << " (hex: " << hex << y << ")" << endl;
    cout << "z = " << z << " (hex: " << hex << z << ")" << endl;
    cout << "Enter a, b: ";
    cin >> a >> b;
   #ifndef MODULESLASTNAME_H
#define MODULESLASTNAME_H

int s_calculation(int x, int y, int z, char a, char b) {
    // Додайте код обчислення s за допомогою x, y, z, a та b
    return 0;
}

#endif // MODULESLASTNAME_H

    cout << "s = " << s << endl;
    return 0;
}


Варіант № 6


Кропивницький | <a href="http://www.kntu.kr.ua/">ЦНТУ</a> | 2023
