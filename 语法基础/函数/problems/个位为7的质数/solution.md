```c++
#include<bits/stdc++.h>
using namespace std;
int n, m;

int is_prime(int x) {
	if (x <= 1) return 0;
	for (int i=2; i<=x/i; i++) {
		if (x%i == 0) return 0;
	}
	return 1;
}

int main() {
	int n, m, flag=0;
	cin >> n >> m;
	for (int i=n; i<=m; i++) {
		if (is_prime(i) and i%10==7) {
			cout << i << '\n';
			flag = 1;
		}
	}
	if (flag == 0) cout << -1;
	return 0;
}
```