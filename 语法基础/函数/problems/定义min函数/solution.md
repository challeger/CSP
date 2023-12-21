```c++
#include<bits/stdc++.h>
using namespace std;

int minn(int a, int b) {
	if (a > b) return b;
	else return a;
}

int main() {
	int a, b;
	cin >> a >> b;
	cout << minn(a, b);
	return 0;
}
```
