```c++
#include<bits/stdc++.h>
using namespace std;

int fact(int n) {
	int sum = 1;
	for (int i=1; i<=n; i++) sum *= i;
	return sum;
}

int main() {
	int n;
	cin >> n;
	cout << fact(n);
	return 0;
}
```