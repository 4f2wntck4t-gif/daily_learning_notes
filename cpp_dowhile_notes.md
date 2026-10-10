do...while 循环，先执行一遍语句 后循环

#include<iostream>
using namespace std;

int main() {

	int num = 0;
	do {
		cout << num << endl;
		num++;

	} while (num < 10);
	system("pause");
	return 0;
}

while 与do...while区别在于
while先判断条件而do...while后判断条件。
