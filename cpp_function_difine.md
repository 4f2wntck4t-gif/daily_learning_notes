函数的定义：
1.返回值类型
2.函数名
3.参数表列
4.函数体语句
5.return表达式

语法：

返回值类型 函数名（参数列表）{

  函数体语句

  return表达式
}

#include<iostream>
using namespace std;
//函数定义时，num1 和num2并没有真实数据，只是形式上的参数，即形参
int add(int num1,int num2) { //返回值类型+函数名称 (参数列表)
	int sum = num1 + num2;//函数体语句
	return sum;//return表达式
}

int main() {
	//main函数中调用add函数
	int a = 10;
	int b = 10;

	//函数调用语法：函数名称（参数）
	 
	int c = add(a, b);//a，b为实际参数，即实参
	cout << c << endl;
	system("pause");
	return 0;
}
