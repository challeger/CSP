```c++
// 也可以使用辗转相除法
#include<bits/stdc++.h>
using namespace std;

int gcd(int a, int b) {
	for (int i=min(a, b); i>=1; i--) {
		if (a%i==0 and b%i==0) return i;
	}
}

int main() {
	int a, b;
	cin >> a >> b;
	cout << gcd(a, b);
	return 0;
}
```