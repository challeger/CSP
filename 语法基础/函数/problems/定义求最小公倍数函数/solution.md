```c++
#include<bits/stdc++.h>
using namespace std;

int lcm(int a, int b) {
	int t = max(a, b);
	for (int i=t; ; i+=t) {
		if (i%a==0 and i%b==0) return i;
	}
}

int main() {
	int a, b;
	cin >> a >> b;
	cout << lcm(a, b);
	return 0;
}
```