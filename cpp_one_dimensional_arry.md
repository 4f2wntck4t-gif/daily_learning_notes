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
	system("pause");
	return 0;
}
