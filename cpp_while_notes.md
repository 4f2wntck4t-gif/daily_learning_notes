猜数字游戏


#include<iostream>
using namespace std;
#include<ctime>
int main() {

	srand((unsigned int)time(NULL));
  	//添加随机数种子，利用当前系统时间生成随机数，防止随机数都一样
	int num = rand() % 100 + 1;//仅有此行代码，生成的随机数都是一样的，为42
	int guess = 0;
	while (1) {
		cin >> guess;
		if (num > guess) {
			cout << "猜测小了" << endl;
		}
		else if (num < guess) {
			cout << "猜测大了" << endl;
		}
		else {
			cout << "猜测正确" << endl;
			break;
		}
	}
}
