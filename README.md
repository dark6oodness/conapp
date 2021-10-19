




#include <iostream>
using namespace std;

  
  /*функции, передача аргументов (параметров) */

  
  void FillArray(int arr[], const int size)
  {
	for (int i = 0; i < size; i++)
	{
		arr[i] = rand() % 10;
	}
}
void PrintArray(int arr[], const int size)
{
	for (int i = 0; i < size; i++)
	{
		cout << arr[i] << endl;
	}
}
void main()
{
	setlocale(LC_ALL, "ru");
	const int SIZE = 10;// константная переменная которая хранит массив (массив из 10 элементов)
	int arr[SIZE];// говори массиву что он размером 10 элементов 

	FillArray(arr, SIZE);
	PrintArray(arr, SIZE);


}
