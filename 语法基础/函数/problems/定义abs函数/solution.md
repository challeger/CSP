```c++
#include<bits/stdc++.h>
using namespace std;

int abss(int a, int b) {
	if (a > b) return a-b;
	else return b-a;
}

int main() {
	int a, b;
	cin >> a >> b;
	cout << abss(a, b);
	return 0;
}
```
