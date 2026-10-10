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

利用do...while 的实例--水仙花数
#include<iostream>
using namespace std;

int main() {

	//水仙花数
	int num = 99;
	do {
		num++;
		int c = num % 10;
		int b = ((num - c) / 10) % 10;
		int a = ((num - c - 10 * b) / 100);
		if (num == a * a * a + b * b * b + c * c * c) {
			cout << num << endl;
		}

	} while (num < 999);
	system("pause");
	return 0;
}


对30行-34行代码的修改：

int c = num %10;
int b = (num / 10 ) % 10;
int a = num / 100;

因为c++中整数/整数不可能出现小数，所以此处不用减c或减b*10之类的操作
