#include<iostream>
using namespace std;

int main() {
	/*
	* 一维数组名称用途
	* 1.可以统计整个数组在内存中的长度
	* 2.可以获取数组在内存中的首地址
	*/

	//1.
	int arr[5] = { 1,2,3,4,5 };
	cout << sizeof(arr) << endl;
	cout << sizeof(arr[0]) << endl;
	cout << sizeof(int) << endl;
	

	//2.可以获取数组在内存中的首地址
	cout << "数组首地址为：" << arr << endl;
	cout << "数组首地址为：" << (int)arr  << endl;
	cout << "数组中第一个元素的地址为" << &arr[0] << endl;
	//关于为什么arr不用&而arr[0]需要，因为arr本身就是一个地址，而arr[0]是一个数据，
	//而&是一个地址符，这样才能找到arr[0]的地址

	//注意不能给数组名再赋值，因为这个时候数组名已经表示一个地址
	system("pause");
	return 0;
}

善用数组（五只小猪称体重）：
#include<iostream>
using namespace std;

int main() {
	int pig_weight[5];
	for (int j = 0; j < 5;j++) {
		cin >> pig_weight[j];
	}
	int max = 0;
	for (int i = 0; i < 4;i++) {
		if (pig_weight[i] > max) {
			max = pig_weight[i];
		}
	}
	cout << max << endl;
}


利用数组（元素逆置）：
#include<iostream>
using namespace std;

int main() {
	int arr[5] = { 0,1,2,3,4 };
	int start = 0;
	int end = sizeof(arr) / sizeof(arr)[0] - 1;//此为末尾元素的下标
	// start 和 end下标元素进行互换
	while (start < end) {

		//实现元素互换
		int temp = arr[start];
		arr[start] = arr[end];
		arr[end] = temp;


		//下标更新
		start++;
		end--;

	}
	for (int i = 0; i < 5; i++) {
		cout << arr[i] << endl;
	}
	system("pause");
	return 0;
}
