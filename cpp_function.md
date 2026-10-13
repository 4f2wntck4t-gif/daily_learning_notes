#include<iostream>
using namespace std;

//如果函数不需要返回值，声明的时候可以写void
//形参的改变不影响实参
void swap(int num1, int num2) {
	
	cout << "交换前" << num1 << " " << num2 << endl;
	int temp = num1;
	num1 = num2;
	num2 = temp;
	cout << "交换后" << num1 << " " << num2 << endl;
	return;//这里return后不需要加东西
}

int main() {
	int a = 10;
	int b = 20;
	swap(a, b);
	cout << a << " " << b << endl;
	return 0;
}
