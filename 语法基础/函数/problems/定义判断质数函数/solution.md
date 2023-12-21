```c++
#include<bits/stdc++.h>
using namespace std;

bool is_prime(int n) {
	if (n <= 1) return 0;
	for (int i=2; i<=n/i; i++) {
		if (n%i == 0) return 0;
	}
	return 1;
}

int main() {
	int n;
	cin >> n;
	if (is_prime(n)) cout << "yes";
	else cout << "no";
	return 0;
}
```