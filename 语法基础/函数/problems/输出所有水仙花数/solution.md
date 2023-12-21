```c++
#include<bits/stdc++.h>
using namespace std;

bool check(int n) {
	int a = n%10, b = n/10%10, c = n/100%10;
	return a*a*a+b*b*b+c*c*c == n;
}

int main() {
	for (int i=100; i<=999; i++) {
		if (check(i)) cout << i << '\n';
	}
    return 0;
}
```