#include<iostream>
using namespace std;

//函数常见样式
//1.无参无返2.有参无返3.无参有返4.有参有返

//1.无参无返
void test01() {
	cout << "this is you" << endl;
}
//2.有参无返
void test02(int a) {
		cout << a << endl;
}
//3.无参有返
int test03() {
	cout << "that is he" << endl;
	return 1000;
}
//4.有参有返
int test04(int a) {
	cout << "this is test04" << endl;
	return a;
}

int main() {
	test01();
	test02(100);
	test03();
	int num1 = test03();
	cout << num1 << endl;
	int num2 = test04(1000);
	cout << num2 << endl;
	return 0;
}
