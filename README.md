#include <iostream>
#include <ctime> // библиотека вызывается для гинерации случайных чисел
using namespace std;

int main()
{
	int const H = 10, W = 10;
	int m[H][W]{};
	srand(time(0));// функиця гинерирует случайные числа

	for (int j = 1; j < H; j++)
	{
		for (int i = 0; i < W; i++)
		{
			m[j][i] = rand() % 10;
		}
	}

	for (int j = 1; j < H; j++)
	{
		for (int i = 0; i < W; i++)
		{
			cout << m[j][i] << " ";
		}
		cout << "\n";
	}
}
