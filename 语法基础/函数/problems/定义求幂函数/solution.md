```c++
#include<bits/stdc++.h>
using namespace std;

int poww(int n, int x) {
	int sum = 1;
	for (int i=1; i<=x; i++) sum *= n;
	return sum;
}

int main() {
	int n, x;
	cin >> n >> x;
	cout << poww(n, x);
	return 0;
}
```