#include<iostream>
using namespace std;

int main() {

//利用冒泡排序实现升序序列
听完分析后我的代码：
	int arr[5] = { 94,23,98,2049,34};
	for (int j = 0;j < 4;j++) {
		for (int i = 0;i < 4;i++) {
			int temp = 0;
			if (arr[i] > arr[i + 1]) {
				temp = arr[i];
				arr[i] = arr[i + 1];
				arr[i + 1] = temp;
			}
		}
	}
	for (int a = 0;a < 5;a++) {
		cout << arr[a] << endl;
	}
}




