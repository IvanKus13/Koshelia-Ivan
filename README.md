#include <iostream>
#include <cmath> // Для математичних функцій
#include <Windows.h> // Для Укр мови
#include <stdlib.h>

int main() {
SetConsoleOutputCP(1251);
std::cout << "Lab 1 Koshelia Ivan,group 14, task 1" << std::endl;
std::cout << "Порахуйте вираз:abs(1 - B) * abs(1 - A) / ((1 + sin(C)) * (1 + cos(C)) * sqrt(1 / 2.0))" << std::endl;


	double A, B, C;
	std::cout << "Введіть значення A:";
	std::cin >> A;
	std::cout << "Введіть значення B:";
	std::cin >> B;
	std::cout << "Введіть значення C:";
	std::cin >> C;
	if ((1 + sin(C)) == 0) { // Зробимо ОДЗ щоб не отримати помилку в розрахунках
		std::cout << "Помилка:sin не може дорівнювати 0" << std::endl;
	} if((1 + cos(C)) == 0) {
		std::cout << "Помилка:cos не може дорівнювати 0" << std::endl;
	}
	

	double result = abs(1 - B) * abs(1 - A) / ((1 + sin(C)) * (1 + cos(C)) * sqrt(1 / 2.0));
	std::cout << "Відповідь:" << result << std::endl;
		
	


	return 0;





}
