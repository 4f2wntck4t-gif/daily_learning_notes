#include<iostream>
using namespace std;
//函数的声明
//此前，如果将main函数写在前面，将max函数写在后面，因为编译器是一行一行读的，所以可能会报错
//因此，我们要告诉编译器有这个函数

//int max(int a, int b);

//声明可以写多次，但定义只能写一次
int main() {
	int a = 10;
	int b = 20;
	int c = max(a, b);
	cout << c << endl;
	return 0;
}

int max(int a, int b) {
	return a > b ? a : b;//三目运算符
}
